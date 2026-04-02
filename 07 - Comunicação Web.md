# 🌐 07 - Comunicação Web

A comunicação web é baseada no modelo **cliente-servidor**, onde um cliente (navegador) envia requisições a um servidor, que processa e retorna respostas.

---

## 🔁 Request e Response

### 📥 Request (Requisição)

É a mensagem enviada pelo cliente ao servidor.

**Características:**

* Utiliza métodos HTTP (GET, POST, PUT, DELETE)
* Pode conter parâmetros (URL ou corpo)
* Inclui cabeçalhos (headers)

**Exemplo:**

* Acessar uma página web
* Enviar dados de formulário

---

### 📤 Response (Resposta)

É a resposta enviada pelo servidor ao cliente.

**Contém:**

* Código de status (200, 404, 500...)
* Headers
* Corpo da resposta (HTML, JSON, etc.)

---

## 🔄 Funcionamento da Comunicação

1. O cliente envia uma requisição (Request)
2. O servidor processa a requisição
3. O servidor retorna uma resposta (Response)

---

## ⚠️ Característica importante

O protocolo HTTP é **stateless (sem estado)**:

* Cada requisição é independente
* O servidor não “lembra” interações anteriores

---

## 🔗 Integração com aplicações

A comunicação web é a base para:

* Sistemas web dinâmicos
* APIs REST
* Aplicações distribuídas

---
