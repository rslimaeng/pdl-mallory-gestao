# Artefatos · Trilha 2 — Gestão

**O kit do gestor.** Os templates executivos do dia — Canvas, roteiro de 3 frases, CLAUDE.md — prontos para copiar, e o plano das 4 semanas que transformam o treinamento em piloto rodando.

[← Início](../) · [M1](../m1/) · [M2](../m2/) · [M3](../m3/) · [M4](../m4/) · [M5](../m5/) · [M6](../m6/) · [Banco de Prompts](../banco-de-prompts/)

---

## Calculadora ROI · Oportunidades de IA

Ferramenta interativa do **M3**. Traduza suas oportunidades do Mapa em R$/mês e R$/ano — pra defender prioridade em 1 minuto. Preencha 5 campos, empilhe quantas oportunidades quiser e leve o ranking com valor defensável pra reunião de área.

*Módulo · M3 · Identificação de Oportunidades*

**[→ Abrir a Calculadora ROI](calculadora-roi.html)**

---

## Templates copiáveis

### Canvas Executivo — os 5 casos da trilha, preenchidos como exemplo

| Oportunidade | Impacto esperado | Recursos | Próximos passos | Indicadores |
|---|---|---|---|---|
| Controladoria: desvios do mês em 1 página para a diretoria | ~6h/mês de gestor (≈ R$ 500/mês, conservador) | Conta Claude, prompt do M2, dados desidentificados | Rodar no fechamento de julho · validar com diretor · padronizar | Tempo de preparação do briefing: de 1 dia para 2h |
| Jurídico: triagem de cláusulas de risco em contratos de fornecedor | ~8h/mês; reunião preparada em horas, não dias | Conta Claude, prompt do M4, contratos desidentificados | Testar em 2 contratos · validar com parecer humano · definir fluxo | Contratos triados/mês com dupla checagem |
| RH: pesquisa de clima em 3 comunicações sob medida | ~5h/ciclo + mensagem que chega certa em cada público | Conta Claude, prompt do M3, resultados agregados (sem dado individual) | Aplicar no próximo ciclo · colher reação · ajustar tom | Prazo entre resultado e comunicação: de 2 semanas para 3 dias |
| Logística/Importação: cruzamento estoque × demanda para prioridade de contêineres | ~10h/mês e decisão antecipada em 1 semana | Workstation Cowork (M5), planilhas de estoque e demanda | Montar pasta curada · rodar 1 ciclo em paralelo ao processo atual · comparar | Aderência da prioridade sugerida vs. decidida |
| Planejamento: indicadores do S&OP em briefing com cenários | ~6h/ciclo de preparação de reunião | Conta Claude, prompt de cenários do M2, indicadores agregados | Gerar no próximo S&OP · comparar com briefing manual · adotar | Tempo de preparação e nº de retrabalhos pós-reunião |

### Canvas Executivo — template em branco

| Campo | Seu piloto |
|---|---|
| Oportunidade (a rotina, em 1 frase) | |
| Impacto esperado (horas/mês × custo/hora, em R$) | |
| Recursos (o que já tenho · o que falta · quem aprova) | |
| Próximos passos (3 ações datadas; a 1ª até sexta) | |
| Indicadores (métrica que já existe + alvo em 30 dias) | |

### Roteiro de 3 frases para diretoria

1. "Hoje, [processo] consome [X horas/mês] da área — cerca de [R$ Y/mês]."
2. "Proponho um piloto de 30 dias: [o quê], usando [recursos que já temos], medido por [indicador]."
3. "Retorno esperado: [horas ou R$]. Trago o resultado medido na revisão de [data marcada]."

Três frases, três números, uma data. Se a proposta não cabe nesse formato, ela ainda não está pronta para a mesa.

### CLAUDE.md base da workstation

Copie para um arquivo chamado `CLAUDE.md` na raiz da pasta de trabalho e preencha com o seu contexto:

```markdown
# CLAUDE.md — Workstation [Área] · Mallory

## Quem trabalha aqui
Sou [nome], [cargo] da área de [área] na Mallory Eletroportáteis
(fabricante de eletroportáteis, ISO 9001, ERP Datasul).
Esta workstation apoia as rotinas de [ex.: fechamento mensal e relatórios da área].

## Tom e formato
- Português do Brasil, direto, sem jargão não traduzido.
- Documentos no padrão: título, data, seções numeradas, no máximo 1 página
  salvo pedido em contrário.
- Tabelas para comparação; parágrafo para recomendação.

## O que SEMPRE fazer
- Perguntar antes de assumir: se faltar informação, pare e pergunte. Não invente.
- Mostrar o plano de etapas antes de executar tarefas com mais de 2 passos.
- Citar de qual arquivo da pasta veio cada número usado.
- Salvar resultados em /saidas com data no nome do arquivo.

## O que NUNCA fazer
- Nunca criar número, data ou nome que não esteja nos arquivos da pasta.
- Nunca apagar ou sobrescrever arquivo sem confirmar comigo.
- Nunca concluir recomendação definitiva em tema que exige parecer humano
  (jurídico, pessoas, decisão de diretoria) — sinalizar para minha revisão.

## Arquivos de referência
- /referencia/modelo-relatorio.md — o padrão dos meus relatórios
- /referencia/glossario-area.md — termos e siglas da área
```

As duas regras de ouro: **enxuto** (o CLAUDE.md é carregado em toda sessão — até ~300 linhas, apontando para arquivos de referência em vez de colar tudo nele) e **limpo** (nenhum dado das 5 categorias dentro dele).

### memory.md — exemplo mínimo

O segundo arquivo de memória da workstation: o que ela aprende e decide ao longo do uso. Começa com 3 linhas e cresce:

```markdown
# memory.md — Workstation [Área]
- Relatório mensal vai para o diretor [X]; sempre versão em 1 página.
- Fechamos os números no dia 3 de cada mês.
- Tabela comparativa sempre com a coluna "vs. mês anterior".
```

### Cheatsheet PCTFL avançado

```text
P — PAPEL       quem a IA deve ser (nível e vocabulário da resposta)
C — CONTEXTO    a situação da sua área, com números desidentificados
T — TAREFA      o que fazer, com verbo de gestão: analise, compare, estruture
F — FORMATO     o entregável: 1 página, tabela, blocos definidos
L — LIMITAÇÕES  o que não fazer — sempre abrindo com a regra de ouro:
                "Se faltar informação, pergunte. Não invente."

# CRITÉRIO DE SUCESSO   como você saberá que cumpriu:
                        "funciona se [destinatário] conseguir [ação]
                         sem pedir esclarecimento"
# CRITÉRIO NEGATIVO     o que a resposta NÃO pode ser: tom, formato,
                        conteúdo proibido

Regra do módulo 2: 5 minutos no prompt, 45 a menos no retrabalho.
```

### Régua de redesenho: Autopiloto · Colaboração · Manual

| Faixa | O que significa | Exemplos |
|---|---|---|
| **Autopiloto** | A IA faz o rascunho ou a compilação inteira; alguém revisa | Relatório recorrente, primeira versão de documento |
| **Colaboração** | A IA apoia, o humano conduz | Análise, cenário, preparação de decisão |
| **Manual** | A IA não entra | Decisão sobre pessoa, assinatura de parecer, aprovação final |

Redesenhar processo com IA é decidir a faixa de cada etapa — e escrever isso na diretriz da área (M4).

### As 5 categorias que nunca entram em ferramenta externa

```text
1. GENTE         nome, CPF, salário, atestado, avaliação, dado de candidato (LGPD)
2. PRODUTO       especificação, parâmetro de processo, desenho, fórmula
3. CONTRATO      contratos, preços, condições de fornecedor e cliente
4. DIRETORIA     resultado não divulgado, plano estratégico, decisão em discussão
5. CONCORRÊNCIA  informação de negociação ou inteligência competitiva

O teste do gestor: se vazasse, quem daria explicação é você? Então não entra.
```

---

## Dados fictícios para praticar

Os materiais de exercício dos módulos — **distribuídos em sala** pelo instrutor, para treinar sem nenhum dado real da Mallory:

- **Resumo de desvios de junho** (exercício do M2) — os números fictícios do briefing de desvios. *Distribuído em sala.*
- **Cenário para análise de decisão** (Desafio do M2) — a decisão pendente para montar os 3 cenários com premissas. *Distribuído em sala.*
- **Resultado da pesquisa de clima** (exercício do M3) — os agregados fictícios do padrão "1 fonte, N narrativas". *Distribuído em sala.*
- **Contrato de fornecedor de componentes plásticos** (exercício do M4) — o contrato fictício da análise de cláusulas de risco. *Distribuído em sala.*

---

## Material de apoio

- [Anthropic Economic Index](https://www.anthropic.com/research) — a análise contínua de milhões de conversas do Claude no trabalho, citada no M1: redação, análise e síntese dominam o uso profissional; decisão automatizada quase não aparece.
- [Documentação do Claude](https://docs.anthropic.com) — referência oficial de chat, projetos e Cowork (em inglês).
- **Referências do Claude Cowork** — os vídeos que embasaram as demonstrações do M5: *"Claude Cowork FULL COURSE 3 Hours"* e *"Claude Cowork: O Assistente que Trabalha por Você"* (Anwar Hermuche) — busque pelos títulos; peça os links ao instrutor pelo canal do time.
- **WEF Future of Jobs 2025** — o relatório do Fórum Econômico Mundial citado no M1 (IA e dados entre as competências que mais crescem em demanda). Peça o material ao instrutor pelo canal do time.

---

## As 4 semanas que consolidam o L2

Você sai do treinamento em L2 — PCTFL avançado no fluxo e workstation construída em grupo. O que separa isso de "treinamento que passou" é o que acontece agora:

| Semana | O que fazer | De onde vem |
|---|---|---|
| **1** | Agendar e realizar a sessão de 30 min do grupo na conta compartilhada — 1 tarefa real na workstation de sala | Marco do M5 |
| **2** | Rodar o piloto do Canvas: primeira ação datada executada, indicador com número inicial registrado | Marco do M6 |
| **3** | Revisão de 30 dias preparada: dado do indicador coletado, comparação antes × depois em 3 linhas | Canvas, campo Indicadores |
| **4** | Comunicar o resultado (diretoria ou fórum da área) e decidir: escalar, ajustar ou encerrar sem drama | Roteiro de 3 frases, com número medido |

A régua completa L0→L3 está no [M5](../m5/) — ela não expira: L3 (projeto dedicado + skill própria) é o degrau natural de quem fechar as 4 semanas com o piloto de pé.

---

## Nota sobre as licenças Cowork

O Claude Cowork exige conta paga (Claude Pro). O modelo combinado com o TI da Mallory: **contas Pro compartilhadas, ~4 gestores por conta**, organizadas nos grupos do M5 — válidas por 1 mês após o treinamento, cobrindo as 4 semanas do plano acima. Nesse período, o grupo agenda as sessões na conta compartilhada (marco do M5). Se a sua área decidir continuar depois do piloto, o encaminhamento é solicitar conta individual via TI — leve o Canvas com o resultado medido: é ele que justifica a licença.

---

[← Banco de Prompts](../banco-de-prompts/) · [Início](../)
