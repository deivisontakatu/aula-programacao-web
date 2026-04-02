# 🌐 09 - Consumo de APIs

Este tópico aborda a criação de aplicações web que consomem APIs públicas e privadas, integrando frontend, backend e banco de dados dentro de um projeto estruturado com metodologia ágil.

---

## 🎯 Objetivo

Desenvolver sistemas web capazes de:
- Consumir APIs públicas e privadas
- Integrar dados externos ao sistema
- Utilizar arquitetura moderna (Frontend + Backend)
- Aplicar boas práticas de desenvolvimento ágil

---

## 🔌 O que é uma API?

API (Application Programming Interface) é uma interface que permite a comunicação entre sistemas.

### 📌 Exemplos:
- Clima 🌦️
- CEP 📍
- Cotação de moedas 💱

---

## 🌍 APIs Públicas vs Privadas

| Tipo       | Característica                          |
|------------|----------------------------------------|
| Pública    | Acesso livre ou com chave simples      |
| Privada    | Requer autenticação                    |

---

## 📡 Exemplo de API Pública (ViaCEP)

```javascript
fetch('https://viacep.com.br/ws/01001000/json/')
  .then(res => res.json())
  .then(data => console.log(data));
```

---

## 📦 Consumo no Frontend

```javascript
async function buscarDados() {
  const response = await fetch('/api/dados');
  const data = await response.json();
  console.log(data);
}
```

---

## 🎨 Frontend Responsivo

### Tecnologias:
- HTML5
- CSS3
- JavaScript
- React / Vue

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

---

## 🧠 Backend (Exemplo Node.js)

```javascript
app.get('/api/cep/:cep', async (req, res) => {
  const cep = req.params.cep;
  const response = await fetch(`https://viacep.com.br/ws/${cep}/json/`);
  const data = await response.json();
  res.json(data);
});
```

---

## 🛢️ Persistência de Dados

### Exemplo (SQL):

```sql
CREATE TABLE consultas (
  id INT AUTO_INCREMENT,
  cep VARCHAR(10),
  data_consulta TIMESTAMP,
  PRIMARY KEY(id)
);
```

---

## 🔄 Integração Completa

Fluxo:
1. Frontend envia requisição
2. Backend processa
3. Backend consome API externa
4. Backend acessa banco
5. Retorna resposta

---

## 🧩 Exemplo de Sistema

### Consulta de CEP:
- Entrada do usuário
- Consumo da API
- Exibição dos dados
- Armazenamento no banco

---

## ⚡ Chamadas Assíncronas

```javascript
fetch('/api/usuarios')
  .then(res => res.json())
  .then(data => console.log(data));
```

---

## 🔐 Segurança

- HTTPS
- JWT
- Validação de dados

---

## 🧪 Testes

- Testar APIs
- Validar respostas
- Simular falhas

---

## 🚀 Metodologia Ágil (Scrum)

- Sprint
- Backlog
- Daily

---

## 📋 Exemplo de Backlog

| Tarefa               | Prioridade |
|---------------------|-----------|
| Tela de busca       | Alta      |
| Integração API      | Alta      |
| Banco de dados      | Média     |

---

## 🔄 Ciclo de Desenvolvimento

1. Planejamento  
2. Desenvolvimento  
3. Testes  
4. Entrega  

---

## 🧱 Arquitetura

- Frontend
- Backend
- Banco de Dados

---

## 🧰 Tecnologias

| Camada    | Tecnologias           |
|-----------|----------------------|
| Frontend  | React, HTML, CSS     |
| Backend   | Node.js, Java, PHP   |
| Banco     | MySQL, PostgreSQL    |

---

## 📈 Boas Práticas

- Separação de camadas  
- Código limpo  
- Versionamento (Git)  

---

## 🔗 APIs Privadas

```javascript
fetch('/api/privada', {
  headers: {
    Authorization: 'Bearer TOKEN'
  }
});
```

---

## 📊 Tratamento de Erros

```javascript
try {
  const res = await fetch(url);
} catch (error) {
  console.error(error);
}
```

---

## 🧠 UX

- Loading
- Feedback visual
- Mensagens claras

---

## 📱 Responsividade

- Mobile First
- Media Queries

---

## 🔄 Atualização Dinâmica

- Sem reload
- Uso de JavaScript

---

## 🧪 Validação

- Frontend + Backend
- Sanitização de dados

---

## 📌 Versionamento

- Git
- Controle de versões

---

## 🧾 Documentação

- Swagger
- README

---

## 🎯 Conclusão

Aplicações modernas:
- Integram APIs
- São responsivas
- Usam arquitetura em camadas
- Aplicam métodos ágeis

---

## ✅ Resumo

- APIs conectam sistemas  
- Frontend + Backend + Banco = sistema completo  
- Assíncrono melhora performance  
- Ágil organiza o desenvolvimento  