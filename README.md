# Alugadores
Criada por pessoas que nunca encontraram uma forma eficiente em aluguel de bicicletas. Alugadores é uma empresa que visa facilitar o processo de alugação de biciletas da forma mais simples e prática possivel, a Alugadores irá espalhar bicicletas na sua cidade, cada uma com uma trava de segurança e um qrcode, ao abrir-lo, você será direcionado para um link onde, se ja possui cadastro, irá alugar a bicicleta automaticamente, destravando a trava de segurança. 

![image1](https://i.ibb.co/tLKwMV3/Alugadores-Flowchart.png)
*Flowchart de Operações da aplicação*

![image2](https://cdn.discordapp.com/attachments/751444249182208120/756253194400825354/DiagramaCasoDeUso.png)
*Diagrama de Caso de Uso da aplicação*

### Pedido
Quando um Qrcode é escaneado. com sucesso, pelo aplicativo um pedido contendo as informações essenciais do locatário e da bicicleta a ser alugada são enviados para um servidor de porcessos na forma de um pacote de dados seguro denominado "Pedido".

### Disponível
O pedido, no servidor, é analisado para verificar a disponibilidade da bicicleta. Caso ela esteja indisponível o servidor retornará uma mensagem de erro e quebrará o processo de pedidos.

### Pagamento
Em seguida as informações de pagamento, contidas no cadastro do pedido, são utilizadas em uma interface com o banco de escolha para efetuar a transação econômica.

### Efetuado
Se o estagio de pagamento foi executado com sucesso, o pedido segue para a última faze, Aluguel, caso contrário uma mensagem de erro é retornada e o pedido pode ser canselado dependendo da severidade do erro.

### Aluguel
Por último o, com o pedido confirmado a bicicleta recebe um sinal do servidor, que a desbloqueia pelo tempo necessário e retorna um recibo eletrônico ao usuário.

### Financeiro
Responsável pela gestão dos pagamentos.

## Integrantes
André Rodrigues - Estudante de ciência da computação no Mackenzie e database da Cryptal.

Eric Gregory - Estudante de ciência da computação no Mackenzie
