# 📌 Gestão de Backlog aplicada ao Quadro Scrum/Kanban

A qualidade do backlog não depende apenas da descrição dos itens, mas de como eles fluem dentro do **quadro Scrum/Kanban**.

Um bom card deve ser:
- Claro
- Visual
- Objetivo
- Acionável

Isso reduz bloqueios, melhora a comunicação e aumenta a previsibilidade das entregas.

---

# 🧩 Estrutura de um Card no Quadro

## 🟦 Fluxo típico no Kanban/Scrum

- Backlog
- Refinamento
- Pronto para Sprint
- Em Desenvolvimento
- Em Teste
- Concluído (Done)

---

## 🃏 Estrutura do Card

### 🆔 ID + Título
Exemplo:
US-023 | Recuperar senha

Deve ser curto e fácil de identificar no quadro.

---

### 🎯 Descrição (User Story)

Formato padrão:

Como **[tipo de usuário]**  
Quero **[ação]**  
Para **[benefício]**

Exemplo:

Como usuário autenticado  
Quero recuperar minha senha  
Para voltar a acessar minha conta com segurança  

---

### 📌 Tipo (Label)

- Feature
- Bug
- Melhoria
- Técnico

---

### ⚖ Prioridade

- Alta
- Média
- Baixa

ou

- Must / Should / Could / Won’t

---

### 👤 Responsável

Pessoa responsável pelo andamento do card.

---

# ✅ Critérios de Aceite (Checklist)

- [ ] E-mail válido informado
- [ ] Sistema envia e-mail em até 1 minuto
- [ ] Link expira em 24 horas
- [ ] Senha com mínimo de segurança
- [ ] Log da operação registrado

---

# 🔄 Uso do Card no Fluxo

## 🟡 Refinamento

Antes de ir para desenvolvimento, o card deve:

- Estar claro
- Ter critérios definidos
- Estar estimado
- Ser pequeno o suficiente para a sprint

---

## 🟢 Em Desenvolvimento

Adicionar:

- Link do código (PR)
- Comentários técnicos
- Atualizações de progresso

---

## 🔵 Em Teste

Adicionar:

- Casos de teste
- Evidências (prints, logs)

Exemplo:

| ID | Cenário | Resultado Esperado |
|----|--------|------------------|
| CT01 | E-mail válido | Link enviado |
| CT02 | E-mail inválido | Mensagem exibida |

---

## ⚫ Done (Definition of Done)

- [ ] Código finalizado
- [ ] Testes realizados
- [ ] Code review aprovado
- [ ] Deploy realizado
- [ ] Product Owner validou

---

# 🚧 Bloqueios

Se houver impedimentos, marcar o card:

Bloqueado

E descrever o motivo:

- Dependência de API
- Aguardando decisão
- Problema técnico

---

# 📊 Campos Extras

- Dependências
- Riscos
- Anexos (prints, protótipos)
- Links (Figma, API, PR)

---

# 🧠 Checklist antes de mover o card

- Está claro?
- Está pequeno?
- Possui critérios de aceite?
- Está estimado?
- Tem responsável?
- Não possui bloqueios?

---

# 🎯 Benefícios

- Menos retrabalho
- Melhor comunicação
- Fluxo mais eficiente
- Entregas mais previsíveis

---

# 💡 Conclusão

No Scrum/Kanban, um card bem estruturado não é apenas documentação —  
é uma unidade de trabalho que flui pelo sistema.

Quanto mais claro o card, mais rápido ele atravessa o quadro e menor o risco de bloqueios.