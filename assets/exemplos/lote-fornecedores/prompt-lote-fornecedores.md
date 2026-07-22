# Prompt · Lote de fornecedores

> **Como usar:** abra o **Claude Cowork** (desktop app). Anexe as **5 cotações fictícias**: `cotacao-fornecedor-A.pdf` até `cotacao-fornecedor-E.pdf`. Cole o prompt abaixo.
>
> Este caso mostra a força do Cowork em **processamento em lote**: você delega a leitura de N arquivos parecidos e recebe uma consolidação. No chat comum você teria que anexar um por um, comparar mental, montar tabela. Aqui é uma passada.

---

Sou **gestor de suprimentos** numa indústria de eletroportáteis (contexto de treinamento). Preciso escolher fornecedor pra um componente eletrônico de linha média. **Cinco fornecedores** me enviaram cotação (arquivos anexados, formato PDF cada).

Os PDFs não estão em template padronizado — cada fornecedor mandou do jeito dele. Volume, prazo, condição de pagamento, garantia, certificação — cada um destaca uma coisa. Se eu ler um por um vai um dia inteiro.

**O que você vai fazer:**

## 1. Leia os 5 PDFs
Não me pede pra colar conteúdo. Você extrai dos anexos.

## 2. Monte uma tabela comparativa
Colunas mínimas:
- Fornecedor
- Preço unitário (na moeda em que veio, com conversão sinalizada se aplicável)
- Volume mínimo
- Prazo de entrega
- Condição de pagamento
- Garantia oferecida
- Certificações mencionadas (ISO, RoHS, etc.)
- Origem (Brasil, importado — de onde)

Se alguma cotação não menciona algum campo, marca **"não informado"** — não chuta.

## 3. 3 observações qualitativas por fornecedor
Curtas, tipo:
- Fornecedor A — "Cotação bem estruturada, condição de pagamento agressiva, mas prazo longo."
- Fornecedor B — "Preço mais baixo do lote, porém sem certificação declarada. Vale investigar."

Baseadas no que você viu no PDF — não invente.

## 4. Ranking em 3 critérios
Não me dá "vencedor absoluto". Ranking em três recortes:
- **Melhor preço** (top 3, com % de diferença)
- **Melhor prazo** (top 3)
- **Melhor condição comercial global** (ponderando preço + prazo + garantia — explica a ponderação que você usou)

## 5. 3 perguntas que eu deveria fazer antes de fechar
Baseado nas ambiguidades ou omissões que você notou nos PDFs, o que EU precisaria confirmar com cada fornecedor antes de bater o martelo?

## Regras
- Nada de "eu recomendo o fornecedor X" definitivamente — você **apresenta**, quem decide sou eu.
- Se dois fornecedores parecem cotar produtos diferentes (spec ligeiramente diferente), avisa — pode não ser comparação apple-to-apple.
- Se algum PDF estiver ilegível ou parcial, avisa qual e onde.
- Português-BR, sem "solução", "parceria estratégica" e afins. Comercial direto.

---

*Prompt versão 1.0 · PDL Mallory 2026 · M5 T2 · Caso 6*
