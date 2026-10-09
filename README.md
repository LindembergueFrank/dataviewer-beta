# DataViewer Beta

Cópia de estudo do [DataViewer Beta do Natalnet](https://github.com/Natalnet/dataviewer-beta), voltado à visualização de dados educacionais. A autoria original e a licença [GPL-2.0](LICENSE) são preservadas.

## Tecnologias

- Backend: TypeScript, NestJS 9, MongoDB/Mongoose e módulos de autenticação.
- Frontend: Next.js, React 18, Material UI e Recharts.
- Dockerfiles independentes em `backend/` e `frontend/`.

## Organização

| Diretório | Responsabilidade |
| --- | --- |
| [backend](backend/) | API, módulos de usuários, autenticação, turmas, estudantes e coordenação. |
| [frontend](frontend/) | Interface web e visualização dos dados. |

## Desenvolvimento local

Prepare um MongoDB de desenvolvimento e configure os valores indicados em `backend/.env.example` e `frontend/.env.example`. Não reutilize configurações de produção do acervo.

Em um terminal:

```sh
cd backend
npm install
npm run start:dev
```

O backend escuta a porta 3333. Em outro terminal:

```sh
cd frontend
npm install
npm run dev -- --port 3000
```

A interface fica em http://localhost:3000. Configure `NEXT_PUBLIC_API_URL` para o endereço da API e `DATABASE_HOST` conforme o ambiente.

## Comandos disponíveis

- Backend: `npm test`, `npm run test:e2e` e `npm run build`.
- Frontend: `npm run build`.

Esses comandos constam dos manifestos; a execução completa não foi validada nesta revisão documental. As dependências e configurações refletem a versão preservada do projeto.

## Origem e contribuições

Este repositório é um fork. Alterações locais não representam a autoria integral do sistema nem uma implantação oficial. Consulte a [documentação do backend](backend/README.md) e a [documentação do frontend](frontend/README.md) para o material original.
