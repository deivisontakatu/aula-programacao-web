# 🧪 Ambientes Virtuais e Gerenciamento de Dependências

O desenvolvimento moderno de aplicações web exige controle rigoroso do ambiente de execução e das dependências utilizadas.

---

## 🎯 Objetivo

Garantir que a aplicação:
- Rode de forma consistente em qualquer ambiente
- Tenha dependências controladas
- Evite conflitos entre bibliotecas
- Seja facilmente reproduzível

---

## 🧱 Problema Sem Isolamento

Sem ambientes virtuais:
- Conflitos de versões de bibliotecas
- Dificuldade de reproduzir ambiente
- Erros em produção diferentes do desenvolvimento

---

## 🧪 Ambientes Virtuais

Ambientes virtuais permitem isolar dependências por projeto.

---

## 🐍 Exemplo com Python (venv)

```bash
python -m venv meu_ambiente
source meu_ambiente/bin/activate
pip install flask
```

---

## 📦 Gerenciamento de Dependências

### 📌 Arquivos comuns:
- `requirements.txt` (Python)
- `package.json` (Node.js)
- `pom.xml` (Java)

---

## 📌 Exemplo (Node.js)

```json
{
  "dependencies": {
    "express": "^4.18.0"
  }
}
```

---

## 🔄 Instalação de Dependências

```bash
npm install
pip install -r requirements.txt
```

---

## 🧊 Containers (Docker)

Containers permitem empacotar aplicação + dependências + ambiente.

---

## 🐳 Exemplo Dockerfile

```dockerfile
FROM node:18
WORKDIR /app
COPY . .
RUN npm install
CMD ["npm", "start"]
```

---

## 🚀 Execução com Docker

```bash
docker build -t minha-app .
docker run -p 3000:3000 minha-app
```

---

## 🧠 Vantagens dos Containers

- Isolamento total
- Portabilidade
- Facilidade de deploy
- Consistência entre ambientes

---

## 🔗 Isolamento de Partes da Aplicação

Aplicações modernas podem ser divididas em:
- Frontend
- Backend
- Banco de dados

Cada parte pode rodar em um container separado.

---

## 📦 Exemplo com Docker Compose

```yaml
version: '3'
services:
  web:
    build: .
    ports:
      - "3000:3000"
  db:
    image: mysql
```

---

## ⚠️ Boas Práticas

- Versionar dependências
- Usar arquivos de lock (`package-lock.json`)
- Evitar instalar dependências globais
- Documentar ambiente

---

## 🔐 Segurança

- Atualizar dependências
- Evitar bibliotecas vulneráveis
- Usar imagens Docker oficiais

---

## 🎯 Conclusão

Ambientes virtuais e containers:
- Garantem isolamento
- Facilitam desenvolvimento e deploy
- Reduzem erros

---

## ✅ Resumo

- Ambientes virtuais isolam dependências  
- Containers isolam aplicações completas  
- Essenciais para desenvolvimento moderno  