# Aplicação de uma página de Administração de E-commerce

Esta é uma aplicação de administração de um E-commerce desenvolvida em TypeScript, utilizando Next.js, Tailwind CSS com o Shadcn/ui para estilização, Clerk para autenticação, Prisma em conjunto com o PlanetScale para gerenciamento do banco de dados e Stripe para obter relatórios de vendas do E-commerce.

A página de administração se comunica com a página de vendas, onde o projeto está localizado neste [repositório](https://github.com/pedrohxiv/ecommerce-store), para um funcionamento completo da aplicação.

## Descrição

Esta aplicação é uma solução de administração completa para o E-commerce, permitindo aos administradores acessar informações detalhadas sobre as vendas, gerenciar produtos e controlar os dados dos usuários. Ela utiliza tecnologias modernas, como React e Next.js, para fornecer uma experiência de usuário fluida e responsiva.

O Tailwind CSS em conjunto com o Shadcn/ui é utilizado para criar uma interface atraente e funcional, com componentes pré-estilizados que agilizam o desenvolvimento.

O Clerk é uma biblioteca de autenticação que oferece suporte à autenticação baseada em senhaless, permitindo que os usuários façam login de forma segura e sem a necessidade de senhas.

O Prisma é um ORM (Object-Relational Mapping) utilizado para interagir com o banco de dados do E-commerce. Ele facilita o gerenciamento dos dados, garantindo uma manipulação segura e eficiente.

O PlanetScale é utilizado para gerenciamento escalável do banco de dados, garantindo que a aplicação possa lidar com um grande volume de dados de forma eficiente.

O Stripe é utilizado para obter relatórios detalhados de vendas do E-commerce, fornecendo informações importantes sobre as transações, receitas e métricas de desempenho.

## Funcionalidades

- Autenticação de administradores com o Clerk, permitindo login seguro sem a necessidade de senhas.
- Gerenciamento de categorias, cores, tamanhos e produtos, permitindo adicionar, editar e excluir produtos do E-commerce.
- Visualização de relatórios de vendas detalhados, fornecidos pelo Stripe, com informações sobre transações, receitas e métricas de desempenho.
- Interação com o banco de dados do E-commerce utilizando o Prisma em conjunto com o PlanetScale para um gerenciamento escalável e seguro.

## Pré-requisitos

Antes de executar a aplicação, certifique-se de ter as seguintes dependências instaladas:

- Node.js
- npm ou Yarn

## Instalação

1. Faça o clone deste repositório para o seu ambiente local.
2. Navegue até o diretório do projeto no terminal.
3. Execute o comando `npm install` ou `yarn install` para instalar as dependências do projeto.

## Configuração

Antes de iniciar a aplicação, você precisará configurar as seguintes variáveis de ambiente:

- `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`: Chave de API do Clerk.
- `CLERK_SECRET_KEY`: Chave secreta do Clerk.
- `NEXT_PUBLIC_CLERK_SIGN_IN_URL`: /sign-in
- `NEXT_PUBLIC_CLERK_SIGN_UP_URL`: /sign-up
- `NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL`: /
- `NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL`: /
- `DATABASE_URL`: URL do banco de dados do PlanetScale
- `NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME`: Nome da sua conta Cloudinary.
- `STRIPE_API_KEY`:  Chave secreta do Stripe.
- `FRONTEND_STORE_URL`: http://localhost:3001
- `STRIPE_WEBHOOK_SECRET`: Chave secreta do webhook do Stripe.

Certifique-se de criar um arquivo `.env` na raiz do projeto e adicionar as variáveis de ambiente necessárias.

## Uso

Após a instalação e configuração, execute o seguinte comando para iniciar a aplicação:

```
npm run dev
```

Isso iniciará o servidor de desenvolvimento do Next.js e você poderá acessar a aplicação no seu navegador através do endereço `http://localhost:3000`.
