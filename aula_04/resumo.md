## 1. O que é uma API?
Uma **API** (Application Programming Interface ou Interface de Programação de Aplicações) é um conjunto de regras e ferramentas que permite que diferentes softwares se comuniquem entre si.

* **Estilo REST**: Arquitetura muito usada na web baseada em comunicação cliente-servidor sem estado (stateless), usando métodos HTTP e dados em formato JSON.

## 2. O Protocolo HTTP e Métodos
O HTTP é o protocolo que regula a troca de mensagens entre o cliente (navegador/front-end) e o servidor.

### Principais Métodos HTTP:
* **GET**: Recupera informações do servidor (seguro e idempotente).

* **POST**: Cria um novo recurso no servidor.

* **PUT** / **PATCH**: Atualizam informações. O PUT substitui o recurso por completo, enquanto o PATCH faz uma atualização parcial.

* **DELETE**: Remove um recurso específico.

## 3. O que é JSON?
**JSON** (JavaScript Object Notation) é um formato leve de troca de dados, fácil de ler tanto por humanos quanto por máquinas. É estruturado basicamente por:

* Objetos: Pares de chave/valor (ex: `"nome": "Carlos"`).

* Arrays (Listas): Coleções ordenadas de valores (ex: `["tecnologia", "esportes"]`).

## 4. Servidor Backend e Web Service
* **Servidor Backend**: Sistema responsável por processar regras de negócio, conectar-se ao banco de dados e fornecer as APIs.

* **Web Service**: Serviço acessível via web que permite a comunicação padronizada entre sistemas heterogêneos usando HTTP.

## 5. Criando uma API com Express.js
O Express.js é um framework minimalista e flexível para Node.js que simplifica a criação de servidores web e rotas em comparação ao Node.js puro.

### Passos básicos para criar uma API com Express:
1. Inicializar o projeto e instalar dependências (`express` e `cors`).

2. Configurar o arquivo principal (ex: `api.js`) definindo as rotas.

3. Utilizar o CORS para permitir que o front-end acesse a API de domínios diferentes.

4. Executar o servidor com o comando `node api.js`.

## 6. Hospedagem com o Render
O Render é uma plataforma de nuvem moderna ideal para simular Web Services e hospedar APIs (Node.js, Python, etc.) com integração contínua via GitHub, oferecendo deploy rápido e planos acessíveis.