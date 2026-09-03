## 1. Introdução aos Frameworks Front-end
Um *framework front-end* é um conjunto de ferramentas, bibliotecas e regras que padronizam e aceleram o desenvolvimento de interfaces web.

* **Sem framework (Vanilla JS)**: Código manual, repetitivo e difícil de manter.

* **Com framework**: Uso de componentes reutilizáveis, gerenciamento automático de estado e atualizações eficientes.

Diferença entre Biblioteca e Framework
* **Biblioteca**: Você controla o fluxo e decide quando chamar as funções (Ex: React).

* **Framework**: O framework controla o fluxo principal da aplicação e define a estrutura obrigatória (Ex: Angular).

## 2. Principais Tecnologias
**React**
* **O que é**: Biblioteca JavaScript criada pelo Facebook focada na criação de interfaces de usuário dinâmicas.

* **Conceitos Chave**:

    * **Virtual DOM**: Cópia otimizada do DOM real que atualiza apenas o que mudou na tela, garantindo alta performance.

    * **JSX**: Extensão de sintaxe que permite escrever HTML dentro do JavaScript.

    * **Hooks**: Funções especiais como `useState` (para controle de estado) e `useEffect` (para efeitos colaterais e requisições).

**Angular**
* **O que é**: Framework completo e robusto desenvolvido pelo Google, ideal para aplicações de página única (SPA).

* **Características**: Usa TypeScript nativamente, arquitetura organizada em módulos/componentes e uma CLI (Command Line Interface) muito poderosa.

* **Comandos principais**:

    * Instalar CLI: `npm install -g @angular/cli`

    * Criar projeto: `ng new <nome-do-projeto>`

    * Iniciar servidor: `ng serve`

**Vue.js**
* **O que é**: Framework progressivo, flexível e com uma curva de aprendizado suave.

* **Características**: Utiliza arquivos de componente único (.vue), reatividade automática e integração nativa com o empacotador Vite.

* **Comandos principais**:

    * Criar projeto: `npm create vue@latest`

    * Instalar dependências: `npm install`

    * Iniciar servidor: `npm run dev`

**Next.js**
* **O que **é: Framework baseado em React focado no desenvolvimento de aplicações web modernas e _full-stack_.

* **Diferenciais**: Oferece roteamento automático baseado em arquivos, renderização no lado do servidor (SSR) e otimizações avançadas para SEO.

* **Comando para criar**: `npx create-next-app@latest`

## 3. Estrutura Comum de Pastas
A maioria dos projetos modernos possui uma estrutura parecida:

* `node_modules`: Contém todas as dependências e bibliotecas instaladas.

* `public` / `assets`: Arquivos estáticos (imagens, ícones e arquivos globais).

* `src`: Código-fonte da aplicação, onde ficam os componentes e páginas.

* `package.json`: Arquivo que gerencia scripts, dependências e informações do projeto.

## 4. Reutilização de Projetos Prontos
Para economizar tempo, você pode aproveitar códigos e modelos prontos da comunidade através de:

* GitHub: Clonagem de repositórios públicos usando `git clone <url>`.

* Vercel Templates: Busca por modelos de projetos prontos para uso.

* CodeSandbox: Plataforma para encontrar e testar templates online.