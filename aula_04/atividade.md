# 🚀 Top 10 Repositórios no GitHub que Utilizam APIs

Uma seleção de 10 projetos populares e relevantes no GitHub que fazem uso de APIs externas e integrações web, organizados por framework e APIs consumidas.

## 📊 Tabela de Repositórios

| Repositório | Framework utilizado | API's usadas | Como encontrei a API |
| :--- | :--- | :--- | :---|
| [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | LangChain / Pydantic (Python) | OpenAI API, Anthropic Claude API, Google Gemini API, HuggingFace API | Ao verificar o arquivo `./libs/core/Makefile` eu achei os testes de caminhos e funcionamento de API's usadas no projeto |
| [stirling-tools/Stirling-PDF](https://github.com/stirling-tools/Stirling-PDF) | Spring Boot (Java) | PDFbox API, OCR (Tesseract) API | Ao verificar o arquivo `./buildSrc/src/main/groovy/stirling/software/gradle/ModuleLicenseOverrideFilter.groovy` é possível encontrar os imports de algumas APIs logo no começo do código em conjunto de outros imports diversos  |
| [hoppscotch/hoppscotch](https://github.com/hoppscotch/hoppscotch) | Vue.js / Nuxt.js (TypeScript) | WebSockets API, Server-Sent Events (SSE) API, REST/GraphQL APIs | Ao verificar os commits na página inicial do projeto, observei mensagens de commits comentando testes, ajustes ou adiçoes de APIs dentro do projeto |
| [FlowiseAI/Flowise](https://github.com/FlowiseAI/Flowise) | React / Node.js (TypeScript) | OpenAI API, Pinecone API, SerpAPI, Hugging Face API |
| [BloopAI/bloop](https://github.com/BloopAI/bloop) | React (TypeScript) / Rust (Tauri) | OpenAI GPT-4 API, GitHub REST API, Qdrant Vector Search API |
| [activepieces/activepieces](https://github.com/activepieces/activepieces) | Angular / NestJS (TypeScript) | Slack API, Notion API, Google Sheets API, OpenAI API, Webhooks |
| [ChatGPTNextWeb/ChatGPT-Next-Web](https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web) | Next.js / React (TypeScript) | OpenAI Chat Completion API, Google Gemini API, Claude API |
| [dify-ai/dify](https://github.com/dify-ai/dify) | Next.js (Frontend) / Flask (Backend) | OpenAI API, Anthropic API, SERPAPI, DuckDuckGo Search API |
| [postmanlabs/postman-app-support](https://github.com/postmanlabs/postman-app-support) | Electron / React (JavaScript) | Postman Public API, WebSockets API, OAuth 2.0 Auth APIs |
| [spotipy-dev/spotipy](https://github.com/spotipy-dev/spotipy) | Python Client | Spotify Web API |

---

## 📝 Descrição Breve dos Projetos

1. **LangChain**: Framework principal para construção de aplicações impulsionadas por modelos de linguagem (LLMs).
2. **Stirling-PDF**: Ferramenta completa baseada em web para manipulação e processamento de arquivos PDF.
3. **Hoppscotch**: Suíte de desenvolvimento de API open-source, leve e ultra-rápida (alternativa ao Postman).
4. **Flowise**: Interface gráfica drag-and-drop para construir fluxos de trabalho personalizados de LLMs/IA.
5. **Bloop**: Mecanismo de busca de código de alta performance com inteligência artificial integrada.
6. **Activepieces**: Plataforma de automação de fluxo de trabalho open-source (alternativa ao Zapier/Make).
7. **ChatGPT Next Web**: Interface de usuário responsiva e elegante para interagir com modelos da OpenAI, Gemini e Anthropic.
8. **Dify**: Plataforma de desenvolvimento de aplicações LLM que combina orquestração de IA com gerenciamento de APIs.
9. **Postman App Support**: Repositório de suporte e ecossistema do cliente Postman para testes e automação de APIs.
10. **Spotipy**: Biblioteca leve em Python para acesso completo à API Web do Spotify.