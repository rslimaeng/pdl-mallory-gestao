# Prepare a reunião trimestral

**M5 · Trilha 2 · Exemplos aplicados** · [voltar pra M5](../../)

> Delegue ao Cowork a leitura de 3 meses de Slack + a planilha de receita e receba um deck coeso de 7 slides + as perguntas difíceis da diretoria — sem ficar em alt-tab bloco por bloco.

**Estação-âncora:** Cowork + Connectors + Extended Thinking · **Contexto:** Gestão · Comercial regional · fictício (treinamento)

---

## 1. Descreva a tarefa

Você é gestor comercial regional e a reunião trimestral com a diretoria é terça — 45 minutos, 8 pessoas na sala. No chat comum você colaria o material bloco por bloco; no **Cowork** você delega: anexa o pacote extenso, descreve o que quer e deixa o Claude ler enquanto você toca outra coisa.

**Prompt-âncora (cole no Cowork, com os dois arquivos anexados):**

> Sou gestor comercial regional de uma indústria de eletroportáteis (contexto de treinamento). Preciso preparar a reunião trimestral com a diretoria — 45 minutos, 8 pessoas na sala, foco em performance do trimestre e o que muda no próximo.
>
> Anexei `slack-export-mock.md` (3 meses do canal #comercial-regional) e `receita-tri-mock.xlsx` (receita mensal por linha e região, últimos 4 trimestres).
>
> Entregue, usando Extended Thinking: (1) análise de receita — Q vigente vs Q anterior vs mesmo Q do ano anterior, linhas que puxaram pra cima e pra baixo com números, região que destoa; (2) síntese do Slack por temas (não lista de mensagens) — 3-5 assuntos recorrentes com frequência e se é reclamação/oportunidade/alerta; (3) cruzamento — os temas explicam os números? se não conecta, diga que não conecta; (4) deck de 7 slides em outline; (5) as 3 perguntas mais difíceis que a diretoria faria.
>
> Regras: nada de superlativo sem número; marque `[verificar antes da reunião]` em dado ambíguo; nomes do Slack já vieram anonimizados — avise se algum passou.

## 2. Dê contexto ao Claude

Abra o **Claude Cowork** (app desktop), ative **Extended Thinking** e anexe:

- `slack-export-mock.md` — 3 meses do canal #comercial-regional (~90 mensagens fictícias)
- `receita-tri-mock.xlsx` — receita mensal por linha e região, 4 trimestres

**Por que Cowork, e não o chat comum:** material desse tamanho no chat vira colagem em pedaços e você perde o fio. No Cowork ele lê o pacote inteiro, mantém tudo na cabeça e você acompanha o progresso sem alt-tab.

## 3. O que o Claude entrega

Um **deck de 7 slides** em outline (abertura, números, comparações, temas do Slack, cruzamento, 3 decisões, próximos passos), a **síntese do Slack por temas** e um bloco com as **3 perguntas difíceis da diretoria** pra você ensaiar. Copia pro Google Slides ou PowerPoint e ajusta a narrativa. Números fictícios do treinamento — o valor real está no cruzamento: onde a planilha confirma o que a equipe já sentia, e onde não conecta.

## 4. Continue a conversa

- **Enxugar:** "Enxuga o deck pra 5 slides mantendo as decisões e o cruzamento."
- **Script de fala:** "Escreve um script de fala de 45 segundos por slide."
- **Antecipar objeções:** "Antecipa as 3 objeções mais prováveis da diretoria e me dá resposta ancorada nos dados."

Cowork lê o material extenso enquanto você faz outra coisa; ele notifica quando o deck está pronto.

## 5. Truques, dicas e ciladas

- **Cowork existe justamente pra delegar leitura extensa.** No chat comum você colaria bloco por bloco e perderia o fio.
- **Slack real passa pelo Checklist M4 antes.** Os nomes do mock já vieram anonimizados; com export real, limpe nome, matrícula e cliente identificável você mesmo.
- **Peça a marca `[verificar antes da reunião]`** em qualquer dado ambíguo da planilha — você chega na sala sabendo o que ainda precisa confirmar.
- **Não force a narrativa.** O cruzamento números × temas só vale quando os dados de fato conectam; senão, o certo é ele dizer "não conecta".

## 6. Pronto pra testar?

**Baixe:**
- [`slack-export-mock.md`](../../../assets/exemplos/reuniao-trimestral/slack-export-mock.md) — 3 meses do canal #comercial-regional (~90 mensagens fictícias)
- [`receita-tri-mock.xlsx`](../../../assets/exemplos/reuniao-trimestral/receita-tri-mock.xlsx) — receita mensal por linha e região, 4 trimestres
- [`prompt-reuniao-tri.md`](../../../assets/exemplos/reuniao-trimestral/prompt-reuniao-tri.md) — o prompt completo pra colar no Cowork
- [`gabarito-deck.md`](../../../assets/exemplos/reuniao-trimestral/gabarito-deck.md) — referência pra conferir o output (não é resposta única)

**Passo a passo:**
1. Baixe os quatro arquivos.
2. Abra o **Claude Cowork** (app desktop).
3. Anexe `slack-export-mock.md` e `receita-tri-mock.xlsx`.
4. Ative o **Extended Thinking**.
5. Cole o conteúdo de `prompt-reuniao-tri.md` (mesmo prompt da seção 1).
6. Quando ele terminar, compare o deck com `gabarito-deck.md`.

---

**Outros casos:** [Comitê no Projects](../comite-sst-projects/) · [Destrave OEE](../destrave-oee/) · [Análise de segmento](../analise-segmento/) · [Converse com sua planilha](../converse-planilha/) · [Lote de fornecedores](../lote-fornecedores/)

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
