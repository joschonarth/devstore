<div align="center">

<img height="160" alt="devstore" src="/src/app/icon.png" />

# devstore

*O e-commerce de roupas feito por devs, para devs.*

[![last commit](https://img.shields.io/github/last-commit/joschonarth/devstore?style=for-the-badge&color=8b5cf6&labelColor=27272a)](https://github.com/joschonarth/devstore/commits/main)
[![top language](https://img.shields.io/github/languages/top/joschonarth/devstore?style=for-the-badge&color=8b5cf6&labelColor=27272a)](https://github.com/joschonarth/devstore)
[![languages count](https://img.shields.io/github/languages/count/joschonarth/devstore?style=for-the-badge&color=8b5cf6&labelColor=27272a)](https://github.com/joschonarth/devstore)

---

📃 [Sobre](#-sobre)&nbsp;&nbsp;•&nbsp;&nbsp;🛠️ [Tecnologias](#-tecnologias)&nbsp;&nbsp;•&nbsp;&nbsp;✨ [Funcionalidades](#-funcionalidades)&nbsp;&nbsp;•&nbsp;&nbsp;🚀 [Como rodar](#-como-rodar)&nbsp;&nbsp;•&nbsp;&nbsp;🧪 [Testes](#-testes)&nbsp;&nbsp;•&nbsp;&nbsp;⚙️ [CI](#-ci)

</div>

---

## 📃 Sobre

O **devstore** é um e-commerce simulado de roupas com identidade voltada para desenvolvedores. O projeto foi construído com foco em arquitetura moderna com **Next.js App Router**, tipagem estática com **TypeScript**, validação robusta de dados com **Zod**, estilização utilitária com **Tailwind CSS** e qualidade garantida por testes **E2E com Cypress** e um pipeline de **CI com GitHub Actions**.

---

## 🛠️ Tecnologias

- ⚡ **[Next.js](https://nextjs.org/)** — Framework React com App Router, SSR e otimizações de performance.
- ⚛️ **[React](https://react.dev/)** — Biblioteca para construção de interfaces declarativas.
- 🟦 **[TypeScript](https://www.typescriptlang.org/)** — Tipagem estática e segurança em tempo de desenvolvimento.
- 🎨 **[Tailwind CSS](https://tailwindcss.com/)** — Estilização utilitária direto no JSX.
- 🔀 **[tailwind-merge](https://github.com/dcastil/tailwind-merge)** — Resolução inteligente de conflitos entre classes Tailwind.
- 🛡️ **[Zod](https://zod.dev/)** — Validação e parsing de schemas com inferência de tipos.
- 🔑 **[T3 Env](https://env.t3.gg/)** — Tipagem e validação de variáveis de ambiente em tempo de build.
- 🧪 **[Cypress](https://www.cypress.io/)** — Testes end-to-end no navegador.
- 🔍 **[ESLint](https://eslint.org/)** — Linting e padronização de código.
- 🔄 **[GitHub Actions](https://github.com/features/actions)** — Integração contínua e automação do pipeline de testes.

---

## ✨ Funcionalidades

- [x] 🛒 Listagem de produtos com layout em grade
- [x] 🔍 Página de detalhes do produto
- [x] 🛍️ Carrinho de compras
- [x] 🛡️ Validação de dados com Zod
- [x] 🔑 Variáveis de ambiente tipadas e seguras com T3 Env
- [x] 📱 Layout totalmente responsivo
- [x] 🧪 Testes E2E com Cypress
- [x] 🔄 Pipeline de CI rodando os testes a cada push

---

## 🚀 Como rodar

### 📋 Pré-requisitos

- 🟩 [Node.js 18+](https://nodejs.org/)
- 📦 [pnpm](https://pnpm.io/)

### 🔧 Instalação

1. Clone o repositório:

    ```bash
    git clone https://github.com/joschonarth/devstore.git
    ```

2. Acesse a pasta do projeto:

    ```bash
    cd devstore
    ```

3. Instale as dependências:

    ```bash
    pnpm install
    ```

4. Configure as variáveis de ambiente copiando o arquivo de exemplo e renomeando para `.env.local`:

    ```bash
    cp .env.local.example .env.local
    ```

    Em seguida, abra o arquivo `.env.local` e preencha as variáveis conforme necessário.

### 🔌 API

Este projeto consome a **devstore-api**, uma API de produtos que precisa estar disponível para que a aplicação funcione corretamente.

Acesse o repositório abaixo, faça o deploy na sua conta da Vercel com um clique e copie a URL gerada:

👉 **[devstore-api](https://github.com/joschonarth/devstore-api)**

Após o deploy, adicione a URL no arquivo `.env.local`:

```env
NEXT_PUBLIC_API_BASE_URL=https://sua-devstore-api.vercel.app
```

### ▶️ Execução

```bash
# Inicia o servidor de desenvolvimento
pnpm dev
```

Acesse **[http://localhost:3000](http://localhost:3000)** no navegador.

```bash
# Gera o build de produção
pnpm build

# Inicia o servidor de produção
pnpm start
```

---

## 🧪 Testes

Os testes **E2E** são escritos com **Cypress** e cobrem os principais fluxos da aplicação.

```bash
# Abre o Cypress no modo interativo
npm run cypress:open

# Roda todos os testes em modo headless
npm run cypress:run
```

---

## ⚙️ CI

O projeto conta com um workflow de **Integração Contínua** via **GitHub Actions**. A cada `push` para a branch principal, o pipeline é acionado automaticamente e executa todos os testes E2E para garantir que nenhuma funcionalidade foi quebrada antes do merge.

```txt
.github/
└── workflows/
    └── run-e2e.yml
```

---

## ⭐ Apoie este Projeto

Se curtiu o projeto, deixe uma ⭐ aqui no GitHub — isso ajuda muito!

---

<div align="center">

Feito com ♥ por **[João Otávio Schonarth](https://github.com/joschonarth)**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/joschonarth)
[![GitHub](https://img.shields.io/badge/GitHub-171515?style=for-the-badge&logo=github&logoColor=white)](https://github.com/joschonarth)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:joschonarth@gmail.com)

</div>
