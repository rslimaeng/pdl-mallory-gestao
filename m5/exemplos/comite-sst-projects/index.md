# Comitê no Projects — SST/Qualidade

**M5 · Trilha 2 · Exemplos aplicados** · [voltar pra M5](../../)

> Monte um espaço persistente no Claude Projects para preparar pauta, redigir ata e comunicar decisões do comitê semanal — sem começar do zero toda semana e sem depender de quem está de plantão.

**Estação-âncora:** Projects + Artifacts · **Contexto:** Gestão · SST/Qualidade · fictício (treinamento)

---

## 1. Descreva a tarefa

O Claude no Projects mantém o mesmo contexto ativo entre conversas — política interna, atas passadas, papéis do comitê. Cada semana você só descreve o que aconteceu; ele reusa tudo o que já sabe.

**Prompt-âncora (copie e cole numa conversa dentro do Project):**

> Estou preparando o comitê SST/Qualidade desta semana. Aconteceram três coisas desde a última reunião: (1) um quase-acidente no setor de injeção (colaborador escorregou em óleo derramado, sem lesão); (2) reclamação recorrente sobre EPI (luvas com furo relatadas por 4 pessoas em turnos diferentes); (3) auditoria externa marcada pra próximo mês.
>
> Com base na política interna que está no Project e nas 4 atas anteriores, prepara pra mim: pauta com 5 tópicos priorizados por criticidade, minuta de ata com espaços pra preencher no dia, e comunicado curto pra chão de fábrica em linguagem direta (sem jargão técnico).

## 2. Dê contexto ao Claude

Ative o **Claude Projects**, crie um projeto "Comitê SST · Qualidade" e anexe:

- `politica-sst-mallory-mock.docx` — política interna fictícia (11 páginas)
- `instrucoes-projeto-comite-sst.md` — cole no campo **Instructions** do Project

**Opcional:** atas antigas *já anonimizadas* (Checklist M4). Quanto mais atas, mais o Claude aprende o estilo da casa.

## 3. O que o Claude entrega

Um artifact com três peças usáveis direto: **pauta priorizada** (5 tópicos por criticidade), **minuta de ata** pronta pra preencher no dia, e **comunicado curto** pro chão de fábrica. Editável ao vivo no Claude ou copiável pro Word. As peças ficam versionadas no Project.

## 4. Continue a conversa

- **Refinar linguagem:** "Reescreve o comunicado pro colaborador do turno da noite, sem termos técnicos, máximo 3 linhas."
- **Consolidar histórico:** "Pega as 4 últimas atas e faz um relatório trimestral: recorrências, decisões que viraram fato, pendências."
- **Propor indicadores:** "Baseado nos últimos 3 meses de atas, sugere 3 KPIs de SST/Qualidade mensuráveis com o que a Mallory já coleta."

## 5. Truques, dicas e ciladas

- **As instruções do Project valem mais que qualquer prompt.** Escreva a moldura uma vez; todo prompt novo herda.
- **Anonimize antes de anexar ata real** (Checklist M4). A IA nunca faz essa limpeza; você faz.
- **Um Project por comitê, não um Project pra tudo.** Contexto demais compete e degrada a resposta.
- **Reveja as instruções a cada trimestre.** Instruções velhas empurram o Claude pra respostas velhas.

## 6. Pronto pra testar?

**Baixe:**
- [`politica-sst-mallory-mock.docx`](../../../assets/exemplos/comite-sst-projects/politica-sst-mallory-mock.docx) — política fictícia, anexar no Project
- [`instrucoes-projeto-comite-sst.md`](../../../assets/exemplos/comite-sst-projects/instrucoes-projeto-comite-sst.md) — colar em Project → Instructions

**Passo a passo (5 min):**
1. Baixe os dois arquivos.
2. Claude.ai → **Projects → + New Project**, nomeie "Comitê SST · Qualidade".
3. Cole `instrucoes-projeto-comite-sst.md` no campo **Instructions**.
4. Anexe `politica-sst-mallory-mock.docx` em **Project knowledge**.
5. Abra uma conversa nova no projeto e cole o prompt da seção 1.

---

**Outros casos:** [Destrave OEE](../destrave-oee/) · [Reunião trimestral](../reuniao-trimestral/) · [Análise de segmento](../analise-segmento/) · [Converse com sua planilha](../converse-planilha/) · [Lote de fornecedores](../lote-fornecedores/)

*PDL 2026 · Mallory Eletroportáteis · Trilha 2 · Instrutor Rafael Lima ([@iacomrafael](https://www.instagram.com/iacomrafael/))*
