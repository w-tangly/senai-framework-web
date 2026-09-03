## 1. Versionamento vs. Backup
* **Versionamento**: Registra o histórico de cada alteração. Identifica quem, quando e por quê mudou. Permite colaboração simultânea e reversão granular.
* **Backup**: Cria uma cópia pontual do estado atual. Não possui rastreio de autoria. Utiliza arquivo único sem suporte a merge e permite apenas restauração total.
* **Benefícios principais**: 
  * Trabalho simultâneo entre vários desenvolvedores.
  * Menos retrabalho com identificação precoce de conflitos.
  * Auditoria e rastreabilidade completa das modificações.
  * Recuperação segura de versões anteriores.

## 2. Versionamento Semântico (SemVer)
O sistema segue o padrão **MAJOR.MINOR.PATCH** (ex: `2.1.3`):
* **MAJOR**: Indica mudanças incompatíveis com versões anteriores.
* **MINOR**: Adiciona novas funcionalidades compatíveis com versões anteriores.
* **PATCH**: Realiza correção de bugs sem alterar a API.

## 3. Ferramentas Essenciais
* **VS Code (IDE)**: Ferramenta que reúne recursos para desenvolver, testar, executar e depurar software.
* **Git**: Sistema de controle de versão de arquivos instalado via linha de comando. Sincroniza com repositórios online e registra versões do projeto.
* **Tags no Git**: Marcadores usados para identificar pontos específicos no histórico do projeto, como versões estáveis. Podem ser leves ou anotadas.
* **Boas Práticas**: Realizar commits pequenos e frequentes, criar mensagens claras, usar branches para novas funcionalidades e aplicar testes automatizados.

## 4. Node.js e NPM
* **Node.js**: Ambiente de execução JavaScript no servidor. Unifica a linguagem utilizada no front-end e no back-end.
* **NPM (Node Package Manager)**: Gerenciador de pacotes do Node.js instalado automaticamente. Utiliza o arquivo `package.json` para gerenciar dependências do projeto de forma automatizada.

## 5. Criação de Projetos React
* **Comando inicial**: Utiliza-se `npx create-react-app <nome>` para gerar a estrutura padrão do projeto.
* **Fluxo básico de uso**: Navegar até a pasta com `cd`, abrir o VS Code com `code .` e iniciar o servidor local com `npm start`.
* **Estrutura de pastas**:
  * `node_modules`: Contém os pacotes e bibliotecas instaladas.
  * `public`: Contém arquivos HTML, JSON e imagens.
  * `src`: Contém os arquivos JavaScript do React, como `App.js` e `index.js`.
  * Arquivos de configuração como `.gitignore` e `package.json`.

## 6. Deploy e Hospedagem com Vercel
* **Definição de Deploy**: Processo de colocar uma aplicação em produção para torná-la acessível aos usuários finais.
* **Vercel**: Plataforma focada em hospedagem simplificada de aplicações modernas. Oferece integração fácil com o Git para deploys automáticos a cada push, suporte a frameworks modernos, CDN global e funções serverless.