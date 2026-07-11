# Banco de Prompts · Trilha 2 — Gestão

**A biblioteca de prompts do gestor.** Copie o da sua situação, cole no Claude, troque o que está `[entre colchetes]` por dados desidentificados da sua área — e avalie a resposta contra o Critério de Sucesso, não contra "achei bom".

[← Início](../) · [M1](../m1/) · [M2](../m2/) · [M3](../m3/) · [M4](../m4/) · [M5](../m5/) · [M6](../m6/) · [Artefatos](../artefatos/)

---

## Como usar este banco

**PCTFL avançado em 30 segundos:**

- **P**apel — quem a IA deve ser (nível e vocabulário da resposta)
- **C**ontexto — a situação da sua área, com números desidentificados
- **T**arefa — o que fazer, com verbo de gestão: analise, compare, estruture, redija
- **F**ormato — o entregável: 1 página, tabela, blocos definidos
- **L**imitações — o que não fazer, começando pela regra de ouro: *"Se faltar informação, pergunte. Não invente."*
- **# CRITÉRIO DE SUCESSO** — como você saberá que cumpriu: *"a resposta funciona se [destinatário] conseguir [ação] sem pedir esclarecimento"*
- **# CRITÉRIO NEGATIVO** — o que a resposta não pode ser: tom, formato, conteúdo proibido

**O protocolo de 3 passos (M4) — em toda resposta que vira documento:**

1. **Fonte** — cada fato veio do que foi enviado?
2. **Número** — todo número, data, cláusula e norma, conferidos na origem
3. **Consistência** — bate com o que a área sabe? Estranhou, checou.

**As 5 categorias que nunca entram em ferramenta externa:**

**gente** · **produto** · **contrato** · **diretoria** · **concorrência** — a lista detalhada está no [M4](../m4/). Se vazasse, quem daria explicação é você? Então não entra.

**Prompt bom é ativo da área:** escreve uma vez, reusa o ano inteiro. Salve os seus melhores, versione quando melhorar, compartilhe com a equipe — biblioteca de prompts é patrimônio da área, não truque pessoal.

---

## Os 6 prompts dos módulos

Os mesmos que você executou em sala — na íntegra.

### M1 · Mapeamento inicial da minha área

**Área:** todas — o ponto de partida da hipótese executiva
**Para quando:** você quer saber, com critério, quais rotinas da sua área a IA alcança nos próximos 12 meses — e onde começar.
**Você leva:** tabela com cada rotina classificada nos 3 modos de uso da IA + as 2 rotinas recomendadas para os próximos 90 dias, com justificativa executiva.

```text
# PAPEL
Você é um consultor sênior de transformação com IA em indústria de manufatura,
com 10+ anos ajudando gestores a decidir onde a IA rende de verdade —
sem hype e sem propostas que dependem de projeto de TI.

# CONTEXTO
Sou gestor da área de [sua área] em uma fabricante de eletroportáteis
(linha branca — liquidificador, air fryer, ventilador, batedeira). Estrutura
da empresa: certificação ISO 9001, ERP Datasul, processos documentados,
equipe de [tamanho] pessoas reportando a mim. Ferramentas de IA aprovadas
pelo TI: Claude e ChatGPT em versão paga (conta corporativa quando homologada,
conta pessoal Pro por conta e risco enquanto isso).

Minhas rotinas que mais consomem tempo de gestão:
[liste 3-5 rotinas reais — exemplos comuns em gestão industrial:
- Análise mensal de desvios orçamentários da área
- Preparação de reunião mensal de diretoria (briefing + material)
- Triagem inicial de contratos de fornecedores
- Consolidação de indicadores da área para o comitê S&OP
- Leitura e resposta de e-mails complexos com stakeholders internos
- Redação de comunicados corporativos com múltiplas versões (diretoria, gestores, chão)
- Análise de pesquisas de clima e feedbacks para plano de ação]

# TAREFA
Classifique cada rotina em um dos 3 modos oficiais de uso da IA — use estas
definições exatas, elas são o vocabulário do treinamento:

- Autopiloto: rotina que segue sempre o mesmo padrão. Você define uma vez, a IA
  executa, você revisa. Baixo risco, alto ganho de tempo. Ex.: transformar
  reunião gravada em ata estruturada.

- Colaboração: rotina que precisa do seu contexto e julgamento estratégico. A IA
  rascunha e propõe cenários; você conduz e decide. Ganho em qualidade da decisão
  + velocidade. Ex.: estruturar cenários de negociação com fornecedor.

- Manual: decisão de alta responsabilidade autoral, com impacto em pessoa, contrato
  ou posicionamento executivo. A IA no máximo inspira; você decide sem delegar.
  Ex.: decisão de demissão, aprovação de investimento, parecer para a diretoria.

Para cada rotina: classificação + ganho estimado de tempo (horas/mês) +
facilidade de começar (1-5, sendo 5 = "posso testar amanhã com a conta atual").
Encerre com as 2 recomendadas para os próximos 90 dias e o porquê executivo.

# FORMATO
Tabela: Rotina | Modo (Autopiloto/Colaboração/Manual) | Ganho estimado (h/mês) |
Facilidade (1-5) | Justificativa (1 linha).

Depois da tabela: parágrafo final de 3-4 linhas com as 2 rotinas top-priorizadas
para 90 dias, e por que essas — não outras.

# LIMITAÇÕES
Se faltar informação sobre alguma rotina, pergunte antes de classificar. Não invente.
Não proponha nada que dependa de comprar sistema, contratar consultor ou aprovar
orçamento — só o que rende com Claude/ChatGPT versão paga já disponível.
Não classifique como Autopiloto rotina que envolve dado sensível (as 5 categorias
do M4: gente, produto, contrato, diretoria, concorrência) sem processo de
desidentificação prévia — nesses casos, marque como Colaboração com ressalva.

# CRITÉRIO DE SUCESSO
Ao final, eu consigo defender minha lista de 2 top-prioridades diante do meu
diretor com 3 argumentos por rotina — ganho mensurável, risco controlado,
factibilidade nos próximos 90 dias.

# CRITÉRIO NEGATIVO
Não use jargão de consultoria ("sinergia", "transformação digital",
"pipeline de ideação"). Não sugira "criar comitê de IA" — a decisão é minha
como gestor. Não classifique tudo como Colaboração pra ficar seguro —
a força do mapa está em separar Autopiloto de Colaboração com clareza.
```

**Como avaliar:** você defenderia essas 2 top-prioridades numa reunião com seu diretor semana que vem? Consegue nomear 1 risco de cada e como mitiga? Passou. Se ficou tudo Colaboração, a IA jogou seguro — refaça o CONTEXTO com rotinas mais operacionais no meio, pra forçar o Autopiloto aparecer.

### M2 · Briefing de desvios orçamentários

**Área:** Controladoria / Financeiro
**Para quando:** o comitê é quinta-feira e o relatório de 30 páginas precisa virar 1 página com decisão.
**Você leva:** briefing que separa desvio estrutural de pontual e fecha com o que exige decisão da diretoria.

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

**Como avaliar:** contra o Critério de Sucesso — a diretoria decidiria sem abrir o relatório completo? Troque o CONTEXTO pelos seus números desidentificados; o resto é reuso.

### M3 · Uma fonte, N narrativas (pesquisa de clima)

**Área:** RH / Gestão de Pessoas — o padrão serve para qualquer resultado que vai a públicos diferentes
**Para quando:** o mesmo resultado precisa chegar à diretoria, aos gestores e à fábrica — cada um na sua língua.
**Você leva:** 3 comunicações do mesmo dado, cada uma dizendo ao seu público o que fazer.

```text
# PAPEL
Você é um consultor de comunicação organizacional com experiência em indústria.

# CONTEXTO
Sou Gerente de Gente de uma fabricante de eletroportáteis (400+ funcionários, fábrica
e escritório). Resultado FICTÍCIO da pesquisa de clima: participação 78% · orgulho de
trabalhar na empresa 82% · comunicação interna 54% (pior dimensão, queda de 8 pontos) ·
relação com liderança direta 71% · principais comentários abertos citam "decisões
demoram a chegar ao chão de fábrica" e "mudanças são comunicadas em cima da hora".

# TAREFA
Redija 3 comunicações do mesmo resultado, uma para cada público: diretoria (análise
e proposta), gestores (o que fazer diferente), fábrica (transparência e próximos passos).

# FORMATO
Diretoria: 1 página com números, diagnóstico e 2 ações propostas. Gestores: 10 linhas
com as 3 práticas que mudam. Fábrica: 8 linhas em linguagem direta, sem número técnico,
com 1 compromisso concreto.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Use apenas os dados do contexto — não crie estatística nem citação nova.

# CRITÉRIO DE SUCESSO
Cada público entende o que o resultado significa para ele e o que acontece agora —
sem precisar ler a versão dos outros.

# CRITÉRIO NEGATIVO
A versão da fábrica não pode soar defensiva nem burocrática. Nenhuma versão promete
o que não está nas 2 ações propostas.
```

**Como avaliar:** leia a versão da fábrica em voz alta — soa como comunicado que você mandaria? O padrão vale para resultado do mês, mudança de processo, qualquer "1 fonte, N públicos".

### M4 · Revisão de contrato de fornecedor

**Área:** Jurídico — e todo gestor que assina renovação
**Para quando:** a renovação se aproxima e as cláusulas de risco precisam estar na mesa antes da conversa.
**Você leva:** tabela de cláusulas classificadas por risco e os pontos que exigem parecer do jurídico.

```text
# PAPEL
Você é um analista de contratos sênior com experiência em fornecedores industriais.

# CONTEXTO
Contrato FICTÍCIO de fornecimento de componentes plásticos, resumo das cláusulas:
- Vigência 24 meses, renovação automática por igual período se não houver aviso em 90 dias
- Reajuste anual pelo IGP-M, sem teto
- Multa por atraso de entrega: 0,5% por dia, limitada a 10% do pedido
- Rescisão por qualquer parte com aviso de 30 dias, sem multa após 12 meses
- Exclusividade de fornecimento do componente X durante a vigência

# TAREFA
Identifique as cláusulas de risco para a contratante, classifique cada uma
(alto / médio / baixo) e aponte o que negociar antes da renovação.

# FORMATO
Tabela: Cláusula | Risco | Por quê | O que negociar. Fechamento com os 2 pontos
que exigem parecer do jurídico antes de qualquer ação.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não cite cláusula que não está no contexto. Não emita parecer jurídico — sinalize
o que precisa de validação do jurídico.

# CRITÉRIO DE SUCESSO
A gestora identifica os pontos de risco e sabe o que levar ao jurídico —
sem tratar esta análise como parecer final.

# CRITÉRIO NEGATIVO
A resposta não pode interpretar além do texto nem sugerir ação jurídica definitiva.
Sem juridiquês não traduzido.
```

**Como avaliar:** a análise é preparação, não parecer — os 2 pontos finais chegaram ao jurídico? No uso real, o contrato entra **desidentificado** e a regra das 5 categorias vale integralmente.

### M5 · CLAUDE.md base da workstation

**Área:** todas — é o artefato central do Cowork
**Para quando:** montar a memória permanente da sua workstation: quem é a área, tom, o que sempre e nunca fazer.
**Você leva:** o arquivo que faz a workstation falar a língua da sua área em toda sessão.

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

**Como avaliar:** cabe em 1 página e responde quem é a área, tom, o que sempre/nunca fazer? As duas regras de ouro do M5: **enxuto** (até ~300 linhas, apontando para arquivos de referência) e **limpo** (nenhum dado das 5 categorias dentro dele).

### M6 · Argumentação de 3 frases para diretoria

**Área:** todas — fecha o Canvas Executivo
**Para quando:** o Canvas está preenchido e a proposta precisa caber em 2 minutos de fala com resposta pronta para as objeções.
**Você leva:** as 3 frases prontas para falar e as respostas às perguntas prováveis da diretoria.

```text
# PAPEL
Você é um assessor executivo experiente em preparar propostas para diretoria industrial.

# CONTEXTO
Sou gestor de [área] e vou propor um piloto de IA de 30 dias. Meu Canvas:
- Oportunidade: [a rotina, em 1 frase]
- Impacto esperado: [horas/mês e R$/mês, estimativa conservadora]
- Recursos: [o que já tenho e o que preciso]
- Próximos passos: [as 3 ações datadas]
- Indicador: [métrica que já existe + alvo em 30 dias]

# TAREFA
Estruture minha argumentação no formato de 3 frases: problema em número ·
piloto proposto · retorno esperado com evidência. Depois, liste as 3 perguntas
mais prováveis da diretoria e a resposta curta para cada uma, usando só o meu Canvas.

# FORMATO
Bloco 1: as 3 frases, prontas para falar. Bloco 2: tabela Pergunta provável | Resposta
em 2 linhas. Nada além disso.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Use apenas os dados do meu Canvas — não crie número novo nem prometa além do indicador.
```

**Como avaliar:** a primeira frase contém um número que incomoda? Alguma resposta promete o que o Canvas não sustenta? Corte. As objeções do cético do M1 entram no contexto.

---

## Prompts por área da Mallory

Novos prompts, um por situação real da sala. Dados fictícios ou campos para desidentificar — as 5 categorias valem em todos.

### Controladoria / Financeiro

#### Análise de variação de rubrica com histórico

**Área:** Controladoria / Financeiro
**Para quando:** uma rubrica estourou de novo e a pergunta da diretoria será "é tendência ou acidente?" — responda antes de ser perguntado.
**Você leva:** diagnóstico estrutural × pontual com a premissa a vigiar no próximo fechamento.

```text
# PAPEL
Você é um controller sênior com experiência em análise de tendência de custos industriais.

# CONTEXTO
Fabricante de eletroportáteis, ERP Datasul. Rubrica em análise: [ex.: frete].
Histórico FICTÍCIO de 6 meses (troque pelos seus, desidentificados — sem nome de transportadora):
jan R$ 590 mil · fev R$ 610 mil · mar R$ 660 mil · abr R$ 700 mil · mai R$ 780 mil · jun R$ 840 mil.
Orçado mensal: R$ 620 mil. Fatos que conheço: [ex.: mix de vendas deslocou para o Norte;
contrato de frete renova em setembro; combustível subiu no trimestre]

# TAREFA
Analise a variação: separe o que os fatos explicam do que fica sem explicação, classifique
a tendência (estrutural, pontual ou indefinida) e diga qual premissa, se confirmada,
muda a classificação.

# FORMATO
3 blocos: Leitura da série (5 linhas) · Tabela Fator | Quanto explica | Evidência no contexto ·
Fechamento: classificação + a premissa a vigiar no próximo fechamento.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não estime valores que a série não sustenta. O que os fatos não explicam, marque como "investigar".

# CRITÉRIO DE SUCESSO
Eu respondo "é tendência ou acidente?" em 1 minuto, citando fator e evidência —
sem reabrir a planilha na frente da diretoria.

# CRITÉRIO NEGATIVO
Não conclua causa que não está nos fatos do contexto. Não use "provavelmente" para
esconder lacuna — lacuna se declara.
```

**Como avaliar:** a parcela "sem explicação" ficou explícita? É ela que vira investigação — análise que explica 100% na primeira passada merece desconfiança.

#### Roteiro de conciliação de contas

**Área:** Controladoria / Financeiro
**Para quando:** a conciliação do fechamento vive na cabeça de uma pessoa — e essa pessoa tira férias.
**Você leva:** roteiro passo a passo que padroniza a conciliação e sobrevive à ausência de quem sabe.

```text
# PAPEL
Você é um analista contábil sênior com experiência em fechamento mensal com ERP.

# CONTEXTO
Fabricante de eletroportáteis, ERP Datasul. Conciliação a padronizar: [ex.: adiantamento
a fornecedores]. Como é feita hoje, nas palavras de quem faz (sem valores nem nomes
de fornecedor): [descreva — ex.: "extrai o razão da conta, cruza com o relatório de
pedidos, marca o que tem entrega pendente, o resto investiga um a um; casos antigos
consulta o fiscal"]. Erros que já aconteceram: [ex.: saldo antigo esquecido por 3 meses]

# TAREFA
Transforme em roteiro de conciliação: passo a passo, o que conferir em cada passo,
critério para marcar item como pendência e quando escalar.

# FORMATO
Lista numerada: Passo | O que fazer | O que conferir | Quando escalar.
Fechamento com checklist de 3 linhas do "conciliação concluída quando...".

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não acrescente passo que eu não descrevi — se identificar lacuna óbvia no processo,
marque como "sugestão a validar", separada do roteiro.

# CRITÉRIO DE SUCESSO
Um analista que nunca fez esta conciliação executa o roteiro no próximo fechamento
com no máximo 2 dúvidas.

# CRITÉRIO NEGATIVO
Sem jargão contábil não traduzido. Sem passo genérico tipo "verificar inconsistências" —
todo passo diz o que conferir, onde.
```

**Como avaliar:** teste real no próximo fechamento — quem nunca fez executa? As dúvidas que surgirem viram a v2 do roteiro; roteiro é ativo vivo.

### RH / Gestão de Pessoas

#### Análise de saída de talento (turnover)

**Área:** RH / Gestão de Pessoas
**Para quando:** os desligamentos do semestre precisam virar leitura de padrão antes da reunião de gente — sem nenhum dado individual na ferramenta.
**Você leva:** hipóteses de padrão a partir de dados agregados, com o que verificar antes de agir.

```text
# PAPEL
Você é um consultor de gestão de pessoas com experiência em indústria.

# CONTEXTO
Fabricante de eletroportáteis, 400+ funcionários. Dados AGREGADOS de desligamentos
voluntários do semestre (nenhum dado individual — só contagens):
[troque pelos seus — ex.: "14 saídas voluntárias · 8 da produção, 6 do administrativo ·
9 com menos de 2 anos de casa · 5 no primeiro trimestre, 9 no segundo · motivos citados
em desligamento: proposta melhor (7), distância de casa (3), relação com liderança (4)"]
Contexto que conheço: [ex.: concorrente instalou fábrica na região em março]

# TAREFA
Identifique padrões nos dados agregados, formule até 3 hipóteses do que está acontecendo
e diga o que verificar para confirmar ou descartar cada uma.

# FORMATO
Bloco 1: padrões visíveis (até 5 linhas). Bloco 2: tabela Hipótese | O que a sustenta |
Como verificar. Sem recomendação de ação — primeiro confirmar, depois agir.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Trabalhe só com os agregados do contexto. Não infira nada sobre indivíduos ou áreas
que os números não sustentam.

# CRITÉRIO DE SUCESSO
Levo à reunião de gente 3 hipóteses com plano de verificação — em vez de 1 opinião
formada por 2 casos marcantes.

# CRITÉRIO NEGATIVO
Nenhuma conclusão definitiva sobre causa. Nenhuma sugestão que pressuponha dado
individual que não foi (nem pode ser) fornecido.
```

**Como avaliar:** as hipóteses são verificáveis com dado que o RH tem? Lembre a regra: dado individual de funcionário **nunca** entra — a análise é sempre sobre agregados.

#### Briefing de desenvolvimento por gestor

**Área:** RH / Gestão de Pessoas
**Para quando:** o ciclo de desenvolvimento começa e cada gestor precisa de um roteiro para a conversa com a equipe — não de um formulário a mais.
**Você leva:** roteiro de conversa de desenvolvimento que os gestores seguem sem virar burocracia.

```text
# PAPEL
Você é um especialista em desenvolvimento de lideranças em ambiente industrial.

# CONTEXTO
Sou Gerente de Gente de uma fabricante de eletroportáteis. Vamos rodar o ciclo de
conversas de desenvolvimento com [ex.: 35] gestores e líderes. Diretrizes do ciclo:
[ex.: "foco em 1 força a ampliar e 1 lacuna a trabalhar por pessoa; plano com ação
prática no trabalho, não só curso; revisão em 90 dias"]. Realidade da casa: gestores
de fábrica têm pouco tempo de mesa e pouca paciência com formulário.

# TAREFA
Crie o briefing da conversa de desenvolvimento para os gestores: como preparar,
roteiro da conversa em passos, erros a evitar e o registro mínimo que o RH precisa.

# FORMATO
1 página: Antes (3 itens de preparação) · Durante (roteiro em 5 passos, com a pergunta
de abertura de cada passo) · Depois (registro mínimo em 4 campos) · "3 erros que matam
a conversa".

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Nenhum exemplo com nome ou caso real de pessoa. Não crie etapa de formulário além
do registro mínimo que eu defini.

# CRITÉRIO DE SUCESSO
Um supervisor de produção lê o briefing em 5 minutos e conduz a conversa na mesma
semana sem me chamar.

# CRITÉRIO NEGATIVO
Sem linguagem de RH não traduzida. Se soar como processo corporativo
em vez de conversa de líder, refazer.
```

**Como avaliar:** teste com 1 gestor piloto antes de mandar para os 35 — a pergunta que ele fizer é o que falta no briefing.

### Jurídico

#### Comparação de minuta nova × contrato vigente

**Área:** Jurídico
**Para quando:** o fornecedor mandou a minuta de renovação "igual à anterior" — e você precisa saber em 1 hora o que mudou de verdade.
**Você leva:** tabela do que mudou, o que cada mudança significa e o que levar à negociação.

```text
# PAPEL
Você é um analista de contratos sênior com experiência em fornecedores industriais.

# CONTEXTO
Renovação de contrato de fornecimento. Cole abaixo os dois textos DESIDENTIFICADOS
(sem nome das partes, valores substituídos por [V1], [V2]...):
--- CONTRATO VIGENTE (cláusulas relevantes) ---
[cole]
--- MINUTA NOVA ---
[cole]

# TAREFA
Compare os dois textos: liste toda diferença de conteúdo (não de redação), classifique
cada uma como favorável, neutra ou desfavorável à contratante, e aponte as que merecem
negociação antes da assinatura.

# FORMATO
Tabela: Cláusula | O que mudou | Efeito prático | Favorável/Neutra/Desfavorável ·
Fechamento com os pontos de negociação em ordem de relevância.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não cite cláusula que não está nos textos. Diferença só de redação sem efeito prático,
marque como "estilo". Não emita parecer — a análise prepara a revisão humana.

# CRITÉRIO DE SUCESSO
A gestora entra na negociação sabendo exatamente o que mudou e o que pedir —
sem depender da palavra do fornecedor de que "está igual".

# CRITÉRIO NEGATIVO
Nenhuma diferença relevante omitida por parecer pequena — mudança de prazo e de índice
nunca é "estilo". Sem juridiquês não traduzido.
```

**Como avaliar:** faça a contraprova em 2 cláusulas críticas lendo os textos originais — a IA achou o que você achou? Diferença que a IA marcou como "estilo", confira antes de aceitar.

#### Triagem de norma nova

**Área:** Jurídico
**Para quando:** saiu norma, decreto ou regulamento novo e a pergunta é uma só: afeta a Mallory, onde, e com que prazo?
**Você leva:** triagem estruturada do texto normativo — com a obrigação de conferir cada artigo na fonte.

```text
# PAPEL
Você é um advogado empresarial com experiência em indústria de manufatura.

# CONTEXTO
Fabricante de eletroportáteis no Ceará (produção própria, importação de componentes,
vendas nacionais, 400+ funcionários). Texto normativo a triar (cole o TEXTO OFICIAL —
não peça à IA de memória):
[cole o texto ou os trechos relevantes da norma]

# TAREFA
Faça a triagem: quais dispositivos alcançam uma empresa com este perfil, o que cada um
exige na prática, qual o prazo e qual área da empresa é a dona do tema.

# FORMATO
Tabela: Dispositivo (artigo/item) | O que exige | Prazo | Área responsável provável ·
Fechamento: os 2 dispositivos mais urgentes e por quê.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Analise APENAS o texto colado — não complete com o que você "sabe" da legislação, não
cite norma correlata sem que eu peça. Interpretação com consequência relevante,
marque "confirmar com parecer".

# CRITÉRIO DE SUCESSO
Eu sei em 10 minutos se aciono alguma área hoje — e cada linha da tabela aponta
o artigo exato para eu conferir na fonte.

# CRITÉRIO NEGATIVO
Nenhuma afirmação sobre dispositivo que não está no texto colado. Sem "de acordo com
a legislação vigente" genérico — só o que está na fonte fornecida.
```

**Como avaliar:** todo artigo citado na tabela existe no texto que você colou (confira 100% — é aqui que IA jurídica mais inventa)? A triagem orienta; o parecer continua humano. Caso-âncora: Mata v. Avianca.

### Fiscal / Contábil

#### Checklist de mudança regulatória

**Área:** Fiscal / Contábil
**Para quando:** uma mudança de regra fiscal foi confirmada e a área precisa de um plano de adequação que não deixe etapa para trás.
**Você leva:** checklist de adequação organizado por frente, para validar com a consultoria antes de executar.

```text
# PAPEL
Você é um consultor tributário com experiência em indústria.

# CONTEXTO
Fabricante de eletroportáteis, ERP Datasul. Mudança regulatória confirmada:
[descreva com o comunicado oficial em mãos — ex.: "alteração na regra de destaque
do imposto X para operações interestaduais, vigência em 90 dias"]. O que já sabemos:
[ex.: "afeta o faturamento para 3 estados; a parametrização do ERP é da consultoria;
o time fiscal precisa retreinar a conferência"]

# TAREFA
Monte o checklist de adequação: toda frente afetada (sistema, processo, pessoas,
documentos), o que fazer em cada uma e a ordem de dependência entre elas.

# FORMATO
Tabela: Frente | Ação | Depende de | Prazo sugerido (contando da vigência para trás) ·
Fechamento com os 3 itens que, se atrasarem, travam o resto.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não detalhe alíquota, base de cálculo nem interpretação da regra — isso vem da
consultoria e da fonte oficial. O checklist organiza o trabalho, não define o conteúdo fiscal.
```

**Como avaliar:** a consultoria valida o checklist sem acrescentar frente esquecida? O conteúdo fiscal (alíquota, base, enquadramento) vem sempre da fonte oficial — o checklist só garante que nada fica para trás.

### Logística Administrativa

#### Priorização de janela de entrega

**Área:** Logística Administrativa
**Para quando:** há mais pedido do que janela de expedição na semana — e a decisão de quem sai primeiro precisa de critério, não de quem gritou mais alto.
**Você leva:** proposta de sequência de expedição com critério explícito, para você bater o martelo.

```text
# PAPEL
Você é um coordenador de logística experiente em indústria de bens de consumo.

# CONTEXTO
Fabricante de eletroportáteis. Janelas de expedição disponíveis na semana: [ex.: 6].
Pedidos aguardando (FICTÍCIOS — troque pelos seus, sem nome de cliente):
- Pedido A: cliente grande varejo, prazo contratual vence quinta, multa por atraso
- Pedido B: cliente regional, prazo vence semana que vem, caminhão próprio dele
- Pedido C: reposição de centro de distribuição, estoque do CD em nível crítico
- Pedido D: cliente médio, pedido atrasado desde semana passada, já reclamou 2 vezes
- Pedido E: exportação, navio com corte de recebimento na sexta
[ajuste à sua realidade]
Critérios que a área usa: [ex.: multa contratual > risco de ruptura > tempo de atraso]

# TAREFA
Proponha a sequência de expedição da semana aplicando os critérios da área, com
justificativa por pedido — e aponte qual conflito de critério eu preciso decidir pessoalmente.

# FORMATO
Tabela: Ordem | Pedido | Janela sugerida | Critério aplicado | Risco se adiar ·
Fechamento: o conflito que exige decisão do coordenador.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não crie prazo, multa ou nível de estoque que não estão no contexto. A sequência é
proposta — a decisão final é minha.

# CRITÉRIO DE SUCESSO
Eu defendo a sequência para qualquer área que reclamar, citando o critério —
em vez de renegociar pedido a pedido.

# CRITÉRIO NEGATIVO
Sem empate resolvido em silêncio: onde dois critérios conflitam, a resposta explicita
o conflito em vez de escolher por mim.
```

**Como avaliar:** o conflito apontado é real (é onde você teria dúvida)? Se a IA "resolveu tudo" sem apontar conflito, desconfie — semana apertada sempre tem trade-off.

### Importação

#### Comparativo de fornecedores por critério ponderado

**Área:** Importação
**Para quando:** 3 cotações na mesa e a escolha precisa sair defensável — preço não é o único critério, e todo mundo sabe, mas ninguém formaliza.
**Você leva:** matriz ponderada com pesos seus e sensibilidade: o que muda se o peso mudar.

```text
# PAPEL
Você é um comprador internacional sênior de componentes industriais.

# CONTEXTO
Fabricante de eletroportáteis. Cotações DESIDENTIFICADAS para [ex.: componente
eletrônico da linha de air fryer] — fornecedores A, B, C, valores em índice
(menor preço = 100):
- A: preço 100 · lead time 60 dias · histórico: 1 atraso em 8 embarques · MOQ alto
- B: preço 112 · lead time 35 dias · histórico: sem atrasos em 5 embarques · MOQ flexível
- C: preço 95 · lead time 75 dias · fornecedor novo, sem histórico · exige pagamento antecipado
[ajuste à sua realidade — sem nome real de fornecedor nem preço absoluto]
Pesos da área: [ex.: preço 40% · confiabilidade de prazo 35% · flexibilidade 25%]

# TAREFA
Monte a matriz ponderada com os meus pesos, calcule o ranking e mostre a sensibilidade:
qual mudança de peso inverte o resultado.

# FORMATO
Tabela: Critério | Peso | Nota A | Nota B | Nota C (notas justificadas em 1 linha) ·
Ranking final · Parágrafo de sensibilidade: "o resultado inverte se...".

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Use apenas os dados do contexto. Confiro os cálculos antes de usar. Não recomende
o vencedor como decisão — a matriz informa, quem assina o pedido sou eu.

# CRITÉRIO DE SUCESSO
Levo à reunião uma escolha defensável: ranking, pesos explícitos e o cenário
em que a escolha mudaria.

# CRITÉRIO NEGATIVO
Nenhuma nota sem justificativa. O fornecedor sem histórico não pode receber nota
de confiabilidade "média" por falta de dado — falta de dado é risco, e se declara.
```

**Como avaliar:** recalcule a ponderação do vencedor na mão. A frase de sensibilidade é a mais valiosa da resposta — é ela que antecipa a discussão da reunião.

### Marketing

#### Briefing de campanha a partir de indicador

**Área:** Marketing
**Para quando:** um indicador acendeu (sell-out caindo, linha parada no varejo) e a resposta precisa ser uma campanha com objetivo mensurável — não "fazer barulho".
**Você leva:** briefing de campanha amarrado ao indicador que a motivou, com meta e prazo.

```text
# PAPEL
Você é um coordenador de marketing experiente em bens de consumo no varejo brasileiro.

# CONTEXTO
Fabricante de eletroportáteis. Indicador que motiva a campanha (FICTÍCIO — troque pelo
seu, sem dado de cliente ou margem): [ex.: "sell-out da linha de ventiladores caiu 18%
no trimestre versus ano anterior, concentrado no varejo físico do Nordeste; estoque no
canal 40% acima do normal"]. Verba e janela: [ex.: verba média, campanha de 6 semanas
antes do pico de verão]. Canais disponíveis: [ex.: PDV, redes sociais, cooperado com varejo]

# TAREFA
Redija o briefing da campanha: objetivo amarrado ao indicador, público, mensagem
central, papel de cada canal e como mediremos — meta numérica e prazo.

# FORMATO
1 página: Contexto (3 linhas) · Objetivo com meta e prazo · Público · Mensagem central
(1 frase) · Canais e papel de cada um · Medição (indicador + frequência de leitura).

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não crie dado de mercado, share ou comportamento do consumidor que não está no contexto.
Não detalhe peça criativa — briefing define o problema, a agência cria.

# CRITÉRIO DE SUCESSO
A agência (ou o time interno) lê o briefing e faz no máximo 2 perguntas antes de propor —
e a diretoria vê a linha reta entre o indicador e a campanha.

# CRITÉRIO NEGATIVO
Sem objetivo do tipo "fortalecer a marca" sem número. Se a meta não puder ser lida
no indicador que motivou a campanha, refazer.
```

**Como avaliar:** a meta da campanha se mede no mesmo indicador que a motivou? Se a resposta criou "awareness" como meta de uma queda de sell-out, o Critério Negativo falhou — refaça.

### TI

#### Triagem de backlog de chamados por criticidade

**Área:** TI
**Para quando:** o backlog cresceu e a fila está sendo atendida por ordem de chegada — quando deveria ser por impacto.
**Você leva:** backlog classificado por criticidade com regra explícita, pronto para virar rotina semanal.

```text
# PAPEL
Você é um coordenador de TI experiente em ambiente industrial com ERP.

# CONTEXTO
Fabricante de eletroportáteis, ERP Datasul, fábrica em 2 turnos. Regra de criticidade
da área: para produção e faturamento > afeta área inteira > afeta 1 usuário > melhoria.
Backlog atual (FICTÍCIO — troque pelo seu, sem nome de usuário):
- integração do apontamento de produção intermitente desde ontem
- relatório mensal do financeiro com erro de totalização
- 3 usuários sem acesso ao módulo de compras após atualização
- lentidão geral no ERP no início do turno da manhã
- solicitação de novo campo em tela de cadastro
- impressora fiscal da expedição parando 2x por dia
[ajuste à sua realidade]

# TAREFA
Classifique cada chamado pela regra de criticidade, ordene a fila e aponte quais
chamados podem ser o mesmo problema raiz.

# FORMATO
Tabela: Ordem | Chamado | Criticidade | Por quê | Possível causa comum (se houver).

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Não diagnostique causa técnica — "possível causa comum" é hipótese para investigação,
marcada como hipótese. A regra de criticidade é a da área; não crie critério novo.
```

**Como avaliar:** a ordenação segue a regra da área sem exceção escondida? As hipóteses de causa comum economizaram diagnóstico? Rode toda segunda de manhã — triagem é rotina, não evento.

### Planejamento

#### Briefing S&OP com cenários

**Área:** Planejamento
**Para quando:** a reunião mensal de S&OP se aproxima e os indicadores precisam virar decisão — não leitura de slide.
**Você leva:** briefing executivo com 3 cenários de premissas explícitas e a decisão que a reunião precisa tomar.

```text
# PAPEL
Você é um consultor de S&OP com experiência em indústria de bens de consumo.

# CONTEXTO
Fabricante de eletroportáteis. Indicadores AGREGADOS do ciclo (FICTÍCIOS — troque pelos
seus, sem dado de cliente): [ex.: "previsão de vendas do trimestre: 120 mil unidades
(+8% vs ciclo anterior) · capacidade de produção: 110 mil no regime atual · estoque de
produto acabado: 25 dias de cobertura · componente crítico da linha de ventiladores com
lead time subindo de 45 para 70 dias · pico sazonal em 10 semanas"]
Decisão que a reunião precisa tomar: [ex.: abrir turno extra agora ou aguardar 1 ciclo]

# TAREFA
Monte o briefing da reunião: leitura dos indicadores, 3 cenários (base, otimista,
pessimista) com premissas explícitas, o que cada cenário implica para a decisão —
e qual premissa, se falhar, derruba cada cenário.

# FORMATO
1 página: Leitura do ciclo (5 linhas) · Tabela Cenário | Premissas | Implicação para
a decisão | Premissa que derruba · Fechamento: a informação que reduziria a incerteza
antes de decidir.

# LIMITAÇÕES
Se faltar informação, pergunte. Não invente.
Use apenas os indicadores do contexto — não crie projeção de demanda nem custo de
turno extra. A decisão é da reunião, não do briefing.

# CRITÉRIO DE SUCESSO
A reunião passa o tempo discutindo qual cenário é mais provável — não decifrando
os números. A decisão sai com premissas registradas.

# CRITÉRIO NEGATIVO
Sem cenário-fantasia: os 3 cenários derivam dos indicadores fornecidos. Não recomende
um cenário — apresente o espaço da decisão.
```

**Como avaliar:** as premissas dos cenários são fatos verificáveis ou chutes da IA? Marque uma a uma antes da reunião — premissa não validada vira nota de rodapé, não base de decisão.

---

## Antes de fechar a página

- **Prompt bom é ativo da área:** salve, versione, compartilhe com a equipe — a biblioteca da área vale mais que o talento individual.
- As 5 categorias e o protocolo de 3 passos completos: [M4 · Uso Responsável, Governança e Liderança da Adoção](../m4/).
- O CLAUDE.md e a régua L0→L3 da workstation: [M5 · Claude Cowork](../m5/).

---

[← Início](../) · [Artefatos →](../artefatos/)
