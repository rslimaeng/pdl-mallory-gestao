# Destrave um tema técnico — OEE

**M5 · Trilha 2 · Exemplos aplicados** · [voltar pra M5](../../)

> Descreva o que você já entende de OEE; o Claude usa Extended Thinking pra mapear onde você trava e devolve um workbook que fecha só as lacunas — não uma aula genérica sobre o tema.

**Estação-âncora:** Extended Thinking + Artifacts · **Contexto:** Gestão · Produção/Lean · fictício (treinamento)

---

## 1. Descreva a tarefa

Você é gestor de produção e quer destravar seu entendimento de OEE antes da reunião de sexta. O truque não é pedir uma aula: é descrever o que você já sabe e onde trava, ativar o Extended Thinking e deixar o Claude raciocinar sobre suas confusões antes de responder.

**Prompt-âncora (copie e cole numa conversa com Extended Thinking ativado):**

> Sou gestor de produção numa fábrica de eletroportáteis (treinamento). Preciso destravar meu entendimento de OEE antes da reunião de sexta. Já sei o básico — mede quanto do potencial da máquina está sendo usado, tem três componentes (disponibilidade × performance × qualidade), meta world-class ~85%. Mas travo em quatro pontos: (1) disponibilidade vs performance — onde entra setup entre lotes e micro-parada de 30s que ninguém aponta; (2) qualidade — só refugo/rework ou também peça que virou boa após retrabalho fora de linha; (3) denominador — tempo total do turno, tempo planejado ou tempo disponível descontando preventiva agendada; (4) comparabilidade — dá pra comparar injetora (ciclo longo) com montagem manual (ciclo curto).
>
> Antes de responder, usa extended thinking pra mapear meus mal-entendidos — separa o que é definição, método e convenção da indústria. Depois, com os dados de `dados-oee-mock.xlsx`, me devolve: um workbook de 2-3 páginas (artifact editável) que define os 3 componentes com exemplo da planilha, resolve minhas 4 travas marcando "verdade universal" vs "convenção da casa" e mostra o cálculo do OEE de UMA máquina passo a passo; uma tabela de decisão (parada × redução de ritmo × refugo); e 3 perguntas que eu deveria levar ao PCP. Não me dá aula histórica sobre a origem do OEE — vai direto no que destrava.

## 2. Dê contexto ao Claude

Duas coisas fazem o caso funcionar:

- Ative o **Extended Thinking** no menu de configurações da conversa — dá espaço pro Claude raciocinar antes de escrever.
- Anexe `dados-oee-mock.xlsx` — dados fictícios de 3 turnos × 5 dias × 2 máquinas.

**Opcional:** se sua casa tem uma definição interna de como calcula OEE (qual denominador usa, o que conta como refugo), cole junto. Vira a "convenção da casa" que o Claude separa da "verdade universal".

## 3. O que o Claude entrega

Um **workbook** (artifact editável) que resolve as SUAS quatro travas com os números da planilha — não uma explicação genérica. Define os 3 componentes com exemplo, resolve cada trava marcando **verdade universal** vs **convenção da casa**, e mostra o cálculo de uma máquina passo a passo (ex.: Injetora L3 · turno A → Disp 88% × Perf 91% × Qual 89% ≈ **OEE 71,3%**). Fecha com uma **tabela de decisão** (parada × ritmo × refugo) e **3 perguntas pro PCP**.

## 4. Continue a conversa

- **Comparar máquinas:** "Refaz o cálculo pra a montagem manual e compara com a injetora — ciclos curtos vs longos mudam a leitura?"
- **Virar checklist:** "Transforma a tabela de decisão num checklist de 1 página pra imprimir na linha."
- **Caçar distorção:** "Lista os 3 erros de apontamento mais comuns que inflam OEE artificialmente."

**Padrão de uso:** mapear entendimento → destravar lacunas. Vale pra qualquer tema técnico que você "quase" domina (Takt time, MTBF, capabilidade de processo).

## 5. Truques, dicas e ciladas

- **Extended Thinking custa alguns segundos a mais** — vale exatamente onde você tem lacuna. Pra tarefa simples é overkill; pra destravar confusão conceitual, ligue.
- **Peça pra ele separar verdade universal de convenção da casa.** OEE tem mais de uma escola; sem a marcação você mede com uma convenção que o PCP nunca combinou.
- **Valide as convenções com o PCP antes de sair medindo.** O workbook já levanta as perguntas certas — leve-as pra reunião.
- **Dado real de produção é sensível.** Se for anexar apontamento real (não o mock), passe pelo Checklist de Anonimização do M4 antes. A IA nunca faz essa limpeza; você faz.

## 6. Pronto pra testar?

**Baixe:**
- [`dados-oee-mock.xlsx`](../../../assets/exemplos/destrave-oee/dados-oee-mock.xlsx) — dados fictícios, 3 turnos × 5 dias × 2 máquinas
- [`prompt-diagnostico-oee.md`](../../../assets/exemplos/destrave-oee/prompt-diagnostico-oee.md) — prompt pronto, copiar e colar

**Passo a passo (5 min):**
1. Baixe os dois arquivos.
2. Abra o **Claude.ai** e comece uma conversa nova.
3. No menu de configurações da conversa, ative o **Extended Thinking**.
4. Anexe `dados-oee-mock.xlsx`.
5. Cole o conteúdo de `prompt-diagnostico-oee.md`. Veja o Claude mapear suas travas antes de responder.

---

**Outros casos:** [Comitê no Projects](../comite-sst-projects/) · [Reunião trimestral](../reuniao-trimestral/) · [Análise de segmento](../analise-segmento/) · [Converse com sua planilha](../converse-planilha/) · [Lote de fornecedores](../lote-fornecedores/)

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
