# Projeto Laravel

Aplicação web desenvolvida com PHP e Laravel, com estrutura de banco de dados, rotas, views e recursos de frontend.

## Tecnologias

- PHP
- Laravel
- Composer
- Banco de dados relacional
- Vite

## Estrutura principal

- `app/` — código da aplicação;
- `database/` — migrations e dados do banco;
- `resources/` — recursos da interface;
- `routes/` — rotas;
- `public/` — arquivos públicos;
- `tests/` — testes.

## Como executar

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
npm install
npm run build
php artisan serve
```

Configure o banco de dados no `.env` antes de executar as migrations. Não publique esse arquivo.

## Status

Projeto em desenvolvimento.
