# Projrto_laravel

Este repositório contém um projeto de aplicação web desenvolvido com o framework Laravel, indicando uma estrutura robusta para funcionalidades de backend.

## Descrição do Projeto

O projeto é uma aplicação web construída utilizando o Laravel, um dos frameworks PHP mais populares. A estrutura de arquivos e o `composer.json` sugerem uma aplicação completa, possivelmente com autenticação de usuário (`laravel/sanctum`, `laravel/ui`), gerenciamento de banco de dados (`database/`, `laravel.sql`), e rotas definidas (`routes/`). O foco pode ser em um sistema de gerenciamento de conteúdo, e-commerce, ou qualquer outra aplicação que demande um backend sólido. O arquivo `laravel.sql` indica a presença de um esquema de banco de dados, o que é fundamental para a persistência de dados da aplicação.

## Funcionalidades (Potenciais)

*   Autenticação e autorização de usuários.
*   Gerenciamento de dados com banco de dados (MySQL/MariaDB, SQLite, PostgreSQL).
*   APIs RESTful (com Laravel Sanctum).
*   Interface de usuário (com Laravel UI ou Blade templates).

## Tecnologias Utilizadas

*   **PHP:** Linguagem de programação principal.
*   **Laravel:** Framework web para PHP.
*   **Composer:** Gerenciador de dependências para PHP.
*   **MySQL/MariaDB:** (Provável) Banco de dados relacional, indicado pelo arquivo `laravel.sql`.
*   **Vite:** Ferramenta de build frontend (indicado por `vite.config.js`).
*   **JavaScript/Blade:** Para o frontend.

## Como Configurar e Rodar o Projeto

Para configurar e executar este projeto localmente, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/DAVIWENDELL/Projrto_laravel.git
    cd Projrto_laravel
    ```
2.  **Instale as dependências do Composer:**
    Certifique-se de ter o PHP e o Composer instalados.
    ```bash
    composer install
    ```
3.  **Configure o ambiente:**
    Crie um arquivo `.env` a partir do `.env.example` e configure as variáveis de ambiente, especialmente as credenciais do banco de dados.
    ```bash
    cp .env.example .env
    php artisan key:generate
    ```
4.  **Configure o banco de dados:**
    Importe o arquivo `laravel.sql` para o seu banco de dados (ex: MySQL) e execute as migrações (se houver).
    ```bash
    php artisan migrate
    ```
5.  **Instale as dependências do Node.js e compile os assets:**
    ```bash
    npm install
    npm run dev
    # ou para produção
    # npm run build
    ```
6.  **Execute o servidor Laravel:**
    ```bash
    php artisan serve
    ```
7.  **Acesse a aplicação:**
    Abra seu navegador e acesse `http://127.0.0.1:8000/` (ou o endereço indicado no terminal).
