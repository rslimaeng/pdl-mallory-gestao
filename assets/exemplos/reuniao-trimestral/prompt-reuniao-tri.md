# Prompt · Prepare a reunião trimestral

> **Como usar:** abra o **Claude Cowork** (desktop app). Anexe os dois arquivos: `slack-export-mock.md` (conversas fictícias do canal comercial) + `receita-tri-mock.xlsx` (dados de receita mensais). Ative **Extended Thinking**. Depois cole o prompt abaixo.
>
> Este exemplo mostra por que Cowork existe: você **delega** a leitura de material extenso e a síntese pra Claude, em vez de conversar bloco por bloco. Enquanto ele processa, você faz outra coisa.

---

Sou **gestor comercial regional** de uma indústria de eletroportáteis (contexto de treinamento). Preciso preparar a **reunião trimestral com a diretoria** que acontece na próxima terça — 45 minutos, 8 pessoas na sala, foco em performance do trimestre e o que muda no próximo.

**O que anexei:**

1. `slack-export-mock.md` — 3 meses de conversas do canal `#comercial-regional` (exportadas em formato markdown). Volume grande, ruído alto, mas tem o histórico de tudo o que a equipe reclamou, celebrou ou levantou como risco.
2. `receita-tri-mock.xlsx` — receita mensal por linha de produto e por região, os últimos 4 trimestres.

**O que eu preciso que você entregue** (use Extended Thinking pra pensar antes de escrever):

## 1. Análise dos dados de receita
- Comparação Q vigente vs Q anterior vs mesmo Q ano anterior.
- Quais linhas de produto puxaram pra cima, quais puxaram pra baixo, com números.
- Se alguma região destoa (positiva ou negativa), destaca.

## 2. Síntese do Slack
Não me dá lista de mensagens. Me dá **temas**: quais 3-5 assuntos apareceram mais vezes na conversa da equipe nos últimos 3 meses? Pra cada tema:
- O que aparece (1 frase)
- Frequência aproximada (alto/médio/baixo)
- Se é reclamação, oportunidade ou alerta
- 1 exemplo curto (parafraseado, sem citar nome de pessoa)

## 3. Cruzamento
Aqui é onde você agrega valor real: **os temas do Slack explicam alguma coisa dos números?** Ex: se região X caiu 15% e no Slack apareceu 8 vezes "problema de estoque na região X", conecta. Se não conecta, diz que não conecta (não força narrativa).

## 4. Deck da reunião (estrutura em texto)
7 slides no máximo, formato de outline (título + 3 bullets por slide). Sequência:
1. Abertura — 1 frase sobre o trimestre em nível macro
2. Números do trimestre
3. Comparações que importam (destaques positivos e negativos)
4. Temas que a equipe sinalizou (Slack)
5. Cruzamento números × temas
6. 3 decisões que a diretoria precisa tomar nessa reunião
7. Próximos passos

## 5. Perguntas difíceis
Se você fosse a diretoria, que 3 perguntas incômodas você faria pro gestor comercial regional depois desse deck? Lista pra eu me preparar.

## Regras
- Nada de superlativo sem número atrás ("crescimento explosivo" — não. "Cresceu 12%" — sim).
- Se dado da planilha estiver ambíguo, marca com `[verificar antes da reunião]`.
- Nomes de pessoas do Slack já vieram anonimizados. Se você notar algum que passou, avisa.

---

*Prompt versão 1.0 · PDL Mallory 2026 · M5 T2 · Caso 3*
