# APIs e Consumo de Dados na Web (AJAX, Fetch e JSON)

**Disciplina:** Desenvolvimento Web\
**Professor:** Prof. Me. Deivison S. Takatu\
**Contato:** deivison.takatu@facens.br

------------------------------------------------------------------------

## 📚 Conteúdo da Aula

-   Introdução a APIs Web\
-   Comunicação cliente-servidor com dados\
-   JSON como formato de dados\
-   AJAX (Asynchronous JavaScript and XML)\
-   Fetch API\
-   Consumo de APIs REST\
-   Envio de dados para APIs\
-   Atividade prática

------------------------------------------------------------------------

## 🌐 O que são APIs?

**API (Application Programming Interface)** é um conjunto de regras que
permite que **diferentes sistemas se comuniquem entre si**.

Na Web, APIs permitem que aplicações:

-   busquem dados de servidores
-   enviem dados para sistemas externos
-   integrem serviços diferentes

### Exemplos de APIs populares

-   API do **Google Maps**
-   API do **GitHub**
-   API do **OpenWeather**
-   API do **Spotify**

Exemplo de endpoint:

    https://api.github.com/users

Ao acessar esse endereço, o servidor retorna **dados estruturados**,
geralmente em formato **JSON**.

------------------------------------------------------------------------

## 🔄 Comunicação entre Cliente e Servidor

A comunicação entre aplicações web ocorre através de **requisições
HTTP**.

Fluxo básico:

1.  O navegador envia uma requisição para a API\
2.  O servidor processa a solicitação\
3.  O servidor retorna os dados\
4.  O JavaScript manipula os dados na página

Exemplo:

    Cliente → Requisição HTTP → API
    API → Resposta JSON → Cliente

Isso permite que páginas web sejam **dinâmicas e interativas**.

------------------------------------------------------------------------

## 📦 JSON -- JavaScript Object Notation

**JSON** é o formato de dados mais utilizado na comunicação entre
aplicações web.

Características:

-   leve\
-   fácil de ler\
-   fácil de interpretar por máquinas\
-   baseado na sintaxe de objetos JavaScript

### Exemplo de JSON

    {
      "nome": "Maria",
      "idade": 25,
      "cidade": "São Paulo"
    }

### Estrutura do JSON

-   pares **chave : valor**

-   valores podem ser:

-   strings\

-   números\

-   booleanos\

-   arrays\

-   objetos

Exemplo com array:

    {
      "usuarios": [
        {"nome": "Ana"},
        {"nome": "Carlos"},
        {"nome": "João"}
      ]
    }

------------------------------------------------------------------------

## ⚡ AJAX

**AJAX (Asynchronous JavaScript and XML)** é uma técnica que permite
atualizar partes da página **sem recarregar o site inteiro**.

Antes do AJAX:

-   qualquer interação exigia **recarregar a página inteira**

Com AJAX:

-   apenas os **dados necessários são atualizados**

### Benefícios

-   melhor experiência do usuário\
-   maior velocidade\
-   menos consumo de banda\
-   aplicações mais interativas

### Exemplos de uso

-   busca automática do Google\
-   atualização de notificações\
-   carregamento de comentários\
-   atualização de feeds

------------------------------------------------------------------------

## 🧠 Como funciona o AJAX

Fluxo:

1.  Usuário realiza uma ação (ex: clicar botão)\
2.  JavaScript envia requisição HTTP\
3.  Servidor processa a requisição\
4.  Servidor retorna dados (JSON)\
5.  JavaScript atualiza a interface

Fluxo simplificado:

    Usuário → JavaScript → Servidor
    Servidor → JSON → JavaScript → Atualiza página

------------------------------------------------------------------------

## 🚀 Fetch API

A **Fetch API** é a forma moderna de fazer requisições HTTP usando
JavaScript.

Ela substitui métodos antigos como **XMLHttpRequest**.

### Sintaxe básica

``` javascript
fetch("https://api.exemplo.com/dados")
  .then(response => response.json())
  .then(data => {
    console.log(data)
  })
  .catch(error => {
    console.error(error)
  })
```

Explicação:

-   `fetch()` envia a requisição\
-   `response.json()` converte a resposta em JSON\
-   `then()` processa os dados retornados\
-   `catch()` trata erros

------------------------------------------------------------------------

## 📡 Exemplo Prático -- Consumindo uma API

Exemplo usando a API pública **JSONPlaceholder**.

``` javascript
fetch("https://jsonplaceholder.typicode.com/posts")
  .then(response => response.json())
  .then(posts => {
    console.log(posts)
  })
```

A API retorna uma lista de posts em JSON.

Exemplo de resposta:

    {
      "userId": 1,
      "id": 1,
      "title": "titulo do post",
      "body": "conteudo do post"
    }

------------------------------------------------------------------------

## 📤 Enviando dados para uma API

Também é possível **enviar dados para servidores** usando o método
**POST**.

Exemplo com Fetch:

``` javascript
fetch("https://api.exemplo.com/usuarios", {
  method: "POST",
  headers: {
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    nome: "João",
    idade: 30
  })
})
.then(response => response.json())
.then(data => {
  console.log(data)
})
```

Explicação:

-   `method` define o tipo da requisição\
-   `headers` define o formato do dado enviado\
-   `body` contém os dados convertidos para JSON

------------------------------------------------------------------------

## 🌍 APIs REST

Grande parte das APIs modernas seguem o padrão **REST (Representational
State Transfer)**.

Características:

-   comunicação via **HTTP**
-   recursos identificados por **URLs**
-   uso de métodos HTTP
-   respostas geralmente em **JSON**

### Exemplo de endpoints

    GET /usuarios
    GET /usuarios/1
    POST /usuarios
    PUT /usuarios/1
    DELETE /usuarios/1

Cada endpoint representa uma **operação sobre um recurso**.

------------------------------------------------------------------------

## 🧪 Atividade Prática

1.  Crie um arquivo **HTML** com um botão chamado **Carregar Usuários**.

2.  Ao clicar no botão, utilize **Fetch API** para buscar dados da API:

```{=html}
<!-- -->
```
    https://jsonplaceholder.typicode.com/users

3.  Mostre os nomes dos usuários na página.

Exemplo de código:

``` javascript
fetch("https://jsonplaceholder.typicode.com/users")
  .then(response => response.json())
  .then(users => {
    users.forEach(user => {
      console.log(user.name)
    })
  })
```

4.  Envie o resultado com:

-   código HTML
-   código JavaScript
-   print da execução

no **CANVAS**.

------------------------------------------------------------------------

## 📚 Referências

-   FREEMAN, E.; ROBSON, E. *Head First HTML and CSS.* 2. ed. O'Reilly
    Media, 2012.\
-   FREEMAN, E.; ROBSON, E. *Head First Servlets and JSP.* 2.
    ed. O'Reilly Media, 2008.\
-   FLANAGAN, D. *JavaScript: The Definitive Guide.* 7. ed. O'Reilly
    Media, 2020.\
-   MDN Web Docs -- Using Fetch. https://developer.mozilla.org\
-   FIELDING, R. Architectural Styles and the Design of Network-based
    Software Architectures.
