# Base Project

Este repositório contém um projeto base pré-configurado para iniciar novos projetos rapidamente.

## Estrutura do Projeto

A estrutura do projeto é organizada para facilitar o desenvolvimento e a manutenção:

```
Base-Project/
├── app/                  # Contém a lógica da aplicação
│   ├── Contracts/        # Interfaces para contratos
│   ├── Core/             # Componentes centrais (Request, Response, Router)
│   ├── Database/         # Conexão com o banco de dados
│   ├── Helpers/          # Funções auxiliares
│   ├── Http/             # Controladores e Middlewares
│   ├── Providers/        # Provedores de serviço
│   └── Routes/           # Definição de rotas (web.php)
├── docker/               # Configurações Docker
│   ├── nginx/            # Configuração Nginx
│   └── php/              # Configuração PHP (Dockerfile, ini)
├── public/               # Arquivos públicos (index.php)
├── resources/            # Recursos da aplicação
│   └── views/            # Views (home.php, layouts, partials)
├── composer.json         # Dependências PHP
├── docker-compose.yml    # Orquestração Docker
└── .env-example          # Exemplo de variáveis de ambiente
```

## Tecnologias Utilizadas

*   **PHP**: Linguagem de programação principal.
*   **Docker**: Para conteinerização do ambiente de desenvolvimento.
*   **Nginx**: Servidor web.

## Como Usar

Para configurar e executar o projeto localmente, siga os passos abaixo:

### 1. Clonar o Repositório

```bash
git clone https://github.com/NathanGuedes/Base-Project.git
cd Base-Project
```

### 2. Configurar Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto, copiando o `.env-example` e preenchendo com suas configurações:

```bash
cp .env-example .env
# Edite o arquivo .env conforme necessário
```

### 3. Iniciar o Ambiente Docker

Navegue até o diretório raiz do projeto e inicie os contêineres Docker:

```bash
docker-compose up -d --build
```

### 4. Acessar a Aplicação

Após os contêineres estarem em execução, a aplicação estará disponível em `http://localhost` (ou na porta configurada no Nginx/Docker Compose).

## Autor

Nathan Guedes Pessoa



