# 🔐 Segurança em Aplicações Web

A segurança em aplicações web envolve a proteção de dados, sistemas e usuários contra acessos não autorizados, ataques e vulnerabilidades.

---

## 🎯 Objetivo

Garantir que a aplicação:
- Proteja dados sensíveis
- Evite ataques comuns
- Mantenha integridade e confidencialidade
- Seja confiável para usuários

---

## 🧱 Níveis de Segurança

A segurança deve ser aplicada em múltiplos níveis:

- Código
- Comunicação
- Arquitetura
- Banco de dados
- Infraestrutura

---

## 🔒 Segurança no Código

### 📌 Embaralhamento de Código (Obfuscation)

Técnica que dificulta a leitura do código fonte.

```javascript
function a(b){return b*2}
```

### 🎯 Objetivo:
- Proteger lógica da aplicação
- Dificultar engenharia reversa

---

## 🌐 Comunicação Segura

### 🔐 HTTPS (SSL/TLS)

- Criptografa dados entre cliente e servidor
- Evita interceptação (MITM)

```text
http:// → inseguro
https:// → seguro
```

---

## 🔑 Autenticação e Autorização

- Login e senha
- Tokens (JWT)
- Controle de acesso por perfil

---

## 🧱 Arquitetura Segura

### Boas práticas:
- Separação de camadas (Frontend, Backend, DB)
- Validação de dados
- Uso de APIs seguras

---

## 🔐 Criptografia

### 📌 Dados em trânsito
- HTTPS

### 📌 Dados em repouso
- Criptografia no banco

---

## 🛢️ Segurança no Banco de Dados

### ⚠️ SQL Injection

```sql
SELECT * FROM usuarios WHERE login = 'admin' --'
```

### ✅ Prevenção:
- Prepared statements
- ORM

---

## 🔐 Armazenamento de Senhas

Nunca armazenar senhas em texto puro.

```text
Senha → Hash (bcrypt)
```

---

## 🔒 Configurações Seguras

- Variáveis de ambiente (.env)
- Não expor credenciais
- Criptografar arquivos sensíveis

---

## 🧊 Segurança com Containers

- Isolamento de serviços
- Limitação de acesso
- Atualização de imagens

---

## ⚠️ Principais Vulnerabilidades

- XSS (Cross-Site Scripting)
- CSRF (Cross-Site Request Forgery)
- SQL Injection
- Falhas de autenticação

---

## 🛡️ Boas Práticas

- Validar entradas
- Sanitizar dados
- Usar HTTPS
- Atualizar dependências
- Monitorar logs

---

## 📊 Monitoramento

- Logs de acesso
- Alertas de segurança
- Ferramentas SIEM

---

## 🎯 Conclusão

Segurança deve ser aplicada em todas as camadas da aplicação.

---

## ✅ Resumo

- Segurança é multicamada  
- Criptografia protege dados  
- HTTPS é obrigatório  
- Boas práticas evitam vulnerabilidades  