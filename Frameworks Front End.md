# Introdução a Frameworks Front-end

**Disciplina:** Desenvolvimento Web  
**Professor:** Prof. Me. Deivison S. Takatu  

---

## 📚 Conteúdo da Aula

- Introdução aos Frameworks Front-end  
- Diferenças entre Framework e Biblioteca  
- Introdução ao React  
- Instalando o Node.js  
- Criando um Projeto React  
- Atividade prática  

---

## 🏗️ O que é um Framework Front-end?

Um **framework front-end** é um conjunto de ferramentas, bibliotecas e convenções que **padroniza o desenvolvimento de interfaces web**, acelerando a criação de aplicações complexas.

### Comparação com desenvolvimento puro (Vanilla JS)
- **Sem framework**: código manual, difícil manutenção, muita repetição.
- **Com framework**: componentes reutilizáveis, gerenciamento de estado, atualizações eficientes.

---

## 🔍 Diferenças entre Framework e Biblioteca

| **Framework** | **Biblioteca** |
|---------------|---------------|
| Controla o fluxo (inversão de controle) | Você decide quando chamar |
| Exige uma estrutura definida | Flexível, sem imposições |
| Ex.: Angular, Vue | Ex.: React, jQuery |

💡 **Exemplo prático:**  
- **Biblioteca (React)**: você chama `ReactDOM.render()` quando quiser.  
- **Framework (Angular)**: decide quando renderizar os componentes.

---

## 🚀 Por que Utilizar um Framework?

- **Produtividade aumentada**: soluções prontas para roteamento, estado e renderização.  
- **Melhores práticas**: código organizado em componentes.  
- **Manutenção facilitada**: Virtual DOM (React), Change Detection (Angular).  
- **Comunidade e suporte**: documentação extensa, plugins e soluções para problemas comuns.

---

## 🛠️ Exemplos de Frameworks

- **React**: biblioteca JavaScript criada pelo Facebook para construção de interfaces de usuário com componentes reutilizáveis.  
- **Angular**: framework completo criado pelo Google para SPAs (Single Page Applications).  
- **Vue.js**: framework progressivo, fácil de adotar conforme o projeto cresce.

[Google Trends](https://trends.google.com.br/)

---

## ✨ Características dos Frameworks Front-end

- **Estrutura de Código Organizada**: separação de HTML, CSS e JS para melhor manutenção e escalabilidade.  
- **Componentização**: componentes independentes e reutilizáveis.  
- **Programação Reativa**: UI atualiza automaticamente com mudanças no estado.  
- **Ferramentas de Build e Bundling**: minificação, transpiração e empacotamento de arquivos.  
- **Sistema de Rotas**: criação de SPAs com navegação suave.  
- **Integração com APIs**: chamadas assíncronas e gerenciamento de estado.  
- **Documentação e Comunidade Ativas**.  
- **Suporte a Testes**: unitários e de integração.  
- **Padrões de Design e Acessibilidade**: componentes pré-construídos que seguem boas práticas.

---

## ⚛️ Introdução ao React

Biblioteca JavaScript desenvolvida pelo **Facebook (2013)** para criação de **web apps dinâmicos**.  
Baseia-se em **componentes reutilizáveis** e no **Virtual DOM**, permitindo aplicações **rápidas e escaláveis**.

### Conceitos Fundamentais
- **Hooks**:
  - `useState`: gerencia o estado de componentes funcionais.
  - `useEffect`: lida com efeitos colaterais (ex.: chamadas de API).
- **JSX**:
  - Usa `{}` para expressões JavaScript.
  - Atributos em camelCase (ex.: `className` em vez de `class`).
  - Tags sempre fechadas (ex.: `<img />`).
- **Gerenciamento de Estado**:
  - Context API: para estados menores.
  - Redux: para estados complexos e globais.

---

## 🌳 DOM x Virtual DOM

- **DOM**: representação em árvore da página web.  
- **Virtual DOM (React)**: cópia otimizada do DOM que permite atualizações mais rápidas, aplicando apenas as diferenças ao DOM real.

---

## 🟢 Instalando o Node.js

[Baixe aqui](https://nodejs.org/en/download)

1. Escolha a versão para seu sistema operacional.  
2. Execute o instalador.  
3. Teste no terminal:
   ```bash
   node --version
   ```
4. **NPM (Node Package Manager)**: gerenciador de pacotes instalado junto com o Node.js.

---

## 📦 NPM (Node Package Manager)

- Gerencia pacotes JavaScript.
- Facilita instalação, atualização e remoção de bibliotecas.
- `package.json`: registra todas as dependências do projeto.
- Comando:
   ```bash
   npm install
   ```
   Instala automaticamente as dependências listadas no `package.json`.

---

## ⚡ Criando um Projeto React

Use o comando oficial:
```bash
npx create-react-app meu-projeto-react
cd meu-projeto-react
npm start
```

### Estrutura do Projeto
- `node_modules`: pacotes instalados.
- `public`: HTML e arquivos estáticos.
- `src`: código React.
- `.gitignore`: arquivos e pastas a serem ignorados pelo Git.
- `package.json` e `package-lock.json`: informações e dependências do projeto.
- `index.js`: ponto de entrada, renderiza o App no DOM.
- `App.js`: componente raiz.
- `App.css`: estilos do App.
- `index.css`: estilos globais.

---

## 🌍 Publicando no GitHub

1. Faça login no GitHub.  
2. Clique em **Publicar Branch** no VS Code.  
3. Escolha repositório público ou privado.  
4. O código ficará acessível no seu perfil do GitHub.

---

## 🧪 Atividade Prática

Crie um **projeto React** com um cabeçalho listando:
- To-Do List
- Contador de Cliques
- Jogo da Velha
- Calculadora
- Buscador de CEP

✅ **Passos**:
1. Desenvolva o projeto e faça commit no **GitHub**.  
2. Faça deploy no **Vercel**, conectando o repositório.  
3. Documente a escolha de estilização e os elementos criados.  
4. Inclua prints, links do repositório no GitHub e do site no Vercel.  
5. Envie o documento final no **CANVAS**.

---

## 📚 Referências

- AGGARWAL, Sanchit et al. *Modern web-development using ReactJS.* IJ of Recent Research Aspects, 2018.  
- BAEHAQI, Ahmad et al. *Front End Learning Management System Development Using The Nextjs Framework.* Jutif, 2023.  
- BANKS, Alex; PORCELLO, Eve. *Learning React: functional web development with React and Redux.* O'Reilly Media, 2017.  
- RAHAT, Rubaya et al. *Developing an effective front-end planning framework for sustainable infrastructure projects.* International Journal of Construction Management, 2023.

---

## 🛡️ Dicas Extras e Melhorias

### Exemplos Visuais
- Inclua capturas de tela do processo de criação do projeto React, estrutura de pastas e resultado dos componentes.
- Documente cada etapa com imagens para facilitar o acompanhamento.

### Glossário Rápido
- **SPA:** Aplicação de página única, navegação sem recarregar a página.
- **JSX:** Sintaxe que mistura JavaScript e HTML no React.
- **Virtual DOM:** Representação otimizada do DOM para atualizações rápidas.
- **Props:** Propriedades passadas para componentes.
- **State:** Estado interno do componente.

### Checklist de Publicação
- [ ] Node.js instalado
- [ ] Projeto React criado
- [ ] Componentes desenvolvidos e testados
- [ ] Código versionado no GitHub
- [ ] Deploy realizado no Vercel
- [ ] Documentação e prints incluídos

### Dicas de Boas Práticas
- Organize componentes em pastas separadas.
- Utilize prop-types para validação de props.
- Mantenha dependências atualizadas.
- Use variáveis sensíveis em arquivos `.env`.

### Segurança e Acessibilidade
- Adicione textos alternativos em imagens.
- Garanta contraste adequado nas cores.
- Teste navegação por teclado e leitores de tela.
- Atualize dependências regularmente.

### Links Úteis
- [Documentação React](https://react.dev/)
- [Documentação Angular](https://angular.io/)
- [Documentação Vue.js](https://vuejs.org/)
- [Guia de Acessibilidade Web](https://www.w3.org/WAI/test-evaluate/)

### Comparativo Prático
- Implemente um componente simples (ex.: contador) em React, Angular e Vue para ilustrar diferenças de sintaxe e estrutura.

---

💡 **Dica Final:** Revise seu projeto em diferentes dispositivos e peça feedback de usuários reais para aprimorar a experiência.
