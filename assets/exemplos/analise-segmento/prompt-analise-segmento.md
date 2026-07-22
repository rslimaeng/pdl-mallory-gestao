# Prompt · Análise de segmento bottom-up

> **Como usar:** abra o **Claude Cowork** (desktop app). Anexe `gabarito-metodologia-tam-sam-som.xlsx` (planilha modelo com fórmulas em branco). Ative **Extended Thinking**. Cole o prompt abaixo.
>
> Este exemplo mostra Cowork num trabalho que **normalmente virava consultoria externa**: dimensionar um mercado com metodologia auditável (não com número redondo puxado de relatório de terceiro).

---

Sou **gestor de portfólio** numa indústria de eletroportáteis (contexto de treinamento). A diretoria pediu uma análise de tamanho de mercado pra um **novo segmento hipotético**: eletroportáteis para cozinha profissional de pequeno porte (cafeterias, padarias artesanais, bistrôs — não hotelaria industrial). Brasil, mercado B2B.

Precisamos decidir se vale a pena entrar. E não posso levar pra diretoria "achamos que dá R$ X" — precisa ter metodologia.

**O que quero de você**, usando Extended Thinking pra pensar antes de calcular:

## 1. Framework
Aplique **TAM · SAM · SOM** bottom-up (não top-down puxando de relatório). Isso quer dizer:
- **TAM** = universo total possível (todos os potenciais compradores no Brasil)
- **SAM** = subconjunto que a Mallory conseguiria endereçar dado nosso perfil (canal, preço, capacidade produtiva)
- **SOM** = fatia realista nos primeiros 24 meses dado nosso posicionamento

## 2. Bottom-up de verdade
Não me dá "mercado brasileiro de eletroportáteis é R$ X bilhões, assumimos 2%". Isso é preguiça. Bottom-up significa:
- Quantas cafeterias operam no Brasil? (você pode usar estimativas públicas — SEBRAE, ABIC, IBGE)
- Quantas padarias artesanais e bistrôs? (mesmo raciocínio)
- Quanto cada uma gasta em média com eletroportáteis por ano? (ciclo de reposição + expansão)
- Multiplica.
- **Todas as fontes citadas.** Se você chutou, marca "[estimativa não verificada]".

## 3. Preenche a planilha
`gabarito-metodologia-tam-sam-som.xlsx` tem as células em branco e os headers montados. Preenche cada célula com o número + na coluna ao lado a fonte ou premissa. Se a premissa depende de um "chute educado", explica em 1 linha por que aquele chute é razoável.

## 4. Análise de sensibilidade
Depois de preencher, mostra 3 cenários:
- **Otimista** (premissas favoráveis dentro do razoável)
- **Base** (premissas médias)
- **Pessimista** (premissas conservadoras)

Uma tabela comparando os 3 no SOM final.

## 5. Sumário executivo (2 páginas)
Formato de outline (não texto corrido). Estrutura:
- Pergunta que estamos respondendo
- Método aplicado (2 linhas)
- Resultado principal (SOM base + faixa otimista/pessimista)
- 3 premissas mais frágeis (as que mais movem o resultado se erradas)
- Recomendação (entrar / não entrar / pilotar / investigar mais)
- 3 dados que ainda faltam pra decisão ficar sólida

## Regras
- **Nunca invente número.** Se não sabe, "[estimativa a validar]".
- **Não use relatório proprietário** (Gartner, Frost) porque não temos acesso. Só fontes públicas.
- **Faixa > ponto.** Prefere dizer "entre R$ 40M e R$ 60M" do que "R$ 50M".
- Se algum passo dependa de dado que só a Mallory tem (nossa capacidade produtiva atual, nosso ticket médio), marca como `[buscar internamente]` — não chuta.

---

*Prompt versão 1.0 · PDL Mallory 2026 · M5 T2 · Caso 4*
