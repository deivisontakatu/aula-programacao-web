# Introdução ao Protocolo Web (HTTP / HTTPS)

**Disciplina:** Desenvolvimento Web  
**Professor:** Prof. Me. Deivison S. Takatu  

---

## 📚 Conteúdo da Aula

- Introdução ao Protocolo HTTP  
- Estrutura de requisição e resposta (Request/Response)  
- Métodos HTTP  
- Códigos de Status  
- Cookies e Sessões  
- HTTPS e segurança na Web  
- Atividade prática  

---

## 🌐 O que é HTTP?

**HTTP (HyperText Transfer Protocol)** é o protocolo utilizado para comunicação entre **clientes (navegadores)** e **servidores web**.

Ele define **como as mensagens são enviadas e recebidas na Web**.

Exemplo de fluxo:

Cliente (Browser) → Requisição HTTP → Servidor  
Servidor → Resposta HTTP → Cliente

Quando você acessa um site como:

https://www.google.com

O navegador envia uma **requisição HTTP/HTTPS** ao servidor solicitando a página.

---

## 📡 Modelo Cliente-Servidor

A comunicação web segue o modelo **Cliente–Servidor**.

- **Cliente**: navegador ou aplicação que solicita recursos.
- **Servidor**: sistema que processa a solicitação e retorna uma resposta.

### Exemplo

1. Usuário digita um endereço no navegador  
2. O navegador envia uma requisição HTTP  
3. O servidor processa a requisição  
4. O servidor envia uma resposta (HTML, CSS, JS etc.)

---

## 📦 Estrutura de uma Requisição HTTP

Uma requisição HTTP contém:

- **Método**
- **URL**
- **Headers**
- **Body (opcional)**

### Exemplo de Requisição

GET /index.html HTTP/1.1  
Host: www.exemplo.com  
User-Agent: Mozilla/5.0  
Accept: text/html  

Significado:

- `GET` → método da requisição  
- `/index.html` → recurso solicitado  
- `Host` → domínio do servidor  

---

## 📤 Estrutura de uma Resposta HTTP

A resposta enviada pelo servidor possui:

- **Status Code**
- **Headers**
- **Body**

### Exemplo

HTTP/1.1 200 OK  
Content-Type: text/html  
Content-Length: 1256  

Depois dos headers, o servidor envia o **conteúdo da página (HTML)**.

---

## 🔧 Métodos HTTP

Os métodos HTTP indicam **a ação que o cliente deseja realizar**.

| Método | Função |
|------|------|
| GET | Solicitar um recurso |
| POST | Enviar dados ao servidor |
| PUT | Atualizar um recurso |
| DELETE | Remover um recurso |
| PATCH | Atualizar parcialmente |

### Exemplo

Buscar dados:

GET /usuarios

Criar usuário:

POST /usuarios

---

## 📊 Códigos de Status HTTP

Os servidores retornam **códigos de status** para indicar o resultado da requisição.

### 1xx – Informacional
- 100 Continue

### 2xx – Sucesso
- 200 OK
- 201 Created

### 3xx – Redirecionamento
- 301 Moved Permanently
- 302 Found

### 4xx – Erro do Cliente
- 400 Bad Request
- 401 Unauthorized
- 404 Not Found

### 5xx – Erro do Servidor
- 500 Internal Server Error
- 503 Service Unavailable

---

## 🍪 Cookies

**Cookies** são pequenos arquivos armazenados no navegador do usuário.

Eles são usados para:

- manter login
- guardar preferências
- rastrear sessões

### Exemplo de uso

Quando um usuário faz login, o servidor envia um cookie:

Set-Cookie: session_id=123456

Esse cookie será enviado em futuras requisições.

---

## 🔑 Sessões

Sessões permitem que o servidor **mantenha estado entre várias requisições**.

Fluxo comum:

1. Usuário faz login  
2. Servidor cria uma sessão  
3. Servidor envia um cookie de sessão  
4. Navegador envia o cookie em cada requisição  

Isso permite manter o usuário autenticado.

---

## 🔒 HTTPS – HTTP Seguro

**HTTPS (HyperText Transfer Protocol Secure)** é a versão segura do HTTP.

Ele utiliza **criptografia TLS/SSL** para proteger a comunicação.

### Benefícios

- Proteção contra interceptação de dados
- Segurança de informações sensíveis
- Autenticação do servidor
- Integridade dos dados

Exemplo:

http://exemplo.com

versus

https://exemplo.com

O navegador mostra um **cadeado 🔒** quando a conexão é segura.

---

## 🛡️ Como funciona o HTTPS

1. O navegador solicita conexão segura  
2. O servidor envia um **certificado digital**  
3. O navegador valida o certificado  
4. É criada uma **chave criptográfica**  
5. A comunicação passa a ser criptografada  

---

## 🧪 Atividade Prática

1. Abra o navegador e pressione **F12** para abrir as **Ferramentas do Desenvolvedor**.  
2. Acesse a aba **Network**.  
3. Recarregue um site (ex.: https://example.com).  
4. Observe:

- método HTTP utilizado  
- status code retornado  
- headers da requisição  
- headers da resposta  

5. Escolha uma requisição e identifique:

- método HTTP  
- código de status  
- tipo de conteúdo retornado  

6. Faça um print da análise e envie no **CANVAS**.

---

## 📚 Referências

- FIELDING, R.; RESCHKE, J. *Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content.* IETF, 2014.  
- FREEMAN, E.; ROBSON, E. *Head First HTML and CSS.* 2. ed. O'Reilly Media, 2012.  
- FREEMAN, E.; ROBSON, E. *Head First Servlets and JSP.* 2. ed. O'Reilly Media, 2008.  
- MDN Web Docs. *HTTP Overview.* https://developer.mozilla.org  

---

## 🛠️ Dicas Extras e Melhorias

### Exemplos Práticos

- Utilize o **DevTools do navegador** para analisar requisições HTTP.  
- Teste APIs com ferramentas como **Postman** ou **Insomnia**.

### Glossário Rápido

- **HTTP:** protocolo de comunicação da Web.  
- **Request:** solicitação enviada pelo cliente.  
- **Response:** resposta enviada pelo servidor.  
- **Header:** metadados da comunicação.  
- **Cookie:** pequeno dado armazenado no navegador.  
- **HTTPS:** versão segura do HTTP.

### Checklist de Aprendizagem

- [ ] Entender o modelo cliente-servidor  
- [ ] Compreender estrutura de requisições HTTP  
- [ ] Identificar métodos HTTP  
- [ ] Interpretar códigos de status  
- [ ] Entender o papel de cookies e sessões  
- [ ] Diferenciar HTTP de HTTPS  

---

💡 **Dica Final:** utilize sempre **HTTPS** em aplicações web modernas para proteger dados dos usuários e garantir comunicação segura entre cliente e servidor.