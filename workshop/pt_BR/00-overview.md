<!-- l10n-sync: source-file="workshop/00-overview.md" -->
# 🎮 Mona Mayhem — Workshop do GitHub Copilot

---

> **Duração:** ~1 hora  
> **Nível:** Intermediário  
> **Stack:** Astro / Node.js / TypeScript

Crie um aplicativo de comparação de contribuições do GitHub com tema de arcade retrô — **Mona Mayhem** — enquanto aprende todo o espectro de fluxos de trabalho do GitHub Copilot. O workshop oferece **duas trilhas**: uma experiência no VS Code e outra com o GitHub Copilot CLI.

---

## 🎯 Escolha sua trilha

- **Trilha do VS Code** — fique no editor e pratique Chat, Plan Mode, Agent Mode, agentes em segundo plano e o ciclo de revisão integrado.
- **Trilha do CLI** — fique no terminal e pratique `copilot`, contexto com `@file`, `/plan`, edições autônomas, `/fleet`, `/delegate` e `/review`.

Siga a trilha que corresponde ao seu fluxo de trabalho preferido.

---

## 📋 Lista de verificação rápida

Antes de começar, verifique:

- [ ] O GitHub Copilot está habilitado para sua conta
- [ ] Node.js instalado
- [ ] Git instalado e configurado
- [ ] Seu navegador e terminal estão prontos

<!-- track:vscode:start -->
- [ ] VS Code **v1.107+** (sem atualizações pendentes)
- [ ] Sessão iniciada na extensão do **GitHub Copilot**
- [ ] Painel de Chat aberto e Agent pronto
<!-- track:vscode:end -->

<!-- track:cli:start -->
- [ ] GitHub Copilot CLI instalado e disponível como `copilot`
- [ ] Autenticado no CLI com `/login`
- [ ] Familiaridade com comandos slash como `/help`, `/plan` e `/review`
<!-- track:cli:end -->

> 💡 **Dica:** Use o DevContainer para ter um ambiente pré-configurado e começar rapidamente no VS Code.

---

## 🧠 O que você vai aprender

| # | Habilidade | Descrição |
|---|------------|-----------|
| 1 | **Engenharia de contexto** | Ensinar ao Copilot sobre sua base de código com instruções, referências e restrições claras |
| 2 | **Planejar primeiro** | Esboçar a arquitetura antes da implementação |
| 3 | **Implementação agêntica** | Deixar o Copilot realizar tarefas de programação em várias etapas sob sua supervisão |
| 4 | **Design iterativo** | Usar o Copilot para transformar o visual e refinar detalhes da interação |
| 5 | **Fluxos de trabalho paralelos** | Dividir o trabalho entre agentes, sessões ou tarefas delegadas |

<!-- track:vscode:start -->
### Foco em recursos do VS Code

- **Chat + modo Ask** para explorar
- **Plan Mode** para prompts de arquitetura e design
- **Agent Mode** para implementação em vários arquivos
- **Agentes em segundo plano e na nuvem** para polimento em paralelo
<!-- track:vscode:end -->

<!-- track:cli:start -->
### Foco em recursos do Copilot CLI

- **Sessões interativas do CLI** com `copilot`
- **`/plan` e Shift+Tab** para planejamento estruturado
- **Edições autônomas** com aprovações em linha e `/diff`
- **`/fleet`, `/delegate` e `/review`** para paralelismo e etapas de qualidade
<!-- track:cli:end -->

---

## 📚 Partes do laboratório

| Parte | Título | Descrição |
|------|-------|-----------|
| [**01**](01-setup.md) | Configuração e engenharia de contexto | Crie seu repositório, prepare seu ambiente e forneça o contexto adequado ao Copilot |
| [**02**](02-plan-and-scaffold.md) | Planejamento e scaffold | Projete a API e a arquitetura da página antes da implementação |
| [**03**](03-agent-mode.md) | Construção do jogo | Conecte a página de batalha e os gráficos de contribuições com ajuda agêntica |
| [**04**](04-design-vibes.md) | Tematização com design em primeiro lugar | Transforme o scaffold em uma experiência de arcade retrô |
| [**05**](05-polish.md) | Polimento e trabalho paralelo | Use fluxos de trabalho multiagente para melhorar UX, resiliência e qualidade |
| [**06**](06-bonus.md) | Bônus e extensões | Explore funcionalidades abertas, fluxos de compartilhamento e experimentos extras |

---

## 💡 Dicas profissionais

1. **Mantenha o navegador aberto** — acompanhe as atualizações em tempo real enquanto programa.
2. **Faça commits com frequência** — salve pontos de controle estáveis durante as iterações.
3. **Refine o plano antes da implementação** — planos melhores levam a resultados melhores.
4. **Revise as alterações do Copilot** — use a visualização de diferenças ou as ferramentas de revisão do CLI em vez de aceitar tudo sem conferir.

<!-- track:vscode:start -->
5. **Use pontos de controle e Desfazer** no chat se uma iteração sair do rumo.
<!-- track:vscode:end -->

<!-- track:cli:start -->
5. **Use `/session`, `/context` e `/share file`** quando quiser inspecionar ou preservar seu trabalho.
<!-- track:cli:end -->
