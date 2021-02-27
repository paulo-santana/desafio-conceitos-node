# Primeiro desafio do bootcamp GoStack 11.0

Este desafio é sobre a cração de uma simples API REST rodando em NodeJS.
Ele ainda não abrange uma conexão a um banco de dados, então as informações são todas armazenadas na memória com uma Array.

Para testá-lo, depois de clonar o repositório, entre na pasta raíz do projeto e digite no terminal:

```bash
npm install && npm run dev 
# ou yarn && yarn dev
```

Alimente com alguns dados de entrada:

```bash
curl -X POST \
-H "Content-Type: application/json" \
-d '{"title":"desafio-conceitos-nodejs","url":"https://github.com/paulo-santana/desafio-conceitos-node","techs":["Node.js","Express.js"]}' http://localhost:3333/repositories

curl -X POST \
-H "Content-Type: application/json" \
-d '{"title":"CS50","url":"https://github.com/paulo-santana/cs50","techs":["C","SQL", "Algorithms and Data Structures"]}' http://localhost:3333/repositories
```

Abra http://localhost:3333/repositories e veja os repositórios armazenados!

Verifique os testes com `npm run test` ou `yarn test`
