# Lote de fornecedores

**M5 · Trilha 2 · Exemplos aplicados** · [voltar pra M5](../../)

> Delegue ao Cowork a leitura de 5 PDFs de cotação em formatos diferentes e receba uma tabela comparativa apple-to-apple com ranking em 3 critérios — o que no chat comum levaria um dia inteiro de leitura manual.

**Estação-âncora:** Cowork em batch · **Contexto:** Gestão · Suprimentos/Compras · fictício (treinamento)

---

## 1. Descreva a tarefa

Você é gestor de suprimentos e precisa escolher o fornecedor de um componente eletrônico de linha média. Cinco cotações chegaram em PDF, cada uma num formato diferente. Em vez de ler uma por uma, você delega a leitura do lote inteiro e pede a consolidação.

**Prompt-âncora (copie e cole no Cowork, com os 5 PDFs anexados):**

> Sou gestor de suprimentos numa indústria de eletroportáteis (contexto de treinamento). Preciso escolher fornecedor de um componente eletrônico de linha média. Cinco fornecedores mandaram cotação em PDF (anexadas), cada uma num formato diferente.
>
> (1) Leia os 5 PDFs — extraia dos anexos, não me peça pra colar conteúdo. (2) Monte uma tabela comparativa com: fornecedor, preço unitário (na moeda de origem, com conversão sinalizada), volume mínimo, prazo de entrega, condição de pagamento, garantia, certificações (ISO, RoHS, IATF…) e origem. Onde faltar dado, marque "não informado" — não chute. (3) Três observações qualitativas curtas por fornecedor, baseadas só no que você viu no PDF. (4) Ranking em 3 recortes: melhor preço (top 3, com % de diferença), melhor prazo (top 3) e melhor condição comercial global (ponderando preço + prazo + garantia — explique a ponderação). (5) Três perguntas que eu deveria fazer a cada fornecedor antes de fechar, com base nas omissões que você notou.
>
> Regras: você apresenta, quem decide sou eu (nada de "recomendo o fornecedor X"); se dois cotarem spec diferente, avise que pode não ser apple-to-apple; se algum PDF estiver ilegível ou parcial, avise qual. Português-BR, comercial direto.

## 2. Abra o Cowork e anexe as cotações

Abra o **Claude Cowork** (app de desktop) e anexe as cinco cotações (baixáveis na seção 6):

- `cotacao-fornecedor-A.pdf` até `cotacao-fornecedor-E.pdf` — 5 cotações fictícias

Os 5 vêm em formatos propositalmente diferentes — o cenário real de compras:

- **A** — bem estruturado, mas prazo longo.
- **B** — informal, o mais barato do lote, sem certificação declarada.
- **C** — prazo curto.
- **D** — importado, preço em USD (Shenzhen), conector ligeiramente diferente.
- **E** — nacional, com certificação IATF (automotiva).

## 3. O que o Claude entrega

Uma **tabela comparativa apple-to-apple** das 5 cotações (preço · prazo · pagamento · certificação · origem), **observações qualitativas** por fornecedor e **ranking em 3 recortes** — melhor preço, melhor prazo e melhor condição global (com a ponderação explicada). Campos ausentes viram "não informado" (ele não chuta) e conversões de moeda vêm sinalizadas. Não é "vencedor absoluto": é o material pra você decidir.

## 4. Continue a conversa

- **Repriorizar por prazo:** "Reponderando pra priorizar prazo curto (risco de linha parada), o que muda no ranking global?"
- **Gerar e-mails:** "Monta um e-mail curto pra cada fornecedor com as perguntas de esclarecimento que você levantou."
- **Simular câmbio:** "Simula câmbio +10% no fornecedor D e refaz só o ranking de preço."

## 5. Truques, dicas e ciladas

- **O lote vai numa passada.** O Cowork lê os 5 PDFs de uma vez; o chat comum te obrigaria a colar um por um.
- **"Não informado" é melhor que chute.** Exija que ele marque campos ausentes em vez de preencher com estimativa.
- **Apple-to-apple não é automático.** Peça que ele avise quando dois fornecedores cotam spec diferente (neste lote, o D tem conector diferente).
- **Preço é dado sensível.** Cotação real com preço que não pode vazar? Passe pelo Checklist de Anonimização do M4 antes de colar.

## 6. Pronto pra testar?

**Baixe:**
- [`cotacao-fornecedor-A.pdf`](../../../assets/exemplos/lote-fornecedores/cotacao-fornecedor-A.pdf) — estruturado · prazo longo
- [`cotacao-fornecedor-B.pdf`](../../../assets/exemplos/lote-fornecedores/cotacao-fornecedor-B.pdf) — informal · mais barato · sem certificação
- [`cotacao-fornecedor-C.pdf`](../../../assets/exemplos/lote-fornecedores/cotacao-fornecedor-C.pdf) — prazo curto
- [`cotacao-fornecedor-D.pdf`](../../../assets/exemplos/lote-fornecedores/cotacao-fornecedor-D.pdf) — importado · USD · Shenzhen
- [`cotacao-fornecedor-E.pdf`](../../../assets/exemplos/lote-fornecedores/cotacao-fornecedor-E.pdf) — nacional · certificação IATF
- [`prompt-lote-fornecedores.md`](../../../assets/exemplos/lote-fornecedores/prompt-lote-fornecedores.md) — prompt-âncora, colar no Cowork

**Passo a passo:**
1. Baixe os 6 arquivos (5 cotações + o prompt).
2. Abra o **Claude Cowork** (app de desktop).
3. Anexe as 5 cotações (`cotacao-fornecedor-A.pdf` até `E.pdf`).
4. Cole o conteúdo de `prompt-lote-fornecedores.md` (ou o prompt da seção 1).
5. Confira a tabela comparativa e o ranking nos 3 recortes.

---

**Outros casos:** [Destrave OEE](../destrave-oee/) · [Reunião trimestral](../reuniao-trimestral/) · [Análise de segmento](../analise-segmento/) · [Converse com sua planilha](../converse-planilha/) · [Comitê no Projects](../comite-sst-projects/)

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
