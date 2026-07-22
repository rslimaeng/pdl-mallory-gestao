# Análise de segmento bottom-up

**M5 · Trilha 2 · Exemplos aplicados** · [voltar pra M5](../../)

> Dimensione um mercado novo com metodologia auditável — TAM/SAM/SOM construído de baixo pra cima, com toda fonte citada, não um número redondo puxado de relatório de terceiro.

**Estação-âncora:** Cowork + Extended Thinking · **Contexto:** Gestão · Portfólio/Estratégia · fictício (treinamento)

---

## 1. Descreva a tarefa

Você é gestor de portfólio numa indústria de eletroportáteis. A diretoria pediu o tamanho de um mercado novo pra decidir se vale entrar — e não aceita "achamos que dá R$ X". Precisa de método: cada número construído de baixo pra cima, com a fonte ao lado. Segmento hipotético em análise: eletroportáteis para cozinha profissional de pequeno porte — cafeterias, padarias artesanais e bistrôs (não hotelaria industrial). Brasil, mercado B2B. Tudo fictício, contexto de treinamento.

**Prompt-âncora (abra o Cowork com Extended Thinking e cole):**

> Sou gestor de portfólio numa indústria de eletroportáteis (contexto de treinamento). A diretoria pediu uma análise de tamanho de mercado pra um novo segmento hipotético: eletroportáteis para cozinha profissional de pequeno porte — cafeterias, padarias artesanais e bistrôs (não hotelaria industrial). Brasil, mercado B2B. Precisamos decidir se vale entrar, e não posso levar "achamos que dá R$ X" — precisa ter metodologia.
>
> Usando Extended Thinking pra pensar antes de calcular:
>
> 1. **Framework:** aplique TAM · SAM · SOM bottom-up (não top-down). TAM = universo total de compradores no Brasil; SAM = subconjunto que a Mallory endereça dado canal, preço e capacidade; SOM = fatia realista nos primeiros 24 meses.
> 2. **Bottom-up de verdade:** quantas cafeterias, padarias artesanais e bistrôs operam no Brasil (estimativas públicas — SEBRAE, ABIC, IBGE), quanto cada uma gasta por ano em eletroportáteis, e multiplica. Todas as fontes citadas; se chutou, marca [estimativa não verificada].
> 3. **Preenche a planilha** `gabarito-metodologia-tam-sam-som.xlsx` (células em branco, headers montados): cada célula com o número + na coluna ao lado a fonte ou a premissa.
> 4. **Sensibilidade:** 3 cenários (otimista / base / pessimista) numa tabela comparando o SOM final.
> 5. **Sumário executivo** em outline: pergunta, método (2 linhas), resultado principal (SOM base + faixa), 3 premissas mais frágeis, recomendação (entrar / não entrar / pilotar / investigar), 3 dados que ainda faltam.
>
> Regras: nunca invente número (se não sabe, [estimativa a validar]); só fontes públicas — nada de relatório proprietário; faixa > ponto (R$ 40–60M > R$ 50M); dado que só a Mallory tem (capacidade produtiva, ticket médio) marca [buscar internamente] — não chuta.

## 2. Dê contexto ao Claude

Abra o **Claude Cowork** (app desktop), ative o **Extended Thinking** e anexe:

- `gabarito-metodologia-tam-sam-som.xlsx` — planilha modelo: células em branco, headers já montados (TAM/SAM/SOM, coluna de valor, coluna de fonte/premissa)

**Opcional:** dados internos da Mallory *já validados* (capacidade produtiva atual, ticket médio). Sem eles, o Claude marca cada célula que depende desses números como `[buscar internamente]` — não chuta capacidade nem ticket.

## 3. O que o Claude entrega

A planilha preenchida célula a célula — cada número com a **fonte ou premissa** ao lado — mais **3 cenários de SOM** (otimista/base/pessimista) e um **sumário executivo** pronto pra diretoria (pergunta, método, resultado com faixa, 3 premissas frágeis, recomendação entrar/pilotar/investigar). Onde ele chutou, sinaliza `[estimativa não verificada]`; onde falta dado interno, marca `[buscar internamente]`. Você audita: toda linha tem fonte pública ou premissa explicada — nenhum número redondo apareceu do nada.

## 4. Continue a conversa

- **Muda o canal:** "Refaz o SOM assumindo canal só distribuidor (sem venda direta) — quanto muda?"
- **Isola as alavancas:** "Lista as 3 premissas que mais movem o resultado e a faixa de cada uma."
- **Versão cética:** "Escreve a versão 'não entrar ainda' da recomendação, com os 3 dados que faltam pra decidir."

## 5. Truques, dicas e ciladas

- **Bottom-up não é top-down disfarçado.** Exija a multiplicação a partir de unidades reais, com fonte. Se a resposta começa com "o mercado é R$ X, assumimos Y%", devolva.
- **Chute marcado e faixa em vez de ponto.** Peça `[estimativa não verificada]` em todo número sem fonte pública e faixa no lugar de ponto (R$ 40–60M > R$ 50M).
- **Só fontes públicas** (SEBRAE, IBGE, ABIC) — nada de relatório proprietário que vocês não têm acesso.
- **Dado que só a Mallory tem vira `[buscar internamente]`** — não deixe o Claude chutar capacidade ou ticket.

## 6. Pronto pra testar?

**Baixe:**
- [`gabarito-metodologia-tam-sam-som.xlsx`](../../../assets/exemplos/analise-segmento/gabarito-metodologia-tam-sam-som.xlsx) — planilha modelo, células em branco
- [`prompt-analise-segmento.md`](../../../assets/exemplos/analise-segmento/prompt-analise-segmento.md) — prompt completo, colar no Cowork

**Passo a passo:**
1. Baixe os dois arquivos.
2. Abra o **Claude Cowork** (app desktop) e anexe `gabarito-metodologia-tam-sam-som.xlsx`.
3. Ative o **Extended Thinking**.
4. Cole o conteúdo de `prompt-analise-segmento.md` no chat.
5. Ao receber a planilha, confira se cada célula tem uma fonte ou premissa ao lado — e se os chutes estão marcados.

---

**Outros casos:** [Comitê no Projects](../comite-sst-projects/) · [Destrave OEE](../destrave-oee/) · [Reunião trimestral](../reuniao-trimestral/) · [Converse com sua planilha](../converse-planilha/) · [Lote de fornecedores](../lote-fornecedores/)

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
