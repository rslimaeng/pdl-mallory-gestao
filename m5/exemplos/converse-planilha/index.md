# Converse com sua planilha

**M5 · Trilha 2 · Exemplos aplicados** · [voltar pra M5](../../)

> Antes de pedir dashboard bonito, converse com os dados — o Claude faz sanity check, sugere o que a planilha responde bem (e o que não responde) e só renderiza gráfico em artifact quando você pedir.

**Estação-âncora:** Artifacts + Chat · **Contexto:** Gestão · Comercial · fictício (treinamento)

---

## 1. Descreva a tarefa

Você é gestor comercial e recebeu do PCP uma planilha com produção e venda mensal dos últimos 12 meses de 6 SKUs. Antes de pedir dashboard bonito pro time de dados, quer entender o que esses números contam. Este é o caso mais simples do módulo — roda no **Chat** do Claude.ai, não precisa de Cowork.

**Prompt-âncora (anexe a planilha e cole numa conversa nova):**

> Sou gestor comercial numa indústria de eletroportáteis (contexto de treinamento). Recebi uma planilha do PCP com produção e venda mensal dos últimos 12 meses de 6 SKUs e quero entender o que ela me conta antes de pedir dashboard. Antes de qualquer gráfico, na ordem: (1) sanity check — quantas linhas e colunas, alguma célula em branco ou com valor esquisito, os totais mensais batem? Se tiver problema, para e me avisa. (2) 3 perguntas que essa planilha responde bem — específicas destes dados (ex.: quais SKUs têm venda maior que produção há 2+ meses seguidos?). (3) 3 perguntas que ela NÃO responde — onde é cega (ex.: não separa canal, então não dá pra saber se a queda foi B2B ou B2C). (4) Depois eu faço perguntas específicas: responde com número direto, fonte (qual coluna, qual linha) e declara quando depender de suposição. Só quando eu pedir, renderiza gráfico em artifact. Regras: nunca inventa coluna, nunca arredonda pra ficar bonito, marca hipótese como hipótese, português-BR e sem emoji.

## 2. Dê contexto ao Claude

Sem configuração extra. Abra o **Claude.ai** (Chat comum, sem Cowork), anexe o arquivo pelo clipe de anexo e cole o prompt:

- `dados-producao-venda-mock.xlsx` — produção e venda mensal fictícia de 6 SKUs em 12 meses

Não precisa de Project, Connector nem Cowork. É o exemplo mais leve do módulo — de propósito, pra fixar o hábito de *conversar antes de visualizar* sem fricção de setup.

## 3. O que o Claude entrega

Nenhum gráfico ainda — de propósito. Primeiro o **sanity check** (12 linhas de mês × colunas de produção e venda por SKU; totais mensais batem; 1 célula sinalizada — venda em branco num mês, confirmar se é zero real ou dado faltando). Depois **3 perguntas que a planilha responde bem** (ex.: quais SKUs têm venda > produção por 2+ meses seguidos = risco de ruptura) e **3 que ela NÃO responde** (ex.: não separa canal B2B/B2C; não tem preço nem margem). Cada afirmação vem com a fonte. O gráfico só aparece quando você pede.

## 4. Continue a conversa

- **Perguntar em texto:** "Quais SKUs tiveram venda maior que produção por 2+ meses seguidos? Lista com os meses."
- **Pedir o gráfico:** "Agora renderiza um gráfico de linha produção vs venda do SKU de café em artifact."
- **Puxar leitura pro PCP:** "Qual SKU tem maior volatilidade mês a mês e o que isso sugere pro planejamento do PCP?"

Converse antes de visualizar: o Claude ajuda a decidir o que faz sentido plotar, aí sim o Artifacts renderiza.

## 5. Truques, dicas e ciladas

- **Peça sempre a fonte** (qual coluna, qual linha) — pra você conseguir auditar o número.
- **Hipótese não é fato:** quando ele explica um "por que caiu", exija que marque como hipótese.
- **Ele nunca inventa coluna nem arredonda pra ficar bonito** — o número é o que a planilha tem.
- **Planilha de venda real?** Passe pelo Checklist de Anonimização do M4 antes de colar. A IA nunca faz essa limpeza; você faz.

## 6. Pronto pra testar?

**Baixe:**
- [`dados-producao-venda-mock.xlsx`](../../../assets/exemplos/converse-planilha/dados-producao-venda-mock.xlsx) — produção × venda de 6 SKUs em 12 meses, fictício
- [`prompt-converse-planilha.md`](../../../assets/exemplos/converse-planilha/prompt-converse-planilha.md) — prompt completo, colar na conversa

**Passo a passo (2 min):**
1. Baixe os dois arquivos.
2. Abra o **Claude.ai** e comece uma conversa nova (Chat comum, sem Cowork).
3. Anexe `dados-producao-venda-mock.xlsx` pelo clipe de anexo.
4. Cole o conteúdo de `prompt-converse-planilha.md` e envie.
5. Leia o sanity check e o mapa. **Só peça gráfico depois** de entender o que os dados respondem.

---

**Outros casos:** [Destrave OEE](../destrave-oee/) · [Reunião trimestral](../reuniao-trimestral/) · [Análise de segmento](../analise-segmento/) · [Comitê no Projects](../comite-sst-projects/) · [Lote de fornecedores](../lote-fornecedores/)

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
