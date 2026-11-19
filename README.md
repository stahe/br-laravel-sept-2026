# Introdução passo a passo ao framework web [Laravel]

**O curso está disponível online aqui: [https://stahe.github.io/br-laravel-sept-2026/](https://stahe.github.io/br-laravel-sept-2026/)**

## Autor

O curso e todo o seu código foram escritos por **Claude**, a IA da Anthropic, **único autor**, a pedido de Serge Tahé (setembro de 2026).

## Visão geral

Este curso apresenta um guia passo a passo para construir uma aplicação web MVC com o framework **Laravel 13** e a linguagem **PHP 8.4**. As páginas HTML são geradas pelo servidor por meio de views **Blade**, sem framework JavaScript no navegador.

Ele adapta o curso [Introdução passo a passo ao framework web [Flask](https://stahe.github.io/br-flask-sept-2026/)], por sua vez baseado nos cursos [Spring MVC](https://stahe.github.io/br-springmvc-sept-2026/), [ASP.NET Core MVC](https://stahe.github.io/br-aspnetcoremvc-sept-2026/) e [NestJS](https://stahe.github.io/br-nestjs-html-sept-2026/). Os exemplos têm a mesma numeração e abordam os mesmos temas: você pode comparar os frameworks exemplo a exemplo.

## Conteúdo

| Capítulo | Tópicos | Exemplos |
|---|---|---|
| Actions, roteamento, respostas | rotas, controllers, respostas, redirecionamentos, service container | 01–06 |
| O modelo da action | parâmetros da requisição, binding, validação, requisições POST | 07–12 |
| A view e seu template | Blade, template, componentes, formulários, validação, Post/Redirect/Get, proteção CSRF | 13–21 |
| Internacionalização | Uma aplicação em francês e inglês | 22 |
| Escopos de dados | Requisição, sessão, cache, cookies | 23 |
| O ciclo de vida da requisição | middleware, binding de parâmetros, tratadores de exceção | 24 |
| Autenticação e autorização | JWT em um cookie, guards, papéis, CAPTCHA, limitação de taxa (rate limiting) | 25–27 |
| Arquitetura em camadas | web / lógica de negócio / DAO com Eloquent e MySQL | 28 |
| Estudo de caso | **RdvMedecins**, uma aplicação de agendamento de consultas médicas, explicada arquivo por arquivo | - |

O estudo de caso `rdvmedecins2-laravel` gerencia três papéis (administrador, médicos, pacientes): agendas, reservas, gerenciamento de médicos e clientes, criação de contas protegida por CAPTCHA e uma interface em francês/inglês. Ele usa o mesmo banco de dados `dbrdvmedecins2` das outras versões da aplicação.

## Pré-requisitos

- PHP 8.4 ou superior (extensões `intl`, `mbstring`, `openssl`, `pdo_mysql`);
- Composer 2;
- MySQL 8 ou MariaDB (Laragon no Windows);
- Visual Studio Code com as extensões PHP Intelense e Laravel;
- curl.

O código está disponível para download no site do curso. As pastas `vendor` não estão incluídas: `composer install` as cria, uma na pasta `exemples` e outra na pasta `rdvmedecins2-laravel`.
