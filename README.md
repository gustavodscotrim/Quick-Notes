# Quick Notes ✍️📜

Bem-vindo ao Quick Notes! Esta aplicação foi desenvolvida como projeto de Extensão do Curso de Análise e Desenvolvimento de Sistemas (ADS) do Centro Universitário Filadélfia - UniFil. Objetivamos com esta aplicação ofertar uma plataforma para gerenciar suas anotações e informações importantes. Se você não está convencido dos motivos pelos quais deveria adotar um aplicativo de notas, continue lendo para descobrir como Quick Notes pode contribuir em sua vida.

### Acessibilidade em Qualquer Lugar

Uma das vantagens mais evidentes de usar um aplicativo de notas é a acessibilidade. Não importa se você está no trabalho, em casa ou no trânsito, você pode acessar suas notas a partir de qualquer dispositivo conectado à internet. A sincronização automática garante que suas informações estejam sempre atualizadas e disponíveis quando e onde você precisar delas.

### Facilidade de Uso 💯

Nossa interface foi projetada pensando na facilidade de uso. Você não precisa ser um especialista em tecnologia para começar a criar e editar suas notas. Comece a usar este aplicativo web e aproveite a simplicidade.

### Privacidade e Segurança 📎

Preocupado com a segurança de suas informações? Esta aplicação oferece recursos para proteger suas anotações sensíveis. Utilizamos autenticação Google para garantir que apenas você tenha acesso ao conteúdo.

## Tecnologias

- [Node.js](https://nodejs.org/en)
- [mongoDB](https://www.mongodb.com/) (noSQL Database)
- [Passport](https://www.passportjs.org/) (Authentication Middleware)
- [Express.js](https://expressjs.com/) (Web Framework)
- [Template Engine](https://getbootstrap.com/) (EJS & Bootstrap)

## Rotas (API)

Funcionalidade  | HTTP  | Rota
--------- | --------- | ------
Dashboard | GET| "/dashboard"
Notes | GET | "/dashboard/item/:id"
Notes | PUT | "/dashboard/item/:id"
Notes | DELETE | "/dashboard/item-delete/:id"
New Note | GET | "/dashboard/add"
New Note | POST | "/dashboard/add"
Search | GET | "/dashboard/search"
Search | POST | "/dashboard/search"
Login | GET | "/auth/google"
Auth RollBack | GET | "/google/callback"
Logout | GET | "/logout"

## Requisitos Mínimos 🖥

- Node.js (14.18.2)
- Npm (6.14.15)
- Visual Studio Code
- mongoDB (mongoose 6.8.1)

## Configuração do arquivo ".env"
Crie um arquivo ".env" no diretório raiz do projeto para armazenar suas credênciais, como o exemplo abaixo:

```
MONGODB_URI = mongodb+srv://<username>:<password>@<mongodburlhere>?retryWrites=true&w=majority
GOOGLE_CLIENT_ID= SUA_GOOGLE_ID_AQUI
GOOGLE_CLIENT_SECRET= SUA_GOOGLE_CLIENT_SECRET_AQUI
GOOGLE_CALLBACK_URL=http://localhost:5000/google/callback

```

## Instalação 👇🏻

Clone o projeto em um diretório local e utilize o terminal para instalação de todas as dependências do projeto utilizando o "npm install" e, posteriormente, "npm start" para inicialização do servidor da aplicação". Após isso, o projeto será inicializado, e uma página do navegador será aberta (http://localhost:5000/).

```
$ npm install
$ npm start
```
