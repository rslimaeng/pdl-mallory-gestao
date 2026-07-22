# Prompt · Converse com sua planilha

> **Como usar:** abra o **Claude.ai** (chat no navegador — não precisa Cowork). Anexe `dados-producao-venda-mock.xlsx` (dados fictícios: produção e venda mensal de 6 SKUs em 12 meses). Cole o prompt abaixo.
>
> Este exemplo é o mais simples do módulo. Serve pra mostrar que **antes de pedir gráfico, você conversa** — Claude te ajuda a decidir o que faz sentido visualizar. Depois, se quiser, Artifacts renderiza.

---

Sou **gestor comercial** numa indústria de eletroportáteis (contexto de treinamento). Recebi uma planilha do PCP com **produção e venda mensal dos últimos 12 meses de 6 SKUs** e quero entender o que ela está me contando antes de pedir dashboard bonito pro time de dados.

**Antes de qualquer gráfico**, faz o seguinte comigo, na ordem:

## 1. Sanity check da planilha (30 segundos)
- Quantas linhas, quantas colunas
- Alguma célula em branco ou com valor esquisito (negativo, texto onde deveria ser número)?
- Os totais mensais batem?

Se tiver problema, para aqui e me avisa. Não segue.

## 2. 3 perguntas que a planilha responde bem
Olha os dados e sugere **3 perguntas** que essa planilha específica consegue responder com qualidade — não perguntas genéricas de negócio, perguntas que **esses dados** respondem. Ex: "quais SKUs têm venda maior que produção há mais de 2 meses seguidos?" (indica ruptura vindo).

## 3. 3 perguntas que a planilha NÃO responde
Igualmente importante: onde ela é fraca. Ex: "essa planilha não separa canal de venda, então não dá pra saber se a queda do SKU X foi B2B ou B2C".

## 4. Conversa iterativa
Depois disso, eu vou te fazer perguntas específicas. Você responde com:
- Número direto (não parágrafo)
- Fonte (qual coluna, qual linha) — pra eu conseguir auditar
- Se a resposta depende de suposição, você declara ("estou assumindo que quantidade está em unidades, não caixas")

**Só quando eu pedir**, você renderiza gráfico em artifact. Antes disso, texto e números.

## Regras
- Nunca inventa coluna que não existe.
- Nunca "arredonda" pra deixar bonito — dá o número que a planilha tem.
- Se eu perguntar algo que exige suposição forte (ex: "por que caiu?"), você **hipotetiza** com base nos dados mas marca como hipótese, não fato.
- Português-BR, direto, sem emoji.

---

*Prompt versão 1.0 · PDL Mallory 2026 · M5 T2 · Caso 5*
