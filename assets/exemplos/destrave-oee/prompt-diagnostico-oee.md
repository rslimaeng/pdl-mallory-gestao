# Prompt · Destrave um tema técnico — OEE

> **Como usar:** ative **Extended Thinking** no Claude.ai (menu de configurações da conversa) e anexe `dados-oee-mock.xlsx`. Depois copie e cole o prompt abaixo.
>
> Este é o padrão "**mapear entendimento → destravar lacunas**": você descreve o que já sabe, Claude identifica onde tem confusão ou gap, e devolve um material que fecha as lacunas — não uma aula genérica sobre o tema.

---

Sou **gestor de produção** numa fábrica de eletroportáteis (contexto de treinamento). Preciso destravar meu entendimento sobre **OEE (Overall Equipment Effectiveness)** — ouço falar toda semana, olho os dashboards, mas ainda travo em alguns pontos e não quero fazer pergunta boba na reunião de sexta.

**O que eu já sei:**
- OEE mede quanto do potencial de uma máquina/linha está sendo usado.
- Tem três componentes: disponibilidade, performance e qualidade.
- Se multiplicar os três, dá um percentual.
- Meta "world-class" gira em torno de 85%.

**Onde eu trava:**
1. **Disponibilidade vs performance** — a diferença prática entre "a máquina não estava disponível" e "estava rodando devagar" fica nebulosa. Como classificar setup entre lotes? E micro-paradas de 30 segundos que ninguém aponta?
2. **Qualidade** — entra só refugo/rework, ou também "peça boa fora do padrão que virou boa depois de retrabalho fora de linha"?
3. **Denominador do cálculo** — uso tempo total do turno, tempo planejado de produção, ou tempo disponível descontando manutenção preventiva agendada? Cada consultor fala diferente.
4. **Comparabilidade entre máquinas** — dá pra comparar OEE de uma injetora (ciclos longos) com o de uma montagem manual (ciclos curtos)? Ou é maçã com laranja?

**O que preciso de você:**

Antes de me dar a resposta, **use extended thinking pra mapear meus mal-entendidos**. Pega minhas 4 travas, identifica quais são de definição, quais são de método e quais são de convenção da indústria (onde existe mais de uma escola).

Depois, com base nos dados da planilha anexada (`dados-oee-mock.xlsx` · dados fictícios de 3 turnos × 5 dias × 2 máquinas), me devolve:

1. **Um workbook curto** (2-3 páginas, formato artifact editável) que:
   - Define cada componente (disponibilidade, performance, qualidade) com uma frase e um exemplo tirado da planilha.
   - Resolve minhas 4 travas específicas, uma por uma, apontando onde a resposta é "verdade universal" e onde é "convenção da casa".
   - Mostra o cálculo do OEE de UMA das máquinas usando os dados anexados — passo a passo, com números reais.
2. **Uma tabela de decisão** — quando classificar um tempo perdido como cada tipo (parada, redução de ritmo, refugo).
3. **3 perguntas que EU deveria fazer** ao meu time de PCP na próxima reunião pra alinhar convenções da casa antes de sair medindo.

Não me dá aula histórica sobre origens do OEE. Vai direto no que destrava.

---

*Prompt versão 1.0 · PDL Mallory 2026 · M5 T2 · Caso 2*
