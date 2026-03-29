# 🌐 Guia Completo — Desenvolvimento Web (Resumo Estruturado)

---

## 📌 1. Navegadores, Arquitetura Web e Escalabilidade

### 🌐 Tecnologias e Padrões de Navegadores

Os navegadores (Chrome, Firefox, Edge) interpretam tecnologias como:

* HTML → estrutura
* CSS → estilo
* JavaScript → comportamento

📌 Padrões:

* DOM (Document Object Model)
* HTTP/HTTPS
* ECMAScript (JS)

---

### 🏗️ Arquitetura de Aplicações Web

* **Arquitetura de dados** → como os dados são armazenados
* **Arquitetura da informação** → organização da interface
* **Arquitetura de sistema** → como tudo se conecta

---

### ⚡ Sistemas Web Escaláveis

* Escalabilidade horizontal (mais servidores)
* Load balancing
* Uso de cache

💡 Exemplo:

```text
Usuário → Load Balancer → Servidores → Banco de Dados
```

---

### 📚 Dica de estudo

👉 Sempre diferencie:

* dado (banco)
* interface (frontend)
* sistema (backend)

---

## 💻 2. Front-end (Cliente)

### 🧠 Programação do lado cliente

* JavaScript
* Frameworks:

  * React
  * Vue
  * Angular

---

### 🎨 Páginas Dinâmicas e Interativas

* Manipulação do DOM
* Eventos (click, input)
* AJAX / Fetch API

---

### 💡 Exemplo

```javascript
fetch('/api/dados')
  .then(res => res.json())
  .then(data => console.log(data));
```

---

### 📚 Dica

👉 Front-end = interação + experiência do usuário

---

## 🖥️ 3. Back-end (Servidor)

### ⚙️ Programação do lado servidor

Linguagens comuns:

* Java (Spring)
* JavaScript (Node.js)
* Python (Django)
* PHP

---

### 🔄 Responsabilidades

* Processar requisições
* Regras de negócio
* Comunicação com banco

---

### 💡 Exemplo

```pseudo
GET /usuarios → retorna lista de usuários
```

---

### 📚 Dica

👉 Back-end = lógica + dados

---

## 🎨 4. Interface, UX/UI e MVC

### 🖼️ GUI (Interface Gráfica)

* Formulários
* Tabelas
* Dashboards

---

### 🧠 UX/UI

* Usabilidade
* Acessibilidade
* Responsividade

---

### 🧩 MVC (Model View Controller)

* **Model** → dados
* **View** → interface
* **Controller** → lógica

---

### 💡 Exemplo

Usuário → Controller → Model → Banco → View

---

### 📚 Dica

👉 MVC = separação de responsabilidades (cai muito em prova)

---

## 🔄 5. Sessões, Cookies e Estado

### 🍪 Cookies

* Armazenados no navegador
* Mantêm estado do usuário

---

### 🔐 Sessões

* Armazenadas no servidor
* Identificadas por ID

---

### 📦 Escopos de memória

* Aplicação → global
* Sessão → usuário
* Request → requisição

---

### 📚 Dica

👉 Cookies (cliente) ≠ Sessão (servidor)

---

## 🗄️ 6. Banco de Dados e Persistência

### 💾 Persistência de Dados

* Armazenamento permanente (BD)

---

### 🔗 ORM (Object Relational Mapping)

* Mapeia objetos → tabelas

Exemplos:

* Hibernate (Java)
* Sequelize (Node.js)

---

### ⚡ Chamadas assíncronas

* AJAX / APIs
* Atualização sem recarregar página

---

### 📚 Dica

👉 Persistência = salvar dados corretamente

---

## 🔌 7. APIs e Projetos Web

### 🌐 Consumo de APIs

* APIs públicas (ex: clima, mapas)
* APIs privadas

---

### 💡 Exemplo

```javascript
fetch('https://api.openweathermap.org')
```

---

### 🛠️ Projeto Web Completo

Inclui:

* Front-end
* Back-end
* Banco de dados
* APIs
* Layout responsivo

---

### ⚙️ Metodologias ágeis

* Scrum
* Kanban

---

### 📚 Dica

👉 Projeto completo = integração de tudo

---

## 🐳 8. Ambientes, Containers e Build

### 🧪 Ambientes virtuais

* Isolamento de dependências

---

### 🐳 Containers (Docker)

* Empacotamento da aplicação
* Ambiente consistente

---

### 🔄 Automação

* Build tools
* Scripts

---

### 📚 Dica

👉 Docker = padrão atual de mercado

---

## ☁️ 9. Hospedagem e Servidores

### 🌐 Hospedagem

* Cloud (AWS, Azure)
* VPS
* Shared hosting

---

### 🖥️ Servidores Web

* Apache
* Nginx

---

### 📚 Dica

👉 Servidor impacta desempenho e escalabilidade

---

## 🔄 10. Versionamento, CI/CD e Testes

### 🧾 Versionamento

* Git

---

### 🔄 CI/CD

* Integração contínua
* Entrega contínua

---

### 🧪 TDD (Test Driven Development)

* Testes antes do código

---

### 📚 Dica

👉 CI/CD = automação do desenvolvimento

---

## 🔐 11. Segurança em Aplicações Web

### 🔒 Segurança

* HTTPS
* Criptografia
* Proteção contra ataques

---

### ⚠️ Riscos comuns

* SQL Injection
* XSS
* CSRF

---

### 📚 Dica

👉 Segurança cai MUITO em prova

---

## 🎯 Síntese Final

* Desenvolvimento web envolve front-end, back-end e banco
* APIs conectam sistemas
* Containers e cloud facilitam deploy
* CI/CD automatiza processos
* Segurança é essencial em todas as camadas

---
