# 🏗️ Arquitetura de Software

## 📌 Conceito

Arquitetura de software define a estrutura do sistema, organizando seus componentes e como eles se comunicam.

Ela é responsável por:
- Organização do sistema  
- Distribuição de responsabilidades  
- Comunicação entre partes  

---

## 🎯 Objetivo

Criar sistemas que sejam:

- Escaláveis  
- Manuteníveis  
- Reutilizáveis  
- Eficientes  

---

## 🧩 Componentes principais

| Componente | Função |
|------------|--------|
| Interface (GUI) | Interação com o usuário |
| Lógica de negócio | Regras do sistema |
| Banco de dados | Armazenamento |
| APIs | Comunicação entre sistemas |

---

## 🔄 Arquitetura em camadas

Uma das formas mais comuns de organização é por camadas:

```mermaid
flowchart TD
A[Apresentação (GUI)] --> B[Lógica de Negócio]
B --> C[Persistência (Banco)]
```

### 📌 Camadas

- **Apresentação** → interface com o usuário  
- **Negócio** → regras e processamento  
- **Dados** → acesso ao banco  

---

## ⚙️ Princípios importantes

### 🔹 Separação de responsabilidades
Cada parte do sistema deve ter uma função específica.

### 🔹 Baixo acoplamento
Componentes devem depender pouco uns dos outros.

### 🔹 Alta coesão
Cada módulo deve ter responsabilidades bem definidas.

### 🔹 Reutilização
Componentes podem ser usados em outros sistemas.

---

## 🔗 Comunicação entre camadas

Exemplo conceitual:

```javascript
// Interface chama o backend
fetch('/dados');

// Backend acessa o banco
banco.buscar();
```

📌 A interface nunca acessa diretamente o banco.

---

## 📦 Tipos de arquitetura comuns

| Tipo | Descrição |
|------|----------|
| Monolítica | Sistema em um único bloco |
| Cliente-Servidor | Separação entre frontend e backend |
| Em camadas | Divisão por responsabilidades |
| Microsserviços | Serviços independentes |

---

## 💻 Aplicação na prática

Em sistemas com GUI e banco de dados:

- A interface coleta dados  
- O backend processa  
- O banco armazena  
- O resultado retorna ao usuário  

---

## ⚠️ Problemas sem arquitetura

- Código desorganizado  
- Dificuldade de manutenção  
- Erros frequentes  
- Baixa escalabilidade  

---

## 🔗 Resumo

A arquitetura define como o sistema é estruturado e organizado.

Ela garante:

- Organização  
- Facilidade de manutenção  
- Evolução do sistema  

📌 **Conclusão:**
> Uma boa arquitetura é essencial para construir sistemas eficientes, organizados e escaláveis.