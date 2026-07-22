# M5 · Liderança na Era da IA — o ecossistema Claude aplicado

**Trilha 2 · Módulo 5 de 6 · Ecossistema Claude**

> Você conheceu o chat. Agora entra na caixa de ferramentas completa: onde delegar, onde pensar junto, onde deixar o Claude executar tarefa longa. Depois, 6 exercícios prontos pra rodar na sua rotina.

Este é um módulo **demonstrativo e prático**. Cada participante baixa um artefato real, cola no Claude e vê o output ao vivo. A página HTML (`index.html`) traz o mesmo conteúdo em formato interativo (tabs por estação + grid de casos); este `.md` é a fonte canônica de leitura.

---

## Primeiro · o mapa do ecossistema — 5 estações

A ordem é a progressão natural de uso: começa no chat, evolui pra delegação, aprende a organizar, materializa e por fim personaliza.

```
CHAT → COWORK → PROJECTS → ARTIFACTS → PERSONALIZAÇÃO
```

### 1. Chat (Claude.ai) — o ponto de partida

**O que é:** a interface conversacional em `claude.ai` e no app desktop. Uma pergunta, uma resposta, você refina no próximo turno. Feito pra trocas curtas e pensamento rápido.

**Mental model:** Chat é onde você pensa **com** o Claude. Não é onde você delega.

- **Use quando:** precisa de resposta rápida (1-3 turnos); está iterando/pensando em voz alta; a tarefa termina na resposta; vai copiar o output pra outro lugar.
- **Não use quando:** precisa que o Claude modifique arquivos na sua máquina; envolve mais de 20 arquivos ou >30MB; quer entregável salvo em pasta; fluxo tem múltiplos passos automáticos.
- **Exemplo Mallory:** "Me ajuda a redigir a fala de abertura do DDS de amanhã sobre acidente com prensa." → 3 versões de texto. Termina na resposta, sem arquivo, sem sistema externo.

> *"Chat é onde você pensa com o Claude. Cowork é onde você delega ao Claude."* — What is Claude Cowork · Anthropic Academy

### 2. Cowork — Claude que trabalha por você

**O que é:** modo do app desktop onde o Claude opera direto nos seus arquivos e apps conectados. Planeja, executa passo a passo, usa as ferramentas e salva o entregável de volta na pasta. Não é chat mais esperto — é forma diferente de trabalhar.

**Mental model:** Cowork é sobre delegar arco de trabalho inteiro, não conversar mais esperto.

- **Use quando:** tarefa tem múltiplos passos e demora minutos-horas; envolve arquivos locais editados de verdade; puxa dados de várias fontes (Slack, Drive, planilhas); termina em entregável real (deck, xlsx, docx).
- **Não use quando:** só quer pensar em voz alta; é 1 pergunta/1 resposta; está com dado sensível não anonimizado (revisar Checklist do M4); não sabe o resultado que quer.
- **Exemplo Mallory:** "Olha os 5 PDFs de cotação na pasta Compras, compara preço e SLA, e devolve uma planilha com ranking." → xlsx salvo com ranking. Chat não escreve no disco.

> *"Cowork é sobre delegar — não é conversar de forma mais esperta."* — What is Claude Cowork · Anthropic Academy

### 3. Projects — contexto que persiste

**O que é:** workspace persistente no Claude.ai onde você fixa conhecimento estático (arquivos, instruções, contexto) que fica sempre carregado em toda conversa iniciada ali. É a memória compartilhada de um fluxo recorrente.

**Mental model:** Project é a pasta suspensa do arquivo permanente — tudo que está dentro entra em toda conversa que nascer ali.

- **Use quando:** tem 5-15 documentos-âncora que precisam estar em toda conversa do tema; cliente/produto/linha que você conversa toda semana; time pergunta contra o mesmo conjunto de docs; contexto muda pouco mas é sempre relevante.
- **Não use quando:** o conhecimento muda a cada tarefa (vira ruído); precisa de ação em sistema externo (Project não age); procedimento acionado só quando relevante — isso é Skill.
- **Exemplo Mallory:** Gestor de Qualidade cria Project "Auditoria ISO 9001" com o manual, últimos relatórios e plano de ação. Toda conversa sobre auditoria já herda o contexto.

> *"Skills são mais úteis que projects — no instante em que alguém pergunta sobre aquilo, o Claude vai direto no arquivo certo."* — Jan · 9x Claude Cowork Workshop

### 4. Artifacts — entregas prontas em janela própria

**O que é:** deliverables interativos gerados pelo Claude dentro de uma conversa de Chat — documentos, dashboards, mini-apps, visualizações, código — que aparecem num painel próprio e podem ser publicados como link compartilhável.

**Mental model:** Artifact é a peça viva que o Claude produz enquanto conversa com você. Não é texto — é uma coisa que roda.

- **Use quando:** precisa mostrar número/tendência visualmente pro time; quer transformar CSV numa página compartilhável em minutos; está prototipando (fluxo, calculadora, checklist); calculadora simples que abre no celular.
- **Não use quando:** documento formatado pra arquivo oficial (contrato, ata assinada); precisa integrar em sistema corporativo real; dado sensível (link pode ficar público); depende de arquivos reais recorrentes na máquina (aí é Cowork).
- **Exemplo Mallory:** Cola CSV de apontamento: "Vira isso num dashboard que eu compartilho com os 4 coordenadores hoje à tarde." → dashboard publicável, link no grupo.

> *"No fundo, artifacts são projetos compartilháveis que você cria com outras pessoas."* — Alex · 9x Claude Cowork Workshop

### 5. Personalização — Skills, Connectors, Plugins

Três camadas complementares:

- **Skill** — procedimento reusável. Pasta com `SKILL.md`, carregada só quando a descrição bate com a tarefa. Sem auth externa. *Ensina como fazer.*
- **Connector** — acesso a sistema. Ligação OAuth/MCP com Gmail, Drive, Slack, CRM. Herda suas permissões. *Dá acesso a dado/ação.*
- **Plugin** — pacote de função. Agrupa N Skills + N Connectors + sub-agentes de uma função (Finance, Product, RH). *Empacota tudo.*

**Mental model:** Skill é a receita. Connector é o cano até o ingrediente. Plugin é a cesta pronta com receita + ingredientes de uma função inteira.

#### Skill — por dentro
- **Divulgação progressiva:** o Claude lê a `description` de cada skill instalada e só puxa as que batem com a tarefa. Contexto enxuto, desempenho não degrada mesmo com dezenas de skills.
- **Anatomia mínima:** uma pasta com `SKILL.md` (frontmatter `name` + `description` + corpo com instruções em português comum). Scripts em subpastas quando envolve arquivo (Excel, PDF).
- **4 origens:** (1) Anthropic nativas (Excel, Word, PPT, PDF, já instaladas); (2) personalizadas (você/seu time escreve); (3) provisionadas pela organização (Team/Enterprise); (4) de parceiros (Notion, Figma, Atlassian).
- **Padrão aberto:** `agentskills.io` — uma skill escrita hoje pro Claude roda em outros agentes que adotem o padrão. Sem lock-in.

#### Connector — por dentro
- **Herança de permissões (a regra central):** o Claude só enxerga o que *você* enxerga no sistema conectado. Nenhum privilégio é elevado; a ação fica no seu nome, auditoria funciona igual.
- **Duas formas de criar:** Diretório (OAuth, 2 cliques — Google, Microsoft, Slack, Notion) ou MCP remoto (servidor próprio da empresa, URL + client ID/secret).
- **Controles pouco conhecidos:** Modo Sob Demanda (só ativa o connector quando a tarefa exige — recomendado com 10+ instalados); Restrição por ação (leitura sim, escrita não — Team/Enterprise); selo "Interativo" (renderiza UI ao vivo no chat).

#### Plugin — por dentro
- **Dois sabores:** Cowork/Claude.ai (biblioteca por área — Design, PM, Finance, Productivity, Sales, Legal, Marketing, RH, Engineering, Operations; um clique instala) e Claude Code/Agent SDK (skills + agents + hooks + MCP + LSP, via git marketplace).
- **Namespace como pista visual:** em `finance:variance-analysis`, o antes-dos-dois-pontos é o plugin, o depois é a skill dele.
- **Instalar peça, não pacote:** dá pra pegar só a skill que interessa; plugin inteiro atualiza junto (menos manutenção manual).
- **Onde achar os oficiais:** `github.com/anthropics/knowledge-work-plugins` (gratuito, mantido pela Anthropic).

#### Comparar e escolher

| Aspecto | Skill | Connector | Plugin |
|---|---|---|---|
| Resolve | Procedimento reusável | Acesso a sistema externo | Função inteira pronta |
| Auth externa | Não precisa | Sim (OAuth ou MCP) | Pode ter (via connectors internos) |
| Unidade | Pasta com `SKILL.md` | Integração configurada | Pacote (skills + connectors + agents) |
| Onde funciona | Claude.ai + Cowork | Claude.ai + Cowork | Ambos (Cowork ou Claude Code) |
| Quem cria | Você, empresa, ou Anthropic | Você, empresa, ou Anthropic | Você, empresa, ou Anthropic |
| Editável | Sim — edita a pasta | Sim — reconfigura | Sim — pelas skills internas |

Guia rápido:
- *"Sempre que eu pedir X, quero resposta no formato Y."* → **Skill**
- *"Preciso que o Claude leia ou faça algo num sistema real da empresa."* → **Connector**
- *"Quero uma função inteira pronta pra rodar amanhã, sem configurar."* → **Plugin**

#### Plugins prontos da Anthropic

Coleção oficial pública, gratuita, mantida pelo time. Se você já usou Claude for Finance ou Claude for Design, já usou plugin oficial — o namespace na assinatura (`finance:`, `design:`) é a pista.

- `product-management:write-spec` — transforma ideia solta em spec estruturada de produto
- `finance:variance-analysis` — decompõe variação orçamentária em drivers com narrativa
- `design:user-research` — planeja, conduz e sintetiza pesquisa com usuário
- `productivity:task-management` — gerencia tarefas num `TASKS.md` compartilhado

Coleção: `github.com/anthropics/knowledge-work-plugins`

**Armadilhas:**
- **Acumular skills e plugins não vira produtividade sem mudar o rito.** Instalar 20 plugins não te faz mais produtivo se você continua trabalhando do mesmo jeito. A pergunta certa: *qual rotina da minha semana muda depois de instalar isso?* Se nenhuma, não instala.
- **Plugin pronto dá esqueleto, não julgamento.** Um plugin de "análise de variação" te dá a estrutura, não a leitura do seu contexto (por que aquela linha caiu, o que a diretoria vai perguntar). Ferramenta boa acelera; não substitui a decisão do líder.

> *"Skills são muito mais compartilháveis e mantêm o contexto enxuto — o que melhora bastante o desempenho com o tempo."* — Jan · 9x Claude Cowork Workshop

*Personalização não tem caso próprio no grid — é demonstrada ao vivo em aula.*

---

## Agora · mão na massa — 6 casos para praticar

Cada caso termina com você baixando um arquivo real, colando no Claude, e vendo o resultado ao vivo. Comece pelo que mais parece com um problema seu desta semana.

| # | Caso | Estação-âncora | O que você baixa |
|---|------|----------------|-------------------|
| 1 | [Comitê no Projects — SST/Qualidade](exemplos/comite-sst-projects/) | Projects + Artifacts | política SST (mock) + instruções do Project |
| 2 | [Destrave um tema técnico — OEE](exemplos/destrave-oee/) | Extended Thinking + Artifacts | dados OEE (mock) + prompt |
| 3 | [Prepare a reunião trimestral](exemplos/reuniao-trimestral/) | Cowork + Connectors + ET | export Slack + receita trimestral + prompt + gabarito |
| 4 | [Análise de segmento bottom-up](exemplos/analise-segmento/) | Cowork + Extended Thinking | planilha TAM/SAM/SOM + prompt |
| 5 | [Converse com sua planilha](exemplos/converse-planilha/) | Artifacts + Chat | produção×venda 6 SKUs (mock) + prompt |
| 6 | [Lote de fornecedores](exemplos/lote-fornecedores/) | Cowork em batch | 5 PDFs de cotação + prompt |

Todos os arquivos são **fictícios** (contexto de treinamento). Nenhum caso pede colar dado real — cada um usa mock, e o fechamento aponta o Checklist de Anonimização (M4) pra quando você for adaptar o exercício pra rotina real.

---

## Antes de sair deste módulo

Você viu o ecossistema Claude aplicado em 6 situações reais de gestão: comitê no Projects, destrave de tema técnico, reunião trimestral, análise de segmento, conversa com planilha, lote de fornecedores.

**Reflita:**
- Qual desses casos mais se parece com um problema que você enfrenta essa semana?
- Qual estação do funil (Chat · Cowork · Projects · Artifacts · Personalização) você ainda não usa e faria diferença no seu dia?
- Onde você precisaria do Checklist de Anonimização (M4) antes de aplicar em documento real?

**Principais pontos pra levar:**
- Chat pensa · Cowork delega
- Projects preserva contexto pra rotina recorrente
- Artifacts vira algo editável em tempo real
- Skills escalam sua expertise sem inflar o contexto

*Escolha um dos 6 casos, baixe o artefato, teste na sua rotina essa semana.*

---

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Gestão · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
