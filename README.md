# DataViewer Beta

Projeto de visualização de **dados educacionais** organizado em duas aplicações: um backend em **NestJS/TypeScript** e um frontend em **Next.js**.

O repositório preserva uma versão beta e seu histórico de desenvolvimento colaborativo. Ele deve ser lido como projeto de experimentação/evolução e não como um produto atualmente mantido em produção.

## Arquitetura

```text
Navegador
   │
Next.js (frontend/)
   │
API
   │
NestJS (backend/)
```

### Backend

O diretório `backend/` contém uma aplicação NestJS com:

- TypeScript;
- configuração ESLint e Prettier;
- testes;
- Dockerfile;
- variáveis de ambiente documentadas por `.env.example`;
- estrutura modular em `src/`.

### Frontend

O diretório `frontend/` contém uma aplicação Next.js com:

- páginas e componentes React;
- contexts e utilitários;
- estilos e assets públicos;
- Dockerfile;
- configuração por ambiente.

## Executando

Cada aplicação possui seu próprio `package.json`, lockfile, README e Dockerfile. Para desenvolvimento local, entre no diretório desejado e siga a documentação específica.

Exemplo geral com Yarn:

```bash
cd backend
yarn install
yarn start:dev
```

Em outro terminal:

```bash
cd frontend
yarn install
yarn dev
```

Consulte os arquivos `.env.example` antes de iniciar as aplicações e nunca versione credenciais reais.

## Estado do projeto

Este repositório é mantido principalmente como registro técnico de uma versão beta. Antes de utilizá-lo como projeto principal de portfólio ou colocá-lo novamente em produção, é recomendável validar dependências, suíte de testes, segurança, configuração de containers e compatibilidade das versões atuais do Node.js.

## O que o projeto demonstra

- separação entre frontend e backend;
- API com NestJS;
- interface web com Next.js/React;
- TypeScript;
- configuração por ambiente;
- uso de Docker;
- organização de um projeto full stack.

## Histórico e autoria

O histórico do Git registra contribuições de mais de uma pessoa. Para avaliar autoria de mudanças específicas, consulte os commits e pull requests do repositório.
