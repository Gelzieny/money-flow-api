# MoneyFlow API

**MoneyFlow** é uma API para gerenciamento do fluxo de dinheiro, permitindo controle de gastos, categorização de despesas, registro de receitas e monitoramento de investimentos.


## Funcionalidades

- Gerenciamento de contas financeiras
- Registro de receitas e despesas
- Controle de investimentos
- Categorização de gastos
- Relatórios de fluxo financeiro
- Integração com PostgreSQL
- Documentação automática via FastAPI (Swagger)


## Tecnologias

- **Python 3.11**
- **FastAPI** – Framework web
- **SQLAlchemy** – ORM para PostgreSQL
- **PostgreSQL** – Banco de dados relacional
- **Docker & Docker Compose** – Containerização e deploy
- **Pydantic** – Validação de dados
- **Uvicorn** – Servidor ASGI

---

## Estrutura do Projeto

````bash
MoneyFlow/
├─ src/
│ ├─ main.py # Ponto de entrada da aplicação
│ ├─ core/
│ │ ├─ config.py # Configurações da aplicação
│ │ └─ security.py
│ ├─ models/
│ │ └─ transaction.py # Modelos de banco de dados
│ ├─ routers/
│ │ ├─ users.py
│ │ ├─ transactions.py
│ │ └─ investments.py
│ ├─ services/
│ │ └─ transaction_service.py
│ └─ utils/
│ └─ helpers.py
├─ requirements.txt
├─ Dockerfile
└─ docker-compose.yml
````


## Endpoints Principais

`POST /users/` – Criar usuário
`POST /transactions/` – Adicionar transação
`GET /transactions/` – Listar transações
`POST /investments/` – Registrar investimento
`GET /reports/` – Gerar relatório financeiro

