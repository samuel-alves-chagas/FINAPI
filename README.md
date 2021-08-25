## FinAPI - Financeira

API financeira utilizando o padrão de arquitetura REST.

---

## Pré-requisitos

Ter instalado o node e yarn em sua máquina.

---

## Executando o Projeto:

#### Clonando o projeto

```sh
$ git clone https://github.com/triangulodepascal/FINAPI.git
$ cd FINAPI
```

#### Rodando o back-end

```sh
  # Instalar as dependências:
  $ yarn

  # Rodar a aplicação
  yarn dev
```

---

## Instruções:

    Requisições feitas via Insomnia

    URL para acessar as rotas: http://localhost:3333

    Rota para criar uma conta: POST - http://localhost:3333/account
        Os dados devem ser passado via JSON no body.
        Ex.:
        body
        {
            "cpf": "111.111.111-11"
            "name": "João da Silva",
        }

---

### Requisitos:

- [x] Deve ser possivel criar uma conta
- [x] Deve ser possivel buscar o extrato bancário do cliente
- [x] Deve ser possivel realizar um depósito
- [ ] Deve ser possivel realizar um saque
- [ ] Deve ser possivel busca o extrato bancário do cliente por data
- [ ] Deve ser possivel atualizar dados da conta do cliente
- [ ] Deve ser possivel obter dados da conta do cliente
- [ ] Deve ser possivel deletar uma conta
- [ ] Deve ser possivel retornar o balance

## Regras de negócio

- [x] Não deve ser possivel cadastrar uma conta com CPF já existente
- [x] Não deve ser possivel buscar extrato em uma conta não existente
- [x] Não deve ser possivel fazer depósito em uma conta não existente
- [ ] Não deve ser possivel fazer saque em uma conta não existente
- [ ] Não deve ser possivel excluir uma conta não existente
- [ ] Não deve ser possivel fazer saque quando o saldo for insuficiente
- [ ] Não deve ser possivel buscar o balance em uma conta não existente
