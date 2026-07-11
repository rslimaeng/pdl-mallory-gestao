# M2 · IA para Gestores: Prática em Decisão, Análise e Comunicação

**Trilha 2 · Módulo 2 de 6 · 1h15**

Análise de cenários, extração de insight de relatórios e comunicação estratégica — executados por você, ao vivo.

---

## O contrato deste módulo

**Você ganha:** o PCTFL avançado — com Critério de Sucesso e Critério Negativo — aplicado às 3 tarefas mais caras do seu cargo: analisar, decidir, comunicar.

**Você se compromete a:** executar os 3 prompts ao vivo com material da sua área (desidentificado) e avaliar cada resposta contra o critério que você mesmo definiu.

**Tempo de leitura desta página:** 10 min

---

## Você entra com → O que acontece → Você sai com

| Você entra com | O que acontece | Você sai com |
|---|---|---|
| A hipótese do M1 e sua conta no Claude configurada | Você aprende as 2 camadas que faltam no seu prompt — Critério de Sucesso e Negativo — e roda 3 execuções reais | 3 prompts de alto valor executados: síntese de relatório, comunicado de liderança e análise de cenário — o método alimenta o M3 |

---

## Por que isso importa aqui dentro

O comitê é quinta-feira. Você tem o relatório de 30 páginas da sua área, os números do mês e 40 minutos livres na agenda até lá. O que você faz nesses 40 minutos define a qualidade da sua fala — e hoje eles vão embora em compilar e formatar, não em pensar.

Você já usa IA — a diferença desta turma para a da manhã é essa. Mas há um degrau entre usar e extrair valor consistente: quando você mostra a resposta da IA para outra pessoa e ela diz "não era bem isso", o problema quase nunca é a IA. É a definição de "bom" que ficou na sua cabeça e não entrou no prompt.

É o mesmo princípio de delegar para a equipe. Dizer só *o que* fazer é briefing incompleto. Delegação de gestor entrega o pacote: faça isto, baseie-se nestes dados, evite estes erros, e vou avaliar por este critério. O PCTFL avançado é exatamente isso — por escrito, para a IA.

---

## O conceito em 5 pontos

### 1. As 2 camadas que separam prompt funcional de prompt de gestor

**Critério de Sucesso:** como você saberá que a resposta cumpriu o objetivo — na fórmula *"a resposta funciona se [destinatário] conseguir [ação] sem pedir esclarecimento"*. **Critério Negativo:** o que a resposta não pode ser — tom, formato, conteúdo proibido. Sem o primeiro, você avalia por sensação; sem o segundo, a IA entrega a média da internet.

### 2. Análise de cenário: premissas explícitas, nunca "o que você acha?"

Pergunta de opinião gera resposta de opinião — rasa e sem dono. O padrão de gestor: "monte 3 cenários (base, otimista, pessimista) para [decisão], com premissas explícitas em cada um, e aponte qual premissa, se falhar, derruba o cenário". A IA organiza o espaço da decisão; as premissas você valida — e a escolha é sua.

### 3. Narrativa executiva: dado → significado → ação

Todo relatório pode parar em 3 alturas. **Observação:** "a rubrica X estourou 12%". **Insight:** "o estouro é estrutural — 3º mês seguido, mesmo direcionador". **Ação:** "renegociar o contrato Y antes do próximo ciclo". Entregar só a observação é largar o trabalho difícil com o leitor. Instrua a IA a subir os 3 degraus — e revise se o insight é seu de verdade.

### 4. Uma fonte, N narrativas

O mesmo resultado do mês vira: 1 página analítica para a diretoria, 5 linhas de prioridades para seus coordenadores, 1 comunicado claro para o time. Ninguém tem tempo de escrever 3 documentos — e a IA transforma o primeiro nos outros dois em minutos, se o prompt disser quem lê cada um e o que cada leitor deve fazer depois de ler.

### 5. O hábito que paga o módulo: 5 minutos no prompt, 45 a menos no retrabalho

Prompt de gestor se escreve uma vez e se reusa o ano inteiro — o do fechamento de janeiro serve para os outros 11. O custo real não é o tempo de escrever o prompt completo; é o ciclo de "não era isso" que o prompt incompleto gera. Salve os seus 3 melhores. Eles são ativo da área.

---

## Quando aplicar / Quando NÃO aplicar

| 🟢 Quando aplicar | 🔴 Quando NÃO aplicar |
|---|---|
| Sintetizar relatório longo em briefing com decisão sugerida | Delegar a decisão à IA — ela estrutura cenários, você escolhe |
| Montar cenários com premissas explícitas antes de decidir | Colar relatório com dado confidencial sem desidentificar (M4) |
| Adaptar a mesma mensagem para diretoria, gestores e time | Assinar número que você não recalculou na fonte |
| Ensaiar conversa difícil ou antecipar objeções da diretoria | Usar a resposta como parecer técnico — parecer tem responsável, e é você |

---

## Prompt-âncora do módulo

O briefing de desvios orçamentários — o caso que todo gestor da sala reconhece. Dados fictícios; roda como está:

```text
# PAPEL
Você é um controller sênior com experiência em indústria de manufatura no Brasil.

# CONTEXTO
Fechamento de junho de uma fabricante de eletroportáteis. Dados FICTÍCIOS do meu resumo:
- Orçado total: R$ 8,2 mi · Realizado: R$ 8,9 mi (desvio +8,5%)
- Frete: orçado R$ 620 mil, realizado R$ 840 mil (3º mês seguido acima; novo contrato só em setembro)
- Energia: orçado R$ 410 mil, realizado R$ 465 mil (bandeira tarifária, pontual)
- Manutenção: orçado R$ 380 mil, realizado R$ 510 mil (parada não programada da injetora 7)
- Demais rubricas dentro de ±2%

# TAREFA
Redija o briefing de desvios para a reunião de diretoria: separe desvio estrutural
de pontual, explique o direcionador de cada um e sugira 1 ação por desvio relevante.

# FORMATO
1 página: parágrafo de abertura com o número total e a mensagem central ·
tabela (Rubrica | Desvio | Estrutural ou Pontual | Direcionador | Ação sugerida) ·
fechamento com os 2 pontos que exigem decisão da diretoria.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Use apenas os números do contexto — não crie projeção que os dados não sustentam.

# CRITÉRIO DE SUCESSO
A diretoria decide sobre os 2 pontos finais sem abrir o relatório completo.

# CRITÉRIO NEGATIVO
Não use jargão contábil sem tradução. Não suavize desvio estrutural como se fosse
pontual. Não proponha ação que dependa de orçamento novo.
```

Para o seu caso: troque o CONTEXTO pelos seus números (desidentificados), reescreva o Critério de Sucesso pensando em quem recebe — e o resto é reuso.

---

## Exercício

### Camada 1 — Básico (todos · 10-15 min)

**Objetivo:** executar 2 dos 3 prompts do módulo — síntese e comunicado — com material seu.

**Passo a passo:**
1. Rode o prompt-âncora como está e compare a resposta com o Critério de Sucesso dele. Passou? (Ainda sem conta? [claude.ai](https://claude.ai) → "Continuar com Google" — 2 minutos, e o colega do lado ajuda. A maioria da sala já chega logada.)
2. Adapte: troque o CONTEXTO por um resumo real da sua área (números desidentificados — troque valores reais por aproximados) e rode de novo.
3. Terceira execução — o comunicado de liderança: na mesma conversa, peça: "Transforme este briefing em um comunicado de 10 linhas para meus coordenadores: o que muda para eles e o que espero de cada um até o fim do mês. Critério de sucesso: cada coordenador sabe sua prioridade sem me perguntar. Negativo: sem tom de cobrança genérica."
4. Avalie cada resposta contra o critério que você escreveu — não contra "achei bom".

**Resultado esperado:** 1 briefing da sua área + 1 comunicado derivado dele, ambos avaliados por critério explícito.

**Como avaliar:** pergunta-teste: se você enviasse agora, o destinatário executaria sem te procurar? Se a resposta é "ia me ligar para perguntar X", o X faltou no prompt — ajuste e rode de novo.

### Camada 2 — Desafio (para quem terminou · +10-15 min)

**Objetivo:** o terceiro prompt — análise de cenário com premissas explícitas.

**Passo a passo:**
1. Escolha 1 decisão real pendente na sua área (renovar contrato, redistribuir equipe, antecipar compra).
2. Monte o PCTFL avançado: tarefa = "monte 3 cenários com premissas explícitas e aponte a premissa que, se falhar, derruba cada cenário"; Critério de Sucesso = "consigo defender a escolha em reunião citando premissas, não achismos"; Negativo = "não recomende um cenário — a escolha é minha".
3. Rode. Valide as premissas uma a uma: quais são fato, quais são chute da IA?
4. Refine: "a premissa 2 do cenário base está errada — [fato real]. Refaça os cenários."

**Resultado esperado:** 3 cenários com premissas marcadas por você como fato ou chute — e 1 refinamento que mudou a análise.

**Como avaliar:** se você consegue apontar qual premissa vigia daqui pra frente, a análise virou instrumento de decisão. Se os 3 cenários parecem intercambiáveis, as premissas ficaram genéricas — aperte o CONTEXTO.

---

## Os 3 erros mais comuns

| Erro | Sintoma | Causa | Como corrigir |
|---|---|---|---|
| Avaliar por sensação | "Achei boa" — e o destinatário devolve com 4 perguntas | Critério de Sucesso ficou na cabeça, não no prompt | Escreva o critério antes do prompt: quem recebe, faz o quê, sem perguntar o quê |
| Pedir opinião em vez de estrutura | "O que você acha de X?" — resposta morna, dos dois lados | Delegar o julgamento em vez do preparo | Peça cenários, premissas, riscos, comparação por critério — e decida você |
| Reescrever em vez de refinar | Resposta 80% boa, você reescreve os 20% na mão, toda vez | Tratar cada resposta como final, não como iteração | Devolva na mesma conversa: "revise considerando [o que faltou]" — 2 iterações batem 1 reescrita |

---

> ⚠️ **Anti-alucinação — antes do briefing subir**
> - **Não deixe a IA inventar número que não está no seu relatório fonte.** O Critério Negativo trava; o protocolo confere: fonte · número · consistência.
> - O briefing que sobe para a diretoria com número inventado não é erro da IA — **é erro seu, com o seu nome**. Revisão de conteúdo não é opcional em documento de decisão.
> - Caso-âncora: **Mata v. Avianca (2023)** — texto fluido, conteúdo fabricado, sanção real. O M4 traz o protocolo completo para você e para a sua equipe.

---

> 🟣 **Marco: o que você leva para a Mallory na 2ª feira**
> Até sexta-feira, gere com PCTFL avançado 1 documento real do seu cargo — briefing, síntese ou comunicado — e use de verdade: envie ou apresente a quem ele se destina.
> Como saber que aconteceu: o documento chegou ao destinatário, e o prompt está salvo para o próximo ciclo.

---

[← M1 · O Cenário Global de IA](../m1/) · [M3 · IA por Área →](../m3/)

[Banco de Prompts](../banco-de-prompts/) · [Artefatos](../artefatos/)
