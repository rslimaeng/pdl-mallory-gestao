# M4 · Uso Responsável, Governança e Liderança da Adoção

**Trilha 2 · Módulo 4 de 6 · 1h15**

LGPD, confidencialidade, alucinação como risco de gestão, shadow IT — e como redesenhar processos e liderar a adoção na sua equipe sem gerar resistência.

---

## O contrato deste módulo

**Você ganha:** o rascunho das diretrizes de uso de IA da sua área e uma régua simples para redesenhar processos — o que delegar, o que manter como apoio, o que fica só com humano.

**Você se compromete a:** escrever a primeira versão das diretrizes ainda em sala e definir como vai comunicá-las à equipe sem transformar orientação em caça às bruxas.

**Tempo de leitura desta página:** 11 min

---

## Você entra com → O que acontece → Você sai com

| Você entra com | O que acontece | Você sai com |
|---|---|---|
| As 3 oportunidades priorizadas do M3 — pelo menos 1 toca dado que exige cuidado | Você aplica os 3 modos do M1 (Autopiloto · Colaboração · Manual) como régua de governança da sua área e escreve as diretrizes | Diretrizes rascunhadas + o mapa de qual processo entra em qual modo — pré-requisito do M5, onde a IA ganha acesso a arquivos |

---

## Por que isso importa aqui dentro

Metade da sua equipe já usa IA. Você provavelmente não sabe qual metade, nem com quais dados. Isso não é hipótese provocativa — é o retrato que a pesquisa interna da Mallory sobre uso de ferramentas de IA foi feita para revelar. O uso não homologado tem nome, shadow IT, e a resposta errada para ele é proibir: proibição não elimina o uso, só o esconde — e esconde junto o dado que vazou.

A dimensão nova deste módulo, em relação a tudo que você já sabe de uso seguro: **você responde pela área**. Quando alguém do seu time cola dados de funcionário numa ferramenta externa, a LGPD não pergunta quem clicou — pergunta quem deveria ter orientado. Quando um número inventado pela IA sobe num relatório assinado por você, o erro é da sua mesa.

A boa notícia: a Mallory já se move nesse tema — protótipo no jurídico, pesquisa de governança, TI engajado. O que falta é o elo entre a política corporativa e o dia a dia de cada área. Esse elo é a diretriz que você escreve hoje.

---

## O conceito em 5 pontos

### 1. LGPD executiva: quem responde é quem enviou — e a empresa junto

Dado pessoal é o que identifica alguém: nome, CPF, salário, atestado, avaliação, dado de candidato. A LGPD responsabiliza a empresa pelo tratamento — inclusive pelo que um colaborador cola numa ferramenta externa por conta própria. Para o gestor, a consequência é direta: orientar a equipe não é zelo, é gestão de risco da área.

### 2. Os 3 "nunca" — com a camada do gestor

A regra que a turma da manhã levou vale aqui: **gente, produto, contrato** — nunca entram em ferramenta externa. O gestor soma duas categorias: **dado de diretoria** (resultado não divulgado, plano estratégico, decisão em discussão) e **informação de concorrência** (preço, condição, negociação). Mnemônico da área: se vazasse, quem teria que dar explicação é você? Então não entra.

### 3. Alucinação é risco de gestão, não defeito de ferramenta

A IA erra com a mesma fluência com que acerta — e a decisão assistida por IA continua tendo um único assinante: você. O protocolo de 3 passos vira norma da área: **fonte** (o fato veio do que enviamos?), **número** (todo número, data e cláusula conferidos na origem), **consistência** (bate com o que sabemos?). Custa 30 segundos por documento; a versão sem protocolo custa uma reunião de retratação.

### 4. Shadow IT: a equipe já usa — orientar é mais barato que proibir

Proibir empurra o uso para o celular pessoal, fora de qualquer visibilidade. A diretriz clara faz o contrário: diz onde a IA é bem-vinda, com quais dados, com qual revisão — e transforma usuários escondidos em usuários orientados. O antídoto do shadow IT não é firewall: é uma página de regras que a equipe entende e um gestor que pergunta "o que você está automatizando?" sem tom de auditoria.

### 5. A régua de redesenho: Autopiloto · Colaboração · Manual

Todo processo da sua área cabe em uma das três faixas do M1 — agora usadas como instrumento de governança, não só de uso pessoal. **Autopiloto:** a IA executa o rascunho ou a compilação inteira, alguém revisa — relatório recorrente, primeira versão de documento, consolidação de dados desidentificados. **Colaboração:** a IA apoia, o humano conduz — análise, estruturação de cenário, preparação de decisão executiva. **Manual:** a IA não entra — decisão sobre pessoa, assinatura de parecer, aprovação final, posicionamento à diretoria. Redesenhar processo com IA é decidir a faixa de cada etapa — e escrever isso na diretriz, para que a equipe não decida sozinha em qual faixa cada tarefa mora.

---

## Quando aplicar / Quando NÃO aplicar

| 🟢 O que orientar (e incentivar) | 🔴 O que restringir (por escrito) |
|---|---|
| Rascunho e compilação de documento recorrente, com revisor nomeado | Qualquer dado das 5 categorias: gente, produto, contrato, diretoria, concorrência |
| Análise e cenário como preparação de decisão — decisão fica com humano | Decisão sobre pessoa assistida por IA sem julgamento humano documentado |
| Uso com conta e ferramenta homologadas pelo TI | Ferramenta nova na área sem passar pelo TI — é assim que nasce o shadow IT |
| Compartilhar prompts que funcionam — biblioteca da área | Repassar saída de IA como parecer técnico sem o protocolo de 3 passos |

---

## Prompt-âncora do módulo

O território mais sensível da sala — revisão de contrato — feito do jeito certo: dados fictícios, limitações explícitas. Roda como está:

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

Repare no desenho: dado fictício, proibição de inventar cláusula, fronteira explícita com o parecer humano. É este padrão que a sua diretriz vai exigir da equipe.

---

## Exercício

### Camada 1 — Básico (todos · 15 min)

**Objetivo:** escrever a primeira versão das diretrizes de uso de IA da sua área.

**Passo a passo:**
1. Monte o prompt: papel = "consultor de governança de dados em indústria"; contexto = sua área, tamanho da equipe, os processos do seu mapa do M3 e as 5 categorias de dado proibido; tarefa = "redija diretrizes de uso de IA em 1 página: onde usar, com quais dados, qual revisão, o que é proibido"; Critério de Sucesso = "um analista novo entende as regras sem me perguntar"; Negativo = "sem tom de ameaça — o objetivo é orientar o uso, não assustar".
2. Rode e edite: corte o que não se aplica, endureça o que a sua área exige. A IA rascunha a diretriz — quem assina a régua é você.
3. Aplique a régua dos 3 modos (Autopiloto / Colaboração / Manual) aos 3 processos do seu mapa do M3: marque a faixa de cada um na própria diretriz — e diga em 1 linha por que aquela e não outra.
4. Valide com o colega do lado: ele entende as regras da sua área em 2 minutos de leitura?

**Resultado esperado:** diretrizes da sua área em 1 página, com os 3 processos do M3 classificados na régua.

**Como avaliar:** teste do analista novo — se alguém recém-chegado lê e sabe o que pode, com o quê e quem revisa, está pronta. Se precisa de você do lado explicando, ainda é rascunho: aperte mais uma rodada.

### Camada 2 — Desafio (para quem terminou · +10-15 min)

**Objetivo:** preparar a conversa de adoção — a diretriz sem a conversa vira circular ignorada.

**Passo a passo:**
1. Peça à IA: "Simule as 3 reações mais prováveis da minha equipe a estas diretrizes — o entusiasta que já usa tudo, o cético que acha perda de tempo, o inseguro que teme ser substituído. Para cada um, o que dizer e o que não dizer." Cole a diretriz.
2. Avalie as respostas contra o que você sabe da sua equipe real — ajuste com nomes em mente (sem colocar os nomes no prompt).
3. Ensaie a fala de abertura: 3 frases que apresentam a diretriz como habilitação, não como policiamento.
4. Marque no calendário: quando e em que fórum você comunica.

**Resultado esperado:** roteiro da conversa de adoção com resposta preparada para os 3 perfis.

**Como avaliar:** se a sua fala de abertura contém a palavra "proibido" antes de conter "podem", inverta — a diretriz que a equipe abraça começa pelo que habilita.

---

## Os 3 erros mais comuns

| Erro | Sintoma | Causa | Como corrigir |
|---|---|---|---|
| Governança por e-mail | Diretriz enviada, nunca conversada — 3 semanas depois, ninguém lembra | Tratar adoção como comunicado, não como conversa | 15 minutos de reunião: contexto, regras, perguntas. E-mail é o registro, não o veículo |
| Proibir para se proteger | "Melhor ninguém usar até a empresa definir" — e a equipe usa escondido | Confundir ausência de regra com ausência de uso | A regra da sua área pode existir antes da política corporativa — e ser absorvida por ela depois |
| Régua sem manutenção | Processo mudou de faixa (Autopiloto → Colaboração porque a IA piorou naquele caso, ou o oposto porque a equipe ganhou maturidade) e ninguém atualizou | Tratar a diretriz como documento, não como instrumento vivo | Revisão trimestral de 10 minutos: a régua ainda bate com a prática? |

---

> ⚠️ **Anti-alucinação e governança — o protocolo da sua área (leve esta página)**
>
> **Por que existe:** em *Mata v. Avianca* (2023), advogados entregaram à Justiça uma petição com 6 decisões judiciais que o ChatGPT inventou — plausíveis, confiantes, falsas. Sanção pública e dano de reputação. E mesmo ferramentas que leem os seus documentos erram: estudos de Stanford (2025) mediram 17–33% de erro em sistemas desse tipo. Rastreável não é sinônimo de correto.
>
> **As 5 categorias que nunca entram em ferramenta externa:**
> - **Gente** — nome, CPF, salário, atestado, avaliação, dado de candidato (LGPD)
> - **Produto** — especificação, parâmetro de processo, desenho, fórmula
> - **Contrato** — contratos, preços, condições de fornecedor e cliente
> - **Diretoria** — resultado não divulgado, plano estratégico, decisão em discussão
> - **Concorrência** — informação de negociação ou inteligência competitiva
>
> **O protocolo de 3 passos — agora como norma da área:**
> 1. **Fonte** — cada fato da resposta veio do que foi enviado?
> 2. **Número** — todo número, data, cláusula e norma, conferidos na origem
> 3. **Consistência** — bate com o que a área sabe? Estranhou, checou
>
> **A camada do gestor:** você responde pelo uso da sua equipe — o que sobe assinado é seu, e o que vaza da sua área é seu. A diretriz escrita e conversada é a diferença entre risco gerido e surpresa. Se a IA respondeu com confiança algo que ninguém da área sabia: desconfie em dobro e verifique antes de qualquer uso.

---

> 🟣 **Marco: o que você leva para a Mallory na 2ª feira**
> Até sexta-feira, comunique as diretrizes à sua equipe: 15 minutos de conversa (não e-mail solto) apresentando onde usar, com quais dados e quem revisa — e registre a versão v1 no repositório da área.
> Como saber que aconteceu: a equipe participou da conversa, a diretriz está registrada, e você anotou as 2 melhores perguntas que surgiram.

---

[← M3 · IA por Área](../m3/) · [M5 · Claude Cowork: sua Workstation de IA →](../m5/)

[Banco de Prompts](../banco-de-prompts/) · [Artefatos](../artefatos/)
