## 1. Revisão de Conceitos Básicos
* Métodos HTTP:

    * GET: Recupera informações do servidor (seguro e idempotente).

    * POST: Cria novos recursos no servidor.

    * PUT / PATCH: Atualizam informações (o PUT substitui o recurso por completo, enquanto o PATCH faz uma alteração parcial).

    * DELETE: Remove um recurso específico.

* **Endpoint**: URL específica que fornece acesso a um recurso ou funcionalidade na API.

* **JSON (JavaScript Object Notation)**: Formato leve de troca de dados estruturado em objetos (pares de chave/valor) e arrays (listas).

## 2. Construindo uma API com CRUD (Express.js)
Para evoluir o back-end e permitir operações completas de manipulação de dados, utilizamos o Express.js em conjunto com a biblioteca body-parser (para ler os dados enviados no corpo das requisições, como JSON) e um arquivo JSON local (data.json) para armazenamento.

### As Rotas CRUD da API:
* GET /api/notes: Lista todas as notas armazenadas.

* `POST /api/notes`: Adiciona uma nova nota (exige `titulo` e `texto`, gerando automaticamente um ID único e data de criação).

* `GET /api/notes/:id`: Retorna uma nota específica buscada pelo ID.

* `PUT /api/notes/:id`: Atualiza o conteúdo de uma nota existente pelo ID.

* `DELETE /api/notes/:id`: Remove uma nota específica com base no ID.

> Atenção ao CORS: É necessário configurar o cabeçalho de acesso externo (`Access-Control-Allow-Origin: '*'`) para que o front-end consiga consumir a API sem bloqueios de segurança do navegador.

3. Fluxo de Publicação (Deploy)
Back-end: O projeto Node.js/Express é enviado para o GitHub e hospedado na plataforma Render.

Front-end: A interface em React consome a URL gerada pelo Render e é publicada na Vercel.

4. Documentando APIs com o Postman
O que é: Ferramenta essencial e colaborativa para criar, testar, documentar e monitorar requisições HTTP.

Principais funções: Permite enviar requisições (GET, POST, etc.) de forma visual, organizar endpoints em coleções, testar códigos de resposta, utilizar variáveis de ambiente e gerar documentações técnicas automatizadas.