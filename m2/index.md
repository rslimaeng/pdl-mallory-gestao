# M2 · IA para Gestores: Prática em Decisão, Análise e Comunicação

**Trilha 2 · Módulo 2 de 6**

Análise de cenários, extração de insight de relatórios e comunicação estratégica — executados por você, ao vivo.

---

## O contrato deste módulo

**Você ganha:** o PCTFL avançado — com Critério de Sucesso — aplicado às 3 tarefas mais caras do seu cargo: analisar, decidir, comunicar.

**Você se compromete a:** executar os 3 prompts ao vivo com material da sua área (desidentificado) e avaliar cada resposta contra o critério que você mesmo definiu.

---

## Você entra com → O que acontece → Você sai com

| Você entra com | O que acontece | Você sai com |
|---|---|---|
| A hipótese do M1 e sua conta no Claude configurada | Você aprende a camada que falta no seu prompt — o Critério de Sucesso — e roda 3 execuções reais | 3 prompts de alto valor executados: síntese de relatório, comunicado de liderança e análise de cenário — o método alimenta o M3 (matriz 3D · ranking por (I×F)/Risco) |

---

## Por que isso importa aqui dentro

O comitê é quinta-feira. Você tem o relatório de 30 páginas da sua área, os números do mês e 40 minutos livres na agenda até lá. O que você faz nesses 40 minutos define a qualidade da sua fala — e hoje eles vão embora em compilar e formatar, não em pensar.

Você já usa IA — a diferença desta turma para a da manhã é essa. Mas há um degrau entre usar e extrair valor consistente: quando você mostra a resposta da IA para outra pessoa e ela diz "não era bem isso", o problema quase nunca é a IA. É a definição de "bom" que ficou na sua cabeça e não entrou no prompt.

É o mesmo princípio de delegar para a equipe. Dizer só *o que* fazer é briefing incompleto. Delegação de gestor entrega o pacote: faça isto, baseie-se nestes dados, evite estes erros, e vou avaliar por este critério. O PCTFL avançado é exatamente isso — por escrito, para a IA.

---

## Um prompt ruim é sempre culpa do humano

A IA é previsível: ela gera saídas proporcionais à qualidade da entrada. Prompt vago → resposta vaga. Prompt preciso → resposta precisa. **A engenharia de prompt é a habilidade de escrever a entrada certa.**

**Anthropic Economic Index** confirma o padrão: os usos que mais falham são os pedidos vagos, sem contexto. O que resolve é método — não talento nem ferramenta melhor.

| Prompt vago | Problema | Resultado provável |
|---|---|---|
| "Analise esse relatório aí" | Sem foco, sem decisão a suportar | Resumo genérico, ninguém decide com ele |
| "Faz um comunicado pra diretoria" | Sem tese, sem destinatário | Texto morno, sem posição |
| "Sintetiza esse dashboard" | Sem hierarquia do que importa | Lista de números sem prioridade |

Esse módulo te dá o método pra sair desses 3 casos — em 3 exercícios executados por você, ao vivo.

---

## Vago × Situado — a diferença que muda tudo

O mesmo pedido escrito de dois jeitos. Um recebe o que a internet daria; o outro recebe o que decide a reunião.

**Exemplo 1 · cenário**
- 🔴 **Vago:** "O que você acha desse cenário aqui?" → opinião morna dos dois lados, sem premissa explícita — e ninguém decide com isso.
- 🟢 **Situado:** "Monte 3 cenários (base/otimista/pessimista) pra decidir X, com premissas explícitas em cada. Aponte qual premissa, se falhar, derruba o cenário." → o espaço da decisão organizado — você valida premissas e escolhe com argumento.

**Exemplo 2 · síntese**
- 🔴 **Vago:** "Faz um resumo desse relatório." → paráfrase sem hierarquia, sem decisão sugerida — trabalho difícil ainda com você.
- 🟢 **Situado:** "Sintetize este relatório em 1 página pra reunião de diretoria. Formato: abertura com a mensagem central · tabela (Rubrica · Desvio · Estrutural/Pontual · Ação) · fechamento com os 2 pontos que exigem decisão." → briefing que a diretoria lê e decide sem abrir o relatório completo.

A diferença não é a IA. É o quanto você **situa** o pedido — e, no nível de gestor, o quanto você declara o que é uma resposta bem-sucedida. O método a seguir — PCTFL+ — é isso, virado em checklist.

---

## Quando a fonte é planilha — o segundo caso do módulo

Até aqui você viu prompt sobre **relatório curto ou número já resumido** — briefing, comunicado, cenário. Existe um segundo caso, o mais desconfortável pro gestor: **quando a fonte é planilha de 500-2.000 linhas de dado bruto** que ninguém teve tempo de olhar linha por linha. Fluxo de caixa detalhado, apontamento de refugo por lote, extrato do cartão corporativo, base de reclamação de cliente. **Manual leva horas; Excel manual não pega tudo; IA em 1 prompt correto extrai o que importa em minutos — se você validar amostra antes de confiar no todo.**

Aqui a lente é diferente. Você não pede pra IA "resumir". Você pede pra ela **enxergar padrão que você não teria tempo de enxergar sozinho** — e depois valida.

### O caso âncora: refugo por lote da injetora 7 nos últimos 90 dias

Situação concreta que todo gestor Mallory reconhece. Você tem uma planilha exportada do Datasul: 800 linhas · colunas *lote · data · turno · operador · quantidade produzida · refugo · tipo de defeito*. Pedir "resuma isso" volta lixo. **O prompt que funciona tem 3 fases sequenciais na mesma conversa** — cada fase entra na próxima.

**Fase 1 · Diagnóstico da planilha (antes de analisar)**

Você começa pedindo pra IA **descrever o dado**, não interpretar ainda:

    Descreva o padrão desta planilha: colunas, tipos de valor, período coberto,
    valores extremos por coluna. Aponte lacunas (células vazias, coluna com
    domínio ambíguo, formato inconsistente). Não interprete ainda. Só descreva.

**Por que:** você economiza a dor de descobrir uma coluna corrompida depois de 20 min de análise. Se a Fase 1 acusa problema, você limpa a planilha antes de seguir — 2 minutos de disciplina evitam 40 min de conclusão errada.

**Fase 2 · Categorização com marcação explícita de lacuna**

Depois do diagnóstico limpo, você pede categorização — e força a IA a **marcar o que ela não sabe**:

    Agrupe as linhas de refugo por causa provável em 4 categorias:
    setup/regulagem, material, operador em treinamento, ruído de processo.
    Nas linhas onde a causa não é clara pelos dados, marque com [A_INVESTIGAR].
    Não invente causa que os dados não sustentam.

**Por que:** sem a instrução de marcar `[A_INVESTIGAR]`, a IA preenche tudo com palpite — e você não sabe onde ela chutou. Com a instrução, ela devolve com honestidade: "70% categorizado, 30% precisa de olho humano". Você olha só os 30%.

**Fase 3 · Caça a anomalias**

Depois da categorização, o pedido que Excel não faz sozinho:

    Aponte as 5 linhas mais anômalas desta planilha por 3 critérios:
    (1) outlier de volume de refugo dentro do próprio turno,
    (2) combinação turno × operador com defeito raro na base histórica,
    (3) tipo de defeito que aparece 1x isolado (não é padrão, é evento).
    Pra cada linha, explique em 1 linha por que chamou a atenção.

**O que sai:** 5 pontos concretos pra você conversar com o PCP e o supervisor de turno. Não são conclusões prontas — são hipóteses de investigação priorizadas pela IA a partir do padrão do dado.

### A regra da amostra — antes de qualquer conclusão

**Antes de assinar qualquer análise que vai virar decisão, valide 5 linhas aleatórias contra a fonte.** Abra a planilha, escolha 5 linhas ao acaso, confira o que a IA disse contra o dado bruto. Se as 5 batem, a probabilidade de o todo estar coerente é alta. Se 1 das 5 falha, ajuste o prompt e rode de novo — **não** conserte no output final.

Este é o **contrato de confiança com IA em dado**: humano assina depois de amostrar, nunca depois só de ler. É a mesma disciplina de auditoria interna aplicada num ciclo 20× mais rápido.

### Quando este caso vale — e quando não

| 🟢 Use análise de dado bruto quando | 🔴 Não use quando |
|---|---|
| A planilha tem 200+ linhas e você não teria tempo de olhar linha por linha | O dado tá em 3 planilhas que precisam ser cruzadas primeiro — limpe antes |
| O padrão de valor já está estruturado (colunas nomeadas, tipos consistentes) | Coluna livre-texto é a mais importante — precisa de tratamento antes (M4) |
| Você quer priorizar 5-10 pontos para investigação humana | Você quer que a IA "decida" — decisão fica com você, sempre |
| Você pode validar amostra na fonte antes de confiar | Você não tem acesso à fonte pra amostrar — sem amostra, sem assinatura |

---

## O conceito em 5 pontos

### 1. A camada que separa prompt funcional de prompt de gestor: o Critério de Sucesso

**Critério de Sucesso:** como você saberá que a resposta cumpriu o objetivo — na fórmula *"a resposta funciona se [destinatário] conseguir [ação] sem pedir esclarecimento"*. O que a resposta **não pode ser** (tom, formato, conteúdo proibido) entra nas **Limitações**, junto do "não invente" — não é um elemento à parte. Sem o Critério de Sucesso, você avalia por sensação; sem limites claros, a IA entrega a média da internet.

### 2. Análise de cenário: premissas explícitas, nunca "o que você acha?"

Pergunta de opinião gera resposta de opinião — rasa e sem dono. O padrão de gestor: "monte 3 cenários (base, otimista, pessimista) para [decisão], com premissas explícitas em cada um, e aponte qual premissa, se falhar, derruba o cenário". A IA organiza o espaço da decisão; as premissas você valida — e a escolha é sua.

### 3. Narrativa executiva: dado → significado → ação

Todo relatório pode parar em 3 alturas. **Observação:** "a rubrica X estourou 12%". **Insight:** "o estouro é estrutural — 3º mês seguido, mesmo direcionador". **Ação:** "renegociar o contrato Y antes do próximo ciclo". Entregar só a observação é largar o trabalho difícil com o leitor. Instrua a IA a subir os 3 degraus — e revise se o insight é seu de verdade.

### 4. Uma fonte, N narrativas

O mesmo resultado do mês vira: 1 página analítica para a diretoria, 5 linhas de prioridades para seus coordenadores, 1 comunicado claro para o time. Ninguém tem tempo de escrever 3 documentos — e a IA transforma o primeiro nos outros dois em minutos, se o prompt disser quem lê cada um e o que cada leitor deve fazer depois de ler.

### 5. O hábito que paga o módulo: 5 minutos no prompt, 45 a menos no retrabalho

Prompt de gestor se escreve uma vez e se reusa o ano inteiro — o do fechamento de janeiro serve para os outros 11. O custo real não é o tempo de escrever o prompt completo; é o ciclo de "não era isso" que o prompt incompleto gera. Salve os seus 3 melhores. Eles são ativo da área.

---

## As 6 camadas — PCTFL + Critério de Sucesso

| Letra | Elemento | O que define | Exemplo (Mallory) |
|---|---|---|---|
| **P** | Papel | Quem a IA deve ser | Controller sênior com experiência em indústria de manufatura no Brasil. |
| **C** | Contexto | A situação real | Fechamento de junho (dados fictícios): desvio +8,5%, frete/energia/manutenção acima do orçado. |
| **T** | Tarefa | O que fazer (com verbo claro) | "Redija o briefing de desvios: separe estrutural de pontual e sugira 1 ação por desvio relevante." |
| **F** | Formato | Como entregar | 1 página: abertura + tabela (Rubrica \| Desvio \| Direcionador \| Ação) + os 2 pontos que exigem decisão. |
| **L** | Limitações | O que NÃO fazer | "Se faltar informação, pergunte. Não invente. Use apenas os números do contexto." |
| **CS** | Critério de Sucesso | Quando a resposta é boa? | A diretoria decide sobre os 2 pontos finais sem abrir o relatório completo. |

**Regra de ouro:** quanto mais você preenche o PCTFL+CS, menos a IA precisa adivinhar — e menos chance de alucinação ou resultado genérico. O CS é o ponto que mais sobe a qualidade: transforma "achei ok" em "atende o critério".

---

## Quando aplicar / Quando NÃO aplicar

| 🟢 Quando aplicar | 🔴 Quando NÃO aplicar |
|---|---|
| Sintetizar relatório longo em briefing com decisão sugerida | Delegar a decisão à IA — ela estrutura cenários, você escolhe |
| Montar cenários com premissas explícitas antes de decidir | Colar relatório com dado confidencial sem desidentificar (M4) |
| Adaptar a mesma mensagem para diretoria, gestores e time | Assinar número que você não recalculou na fonte |
| Ensaiar conversa difícil ou antecipar objeções da diretoria | Usar a resposta como parecer técnico — parecer tem responsável, e é você |

---

## O verbo de ação é o núcleo do T

Todo prompt tem uma "Tarefa". A qualidade da resposta está sempre em **um único lugar: o verbo da Tarefa.** Quando o verbo é vago ("me ajude", "veja"), a IA escolhe sozinha o que fazer — e escolhe pra média. Quando o verbo é preciso ("liste", "compare", "reescreva no tom X"), a IA obedece.

**Teste prático:** se você não consegue substituir o verbo da sua Tarefa por outro sem mudar completamente o pedido, você acertou o verbo.

Troque "me ajude" por verbo cirúrgico — no nível de gestor, o verbo já carrega a estrutura da decisão:

| Área | Verbo vago | Verbo cirúrgico | Exemplo |
|---|---|---|---|
| Análise | analise, veja | monte cenários, aponte premissa, decomponha | "Monte 3 cenários com premissas explícitas…" |
| Decisão | recomende, escolha | compare por critério, aponte trade-off, ranqueie | "Compare por [custo, prazo, risco]…" |
| Comunicação | escreva, faça | reescreva pra diretoria em 1 página, adapte pra 5 linhas de coordenador | "Adapte esta síntese pra 5 linhas de prioridade…" |
| Diagnóstico | avalie, diga o que acha | liste hipóteses, aponte a mais provável, dê próximo passo pra validar | "Liste 5 hipóteses e a que testaria primeiro…" |
| Preparação | prepare, ajude | ensaie objeções, aponte perguntas hostis, treine pitch | "Ensaie 5 objeções de diretor cético…" |

> ⚙️ **Regra prática:** antes de rodar um prompt, sublinhe o verbo da sua Tarefa. Se for "me ajude", "faça", "veja", "melhore" — pare e troque. Só rode com verbo cirúrgico.

---

> 💡 **Conexão com o M1: modo + método**
> No M1 você viu os 3 modos + a separação Delegação × Estruturação. O PCTFL+CS é o
> método que aparece em cada:
> - **Delegação (Autopiloto/Colaboração):** PCTFL+CS estruturado, roda e revisa contra o Critério.
> - **Estruturação (Colaboração no modo sócio-analítico):** PCTFL+CS aberto, com iteração
>   e crítica em rounds — a IA vira interlocutora, não copista.
> - **Manual:** PCTFL não entra — decisão executiva sem intermédio.

---

## Por que Claude, se a ementa fala em 3 ferramentas?

A ementa oficial cita **ChatGPT, Claude e Microsoft Copilot** — as 3 dominantes hoje. Não vamos treinar todas as 3 nesta manhã: a habilidade que você leva daqui **transfere**. Um bom pedido bem estruturado (o que o M2 ensina) funciona igual em qualquer uma delas.

**As ferramentas fazem coisas parecidas por caminhos diferentes** — assistentes customizados por outros nomes:

| Ferramenta | Assistente customizado | Onde brilha |
|---|---|---|
| **ChatGPT** (OpenAI) | **GPTs** — GPT com contexto e instruções fixas | Ecossistema amplo, plugins, geração de imagem |
| **Claude** (Anthropic) | **Projects** — pasta com arquivos + instruções | Análise longa, escrita executiva, código, **Cowork** (M5) |
| **Gemini** (Google) | **Gems** — Gemini com papel fixo | Integração com Google Workspace |
| **Copilot** (Microsoft) | Copilot for Excel / Word / Teams | Integração nativa no M365 |

**Por que Claude neste treino:** a TI da Mallory adquiriu **licenças Claude Pro pagas** para o programa. Você recebe acesso e leva pra dentro. Se sua área usar outra ferramenta na rotina, os mesmos princípios (Papel · Contexto · Tarefa · Formato · Limitações + Critério de Sucesso) valem — muda a interface, não a habilidade.

**Preview:** no M5 (Claude Cowork) você vai usar o **Projects** — a versão avançada onde o Claude ganha acesso a arquivos e ferramentas. É pra isso que a Pro paga da TI existe.

---

## Gerador de prompt — ferramenta viva

Uma ferramenta viva pra montar seu próprio PCTFL+CS: 6 campos à esquerda, o prompt monta sozinho à direita — você copia e cola no Claude. **Está na versão HTML deste módulo** (abra a página no navegador): é Delegação com método. Lendo só este Markdown? Use o prompt-âncora abaixo como molde e preencha as 6 camadas na mão.

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
Não use jargão contábil sem tradução. Não suavize desvio estrutural como se fosse
pontual. Não proponha ação que dependa de orçamento novo.

# CRITÉRIO DE SUCESSO
A diretoria decide sobre os 2 pontos finais sem abrir o relatório completo.
```

Para o seu caso: troque o CONTEXTO pelos seus números (desidentificados), reescreva o Critério de Sucesso pensando em quem recebe — e o resto é reuso.

---

## Exercício

### Camada 1 — Básico (todos · 10-15 min)

**Objetivo:** executar 2 dos 3 prompts do módulo — síntese e comunicado — com material seu.

**Passo a passo:**
1. Rode o prompt-âncora como está e compare a resposta com o Critério de Sucesso dele. Passou? (Ainda sem conta? [claude.ai](https://claude.ai) → "Continuar com Google" — 2 minutos, e o colega do lado ajuda. A maioria da sala já chega logada.)
2. Adapte: troque o CONTEXTO por um resumo real da sua área (números desidentificados — troque valores reais por aproximados) e rode de novo.
3. Terceira execução — o comunicado de liderança: na mesma conversa, peça: "Transforme este briefing em um comunicado de 10 linhas para meus coordenadores: o que muda para eles e o que espero de cada um até o fim do mês. Critério de sucesso: cada coordenador sabe sua prioridade sem me perguntar. Nas limitações: sem tom de cobrança genérica."
4. Avalie cada resposta contra o critério que você escreveu — não contra "achei bom".

**Resultado esperado:** 1 briefing da sua área + 1 comunicado derivado dele, ambos avaliados por critério explícito.

**Como avaliar:** pergunta-teste: se você enviasse agora, o destinatário executaria sem te procurar? Se a resposta é "ia me ligar para perguntar X", o X faltou no prompt — ajuste e rode de novo.

### Camada 2 — Desafio (para quem terminou · +10-15 min)

**Objetivo:** o terceiro prompt — análise de cenário com premissas explícitas.

**Passo a passo:**
1. Escolha 1 decisão real pendente na sua área (renovar contrato, redistribuir equipe, antecipar compra).
2. Monte o PCTFL avançado: tarefa = "monte 3 cenários com premissas explícitas e aponte a premissa que, se falhar, derruba cada cenário"; Critério de Sucesso = "consigo defender a escolha em reunião citando premissas, não achismos"; nas Limitações: "não recomende um cenário — a escolha é minha".
3. Rode. Valide as premissas uma a uma: quais são fato, quais são chute da IA?
4. Refine: "a premissa 2 do cenário base está errada — [fato real]. Refaça os cenários."

**Resultado esperado:** 3 cenários com premissas marcadas por você como fato ou chute — e 1 refinamento que mudou a análise.

**Como avaliar:** se você consegue apontar qual premissa vigia daqui pra frente, a análise virou instrumento de decisão. Se os 3 cenários parecem intercambiáveis, as premissas ficaram genéricas — aperte o CONTEXTO.

### Camada 3 — Análise de dado bruto (para quem terminou 2 · +10-15 min)

**Objetivo:** aplicar as 3 fases (diagnóstico → categorização → anomalias) numa planilha real sua.

**Pré-requisito:** planilha do seu dia que você **nunca teve tempo de olhar linha por linha** — 200+ linhas, dado desidentificado. Sugestões: extrato do cartão corporativo do trimestre, apontamento de refugo/parada da sua linha, base de reclamação de cliente, planilha de fechamento com detalhamento por rubrica.

**Passo a passo:**
1. Cole a planilha (ou os primeiros 50 linhas se for muito grande) no chat e rode a **Fase 1 · Diagnóstico** exatamente como está na seção acima. Leia com atenção: a IA aponta lacuna, coluna ambígua, formato quebrado? Corrija a planilha antes de seguir.
2. Rode a **Fase 2 · Categorização** com as 4 categorias adaptadas ao seu caso (custo tem outras categorias; reclamação de cliente tem outras). **Não pule a instrução `[A_INVESTIGAR]`** — se tirar, você perde a honestidade da IA.
3. Rode a **Fase 3 · Caça a anomalias**. Ajuste os 3 critérios pro seu contexto (o "turno × operador" só faz sentido pra refugo — pra custo, seria "categoria × fornecedor", etc).
4. **Aplique a regra da amostra:** escolha 5 linhas aleatórias no output da Fase 3, abra a planilha bruta, confira uma a uma. Bateu? Continue. Não bateu? Volte a Fase 2 com prompt corrigido.

**Resultado esperado:** 5 pontos concretos que valem levar pra próxima reunião de área — com a certeza (validada por amostra) de que não são invenção da IA.

**Como avaliar:** se você consegue explicar cada um dos 5 pontos a um colega apontando pra linha da planilha bruta, o exercício funcionou. Se ficou "a IA disse que...", volte à amostra — sem amostra, o output é opinião, não análise.

### Camada 4 — Metaprompt: deixe a IA montar o prompt (opcional · +10 min)

**Objetivo:** aprender o atalho pra quando você não quer preencher os 6 campos na mão — pede pra IA construir o prompt pra você a partir do seu objetivo.

**Como funciona:**
Cole no Claude o modelo abaixo. Ele vai te fazer as perguntas que faltam pra preencher cada elemento, e no fim entrega o prompt pronto — no mesmo padrão do gerador acima.

```text
Você é especialista em Engenharia de Prompt. Vou te dizer meu objetivo, e você vai criar
o prompt perfeito pra mim usando o framework PCTFL+CS (Papel, Contexto, Tarefa, Formato,
Limitações, Critério de Sucesso).

Antes de escrever o prompt final, me faça as perguntas que faltam pra preencher cada elemento.

Meu objetivo é: [descreva o que você quer].
```

**Quando usar cada um:**
- **Gerador da seção acima** — pra tarefa que você repete (fechamento mensal, briefing semanal). Reusa o padrão, muda só o contexto.
- **Metaprompt** — pra pedido novo ou complexo, onde você quer um primeiro rascunho rápido e depois refina.

**Resultado esperado:** 1 prompt gerado por metaprompt, executado, e sua leitura crítica de como a IA estruturou (aprendeu observando).

---

## Os 3 erros mais comuns

| Erro | Sintoma | Causa | Como corrigir |
|---|---|---|---|
| Avaliar por sensação | "Achei boa" — e o destinatário devolve com 4 perguntas | Critério de Sucesso ficou na cabeça, não no prompt | Escreva o critério antes do prompt: quem recebe, faz o quê, sem perguntar o quê |
| Pedir opinião em vez de estrutura | "O que você acha de X?" — resposta morna, dos dois lados | Delegar o julgamento em vez do preparo | Peça cenários, premissas, riscos, comparação por critério — e decida você |
| Reescrever em vez de refinar | Resposta 80% boa, você reescreve os 20% na mão, toda vez | Tratar cada resposta como final, não como iteração | Devolva na mesma conversa: "revise considerando [o que faltou]" — 2 iterações batem 1 reescrita |

---

> ⚠️ **Anti-alucinação — antes do briefing subir**
> - **Não deixe a IA inventar número que não está no seu relatório fonte.** As Limitações travam; o protocolo confere: fonte · número · consistência.
> - O briefing que sobe para a diretoria com número inventado não é erro da IA — **é erro seu, com o seu nome**. Revisão de conteúdo não é opcional em documento de decisão.
> - Caso-âncora: **Mata v. Avianca (2023)** — texto fluido, conteúdo fabricado, sanção real. O M4 traz o protocolo completo para você e para a sua equipe.

---

## Do prompt ao assistente persistente — o próximo passo

Você aprendeu a escrever um prompt PCTFL. O passo seguinte é transformá-lo em um **assistente persistente** — um parceiro especializado que já sabe quem você é e o que você faz, sem você re-explicar a cada nova conversa.

**Como funciona na prática:**
- Você abre o [Claude Projects](https://claude.ai/projects) (versão paga) e cria um projeto.
- Coloca lá o seu contexto fixo (seu cargo, sua área, suas normas de trabalho, exemplos do seu formato preferido).
- Toda conversa nova dentro do projeto já entra com esse contexto — você só descreve a tarefa do momento.

**Existe em outros ecossistemas:** o padrão é o mesmo. **GPTs personalizados** (ChatGPT) e **Gems** (Gemini) seguem a mesma lógica — você cria um assistente com contexto fixo, ele responde já sabendo quem é.

**Por que isso importa:** é o salto de "usei IA hoje" para "tenho IA no meu processo". Você deixa de operar com prompts isolados e passa a operar com assistentes especializados.

> 🔮 **No M5 você vai construir o seu.** A partir do prompt-âncora deste módulo, você monta um assistente que fica funcionando pra você — na sua conta, com o seu contexto. E como gestor, o salto seguinte é **arquitetar assistentes por área ou processo** — um pro fechamento, um pra triagem, um pra briefing — não só o seu individual. Este módulo prepara o método; o M5 prepara a ferramenta.

---

## Entregável do módulo

Ao final do M2, você sai com (marque conforme concluir):

- [ ] Rodei o prompt-âncora do módulo — como está — e li a resposta
- [ ] Adaptei o Contexto pra minha situação real (desidentificada) e rodei de novo
- [ ] Rodei um 3º prompt totalmente meu com PCTFL+ completo
- [ ] Apliquei o Critério de Sucesso na avaliação de pelo menos 1 resposta
- [ ] Salvei os 3 prompts (pré-preparo · âncora · advogado do diabo) pra próximo ciclo

---

> **Marco: o que você leva para a Mallory na 2ª feira**
> Até sexta-feira, gere com PCTFL avançado 1 documento real do seu cargo — briefing, síntese ou comunicado — e use de verdade: envie ou apresente a quem ele se destina.
> Como saber que aconteceu: o documento chegou ao destinatário, e o prompt está salvo para o próximo ciclo.

---

> **Como esses 3 prompts alimentam o Canvas Executivo (M6):** o Canvas Executivo do M6 tem uma linha "Como vou comunicar internamente e pra diretoria". Os 3 prompts que você salva hoje (síntese executiva · comunicado de liderança · análise de cenário) são exatamente a arquitetura de comunicação da sua iniciativa de IA — sem re-preparar cada peça, você chega no M6 com o time de comunicação pronto.

---

[← M1 · O Cenário Global de IA](../m1/) · [M3 · IA por Área →](../m3/)

[Banco de Prompts](../banco-de-prompts/) · [Artefatos](../artefatos/)
