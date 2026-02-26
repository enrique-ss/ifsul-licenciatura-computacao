# (TÍTULO) Matemática Discreta

**Data:** 25/02/2026
**Professor:** Davi

---

## (CONTEÚDO) Representações de Dados: Analógico vs. Digital

### Gráfico Contínuo × Gráfico Pontilhado

- **Gráfico contínuo**: a linha é ininterrupta, representando grandezas que variam de forma suave, sem saltos. Corresponde a funções definidas sobre os números reais. Ex: temperatura ao longo do dia, velocidade de um carro.
- **Gráfico pontilhado (discreto)**: os dados existem apenas em pontos isolados, sem valores entre eles. Corresponde a funções definidas sobre conjuntos discretos, como os naturais. Ex: número de alunos por turma, quantidade de bits.

### Analógico × Digital

- **Analógico**: sinal contínuo, com infinitos valores possíveis entre dois pontos. Representado por um gráfico contínuo. Ex: voz humana, rádio AM/FM.
- **Digital**: sinal discreto, com apenas dois estados possíveis: **0 e 1** (binário). É a linguagem dos computadores.

> 💬 **Minha pergunta em aula:** Questionei o professor Davi se HD e SSD se encaixam nesses exemplos.

> **Resposta:** O prof. Davi disse que não sabia. A pergunta gerou debate entre os colegas próximos, mas ficou em aberto, vale investigar.

---

## (CONTEÚDO) Lógica Proposicional

### O que é uma Proposição?

Uma **proposição** (ou sentença declarativa) é toda afirmação que pode ser classificada como **verdadeira (V)** ou **falsa (F)**, nunca os dois ao mesmo tempo. Esse princípio vem da filosofia (Aristóteles): o **princípio da não-contradição**.

- **Proposição simples**: possui um único valor lógico. Ex: "2 + 2 = 4" (V), "A Terra é plana" (F).
- **Proposição composta**: formada pela combinação de proposições simples usando conectivos lógicos.

### Conectivos Lógicos

| Símbolo    | Palavras equivalentes  | Nome          | Regra                                  |
|------------|------------------------|---------------|----------------------------------------|
| **∧** (^)  | e, and, &              | Conjunção     | V somente se **ambas** forem V         |
| **∨** (v)  | ou, or, \|\|           | Disjunção     | V se **pelo menos uma** for V          |
| **→**      | então, implica         | Condicional   | F apenas quando P = V e Q = F          |
| **↔**      | se e somente se, iff   | Bicondicional | V quando as duas têm o **mesmo** valor |
| **¬** (~)  | não, else              | Negação       | **Inverte** o valor lógico             |

> ⚠️ O símbolo `^` é usado na notação informal/programação para conjunção. Formalmente, o símbolo correto é **∧**.

### Disjunção Inclusiva × Exclusiva

- **Ou inclusivo (∨)**: escolher uma alternativa **não exclui** a outra. Ex: "Você pode pedir café ou chá", pode pedir os dois. É o padrão da lógica formal.
- **Ou exclusivo (XOR, ⊕)**: escolher **uma ou outra**, nunca ambas. Ex: "Vire à esquerda ou à direita". Em programação representado por `^`.

---

## (CONTEÚDO) Tabela-Verdade

O **estudo de possibilidades**: verificação sistemática de todos os valores que uma proposição composta pode assumir.

O número de linhas segue a fórmula **2ⁿ**, onde *n* é o número de proposições simples:

| Proposições | Linhas |
|-------------|--------|
| 1           | 2¹ = 2 |
| 2           | 2² = 4 |
| 3           | 2³ = 8 |
| n           | 2ⁿ     |

### Exemplo: P ∧ Q e P ∨ Q

| P | Q | P ∧ Q | P ∨ Q |
|---|---|-------|-------|
| V | V | **V** | **V** |
| V | F | F     | **V** |
| F | V | F     | **V** |
| F | F | F     | F     |

---

## (DÚVIDAS)

**1) A negação só se aplica a proposições simples?**
Não. A negação pode ser aplicada a proposições compostas inteiras. Por exemplo, ¬(P ∧ Q) nega o resultado da conjunção, não cada parte individualmente. Isso leva às **Leis de De Morgan**: ¬(P ∧ Q) ≡ ¬P ∨ ¬Q.

**2) Qual a diferença prática entre → e ↔?**
O condicional P → Q é uma implicação de mão única: "se P, então Q". O bicondicional P ↔ Q exige equivalência nos dois sentidos: "P se e somente se Q". Em programação, o condicional aparece nos `if`s; o bicondicional é equivalente ao operador de igualdade (`==`) em contexto lógico.

---

## (OBSERVAÇÕES PESSOAIS)

A aula conectou bem a parte visual (gráficos contínuos vs. pontilhados) com a abstração da lógica discreta. Faz sentido que a computação seja toda discreta, bits são exatamente isso: valores isolados, V ou F, 0 ou 1.

A pergunta sobre HD vs. SSD ficou em aberto, o prof. Davi não soube responder na hora, mas gerou um debate interessante com os colegas. Vale pesquisar depois.

Os conectivos lógicos são os operadores booleanos que já aparecem na programação (`&&`, `||`, `!`, `==`). A notação matemática é diferente, mas a lógica é a mesma, isso facilita bastante.