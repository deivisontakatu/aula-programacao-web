# Introdução ao Versionamento e Deploy

---

## 📚 Conteúdo da Aula

- Introdução ao Versionamento e Backup  
- Versionamento Semântico (SemVer)  
- Git e Controle de Versão  
- Branches e Merge no Git  
- Deploy e Hospedagem  
- Atividade prática  

---

## 🗂️ Versionamento x Backup em CMS e Website Builders

- **Versionamento**: permite controlar alterações no código, saber quem fez, quando e o que mudou.  
- **Backup**: garante cópia de segurança do conteúdo do site.

### CMS (ex.: WordPress)
- Controle de versões via **plugins**.
- **Backup manual**: feito pelo usuário (risco de falhas e esquecimento).
- **Backup automático**: via plugins ou serviços de hospedagem (mais confiável, mas pode ter custos).

---

## 🏷️ Introdução ao Versionamento

Versionamento é o processo de atribuir um **identificador único** a cada versão de um documento ou software.  
Exemplo:
- Numérico: `v1.0`, `v1.1`, `v2.0`
- Baseado em datas: `2023-10-01`

✅ **Benefícios**:
- Rastreabilidade e auditoria de mudanças.  
- Organização, colaboração e recuperação de versões anteriores.

---

## 🔢 Versionamento Semântico (SemVer)

Padrão: **MAJOR.MINOR.PATCH** (ex.: `2.1.3`)

- **MAJOR**: mudanças incompatíveis (ex.: `2.0.0`)  
- **MINOR**: novas funcionalidades compatíveis (ex.: `1.1.0`)  
- **PATCH**: correções de bugs (ex.: `1.1.1`)

### Exemplo
- `1.0.0` → Primeira versão estável  
- `1.1.0` → Nova funcionalidade compatível  
- `1.1.1` → Correção de bug  
- `2.0.0` → Mudança incompatível

✅ **Vantagens**:
- Clareza para desenvolvedores e usuários.  
- Facilidade na gestão de dependências e manutenção do software.

---

## 🛠️ Exemplos de Alterações no Código

- **Bug Fix**: correção de erros.
- **New Feature**: adição de nova funcionalidade.
- **Feature Enhancement**: melhorias em funcionalidades existentes.
- **Refactoring**: reorganização do código.
- **Performance**: otimizações de velocidade.
- **Security Patch**: correções de vulnerabilidades.
- **Dependency Update**: atualização de bibliotecas/frameworks.
- **Adding Tests**: inclusão de testes automatizados.

---

## 💡 Importância do Versionamento

- **Controle de Mudanças**: múltiplos colaboradores sem perda de trabalho.  
- **Histórico e Auditabilidade**: registro de todas as modificações.  
- **Recuperação de Dados**: reverter versões em caso de erro.  
- **Colaboração Eficiente**: branches para testar mudanças isoladas.  
- **Qualidade**: testar versões antes da publicação.  
- **Integração com Ferramentas**: gestão de projetos e integração contínua.

---

## 🐙 Git – Sistema de Controle de Versão

- **Git**: sistema instalado localmente e usado via linha de comando.
- Sincroniza com **repositórios online** (GitHub, GitLab etc.).
- Registra versões, acompanha mudanças e permite restaurar versões anteriores.

[GitHub – Linus Torvalds](https://github.com/torvalds)

---

## ⚙️ Instalação do Git

1. Baixe em [git-scm.com](https://git-scm.com/downloads).  
2. Instale seguindo “Next > Install”.  
3. Teste no terminal: `git --version`.  
4. Configure usuário:
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu@email.com"
   ```

---

## 🌿 Branches e Merge

- **Branch**: ramificação para desenvolver sem impactar a versão principal.
  - `main`/`master`: versão estável.
  - `develop`: integra novas funcionalidades antes de ir para `main`.
  - `feature`: desenvolvimento de uma nova funcionalidade.
- **Merge**: une mudanças de uma branch em outra.
- **Conflitos**: quando duas branches alteram a mesma parte do código.

✅ **Boas Práticas**:
- Commits pequenos e frequentes.  
- Mensagens de commit claras.  
- Testes automatizados antes do merge.

---

## 🏷️ Tags no Git

- Marcadores para identificar pontos específicos no histórico (ex.: `v1.0`).
- **Tipos**:
  - *Lightweight*: apenas um nome para um commit.
  - *Annotated*: inclui data, autor e mensagem.

Comandos principais:
```bash
git tag 1.0.0
git push origin 1.0.0
```

---

## ☁️ Deploy – Colocando em Produção

Deploy é o processo de **publicar uma aplicação** para torná-la acessível a usuários.

### Etapas comuns:
- Compilação do código.
- Configuração do ambiente.
- Testes finais.
- Publicação.

---

## 🚀 Vercel para Deploy e Hospedagem

- **Hospedagem simplificada** para sites estáticos e aplicações modernas.
- **Integração com Git**: deploy automático a cada push.
- **Frameworks suportados**: Next.js, React, Vue, Nuxt.js, etc.
- **Deploys instantâneos** com rollback.
- **Serverless Functions**: backend sem servidor.
- **CDN Global**: baixa latência e alta performance.

[vercel.com](https://vercel.com/)

---

## 🧪 Atividade Prática

1. Crie um repositório no **GitHub** com uma página HTML simples.  
2. Versione o código com **Git**, usando **tags** para marcar versões estáveis.  
3. Realize o **deploy no Vercel**, conectando o repositório.  
4. Documente o processo com prints e links (GitHub e Vercel).  
5. Envie o documento final no **CANVAS**.

---

## 📚 Referências

- TATE, B.; LOUTH, F. *Version Control with Git.* O'Reilly Media, 2022.  
- HODSON, R. *Continuous Delivery and DevOps: A Quickstart Guide.* 2. ed. Packt Publishing, 2023.  
- NEWMAN, S. *Building Microservices.* 2. ed. O'Reilly Media, 2021.  
- FREEMAN, E.; ROBSON, E. *Modern Web Development: Building and Deploying with Modern Tools.* O'Reilly Media, 2022.

---

## 🛡️ Dicas Extras e Melhorias

### Exemplos Práticos
- Inclua capturas de tela dos comandos Git, criação de branches, tags e do processo de deploy no Vercel.
- Documente cada etapa com imagens para facilitar o acompanhamento.

### Glossário Rápido
- **Commit:** Registro de alteração no repositório.
- **Branch:** Ramificação do projeto para desenvolvimento paralelo.
- **Merge:** Junção de alterações de diferentes branches.
- **Tag:** Marcador de versão específica.
- **Deploy:** Publicação do projeto para acesso público.

### Checklist de Publicação
- [ ] Repositório criado no GitHub
- [ ] Código versionado com commits claros
- [ ] Branches utilizadas para desenvolvimento
- [ ] Tags aplicadas para versões estáveis
- [ ] Deploy realizado no Vercel
- [ ] Documentação do processo concluída
- [ ] Backup do projeto realizado

### Segurança e Boas Práticas
- Use autenticação em dois fatores no GitHub.
- Mantenha dependências sempre atualizadas.
- Revise permissões de acesso ao repositório.
- Teste o site após cada deploy.

### Links Úteis
- [Guia Oficial do Git](https://git-scm.com/doc)
- [Documentação Vercel](https://vercel.com/docs)
- [Guia de Versionamento Semântico](https://semver.org/lang/pt-BR/)

---

💡 **Dica Final:** Revise o histórico do Git antes de cada deploy e utilize tags para facilitar rollback em caso de problemas.
