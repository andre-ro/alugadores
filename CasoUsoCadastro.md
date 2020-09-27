## Caso de Uso: Cadastro

![image3](https://i.ibb.co/WGnBmM2/Modelo-Negocio-Cadastro.png)

| _                  | _   |
|:-------------------|:----|
| Identificador      | UC001 |
| Nome               | Solicitar Cadastro |
| Atores             | Cliente |
| Sumário            | Permitir o cliente solicitar um cadastro de suas informações básicas na plataforma Alugadores |
| Complexidade       | Alta |
| Regras de Negócio  | _ |
| Pré-condições      | Nenhuma |
| Pós-condição       | Informar o cliente que seu cadastro foi efetuado e armazenado com segurança |
| Pontos de Inclusão |Não há |
| Pontos de Extensão | Não há |

**Fluxo Principal**
| Ações do Ator                    | Ações do Sistema |
|:---------------------------------|:-----------------|
| 1) Cliente pede para se cadastrar | 2) Sistema exibe o formulário de cadastro (nome, email, cpf, informações de pagamento) |
| 3) Cliente preenche o formulário  | 3) Sistema valida e armazena os dados |
|                                   | 4) Sistema envia email de verificação |
| 5) Cliente acessa seu e-mail e valida o e-mail clicando no link de validação enviado por e-mail | 6) Sistema valida e armazena os dados 
|                                                                                                 | 7) Sistema exibe termos e condições da plataforma
| 8) Cliente aceita termos e condições | |
| 9) Cliente está cadastrado           | |


**Fluxo Alternativo:** Email Invalido
| Ações do Ator                    | Ações do Sistema |
|:---------------------------------|:-----------------|
| 1) Cliente pede para se cadastrar | 2) Sistema exibe o formulário de cadastro (nome, email, cpf) |
| 3) Cliente preenche o formulário  | 4) Sistema valida **[ERRO] email invalido** |
|                                   | 5) Sistema informa email invalido |


**Fluxo Alternativo:** CPF Inválido
| Ações do Ator                    | Ações do Sistema |
|:---------------------------------|:-----------------|
| 1) Cliente pede para se cadastrar | 2) Sistema exibe o formulário de cadastro (nome, email, cpf) |
| 3) Cliente preenche o formulário  | 4) Sistema valida **[ERRO] CPF invalido** |
|                                   | 5) Sistema informa CPF invalido |


**Fluxo Alternativo:** Informações de Pagamento Invalido
| Ações do Ator                    | Ações do Sistema |
|:---------------------------------|:-----------------|
| 1) Cliente pede para se cadastrar | 2) Sistema exibe o formulário de cadastro (nome, email, cpf) |
| 3) Cliente preenche o formulário  | 4) Sistema valida **[ERRO] Informações de Pagamento Invalido** |
|                                   | 5) Sistema informa Informações de Pagamento Invalido |
