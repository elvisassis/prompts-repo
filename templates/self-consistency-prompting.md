# 📝 Self-consistency (Auto-consistência)

## Descrição
O prompt é executado **várias vezes** com diferentes caminhos de raciocínio (Chain-of-Thought) para a mesma pergunta. Depois, os resultados são **agregados** e a resposta mais frequente ou consistente entre as diversas execuções é selecionada como a resposta final. Aumenta a confiabilidade do resultado, especialmente em problemas de raciocínio e matemática.

## Estrutura do Prompt

- **Pergunta:** "Se uma caixa contém 12 maçãs e 8 laranjas, e você adiciona mais 5 maçãs e retira 3 laranjas, quantas frutas no total estão na caixa? Pense passo a passo em 3 formas diferentes."

## Resultado e Análise (Exemplo Prático)

### Execução 1 (Raciocínio Correto)
- **Caminho 1:**
  1. Maçãs iniciais: 12
  2. Laranjas iniciais: 8
  3. Total inicial: 12 + 8 = 20 frutas.
  4. Adiciona 5 maçãs: 20 + 5 = 25 frutas.
  5. Retira 3 laranjas: 25 - 3 = 22 frutas.
- **Resposta 1:** 22

### Execução 2 (Raciocínio com Erro)
- **Caminho 2:**
  1. Maçãs: 12 + 5 = 17.
  2. Laranjas: 8 - 3 = 5.
  3. Total: 17 + 5 = 22.
  4. (Erro de interpretação) O modelo esqueceu de somar as laranjas no início e somou no final.
- **Resposta 2:** 22

### Execução 3 (Raciocínio Correto, outra ordem)
- **Caminho 3:**
  1. Maçãs finais: 12 + 5 = 17 maçãs.
  2. Laranjas finais: 8 - 3 = 5 laranjas.
  3. Total final: 17 + 5 = 22 frutas.
- **Resposta 3:** 22

### Agregação e Resposta Final
- **Respostas obtidas:** [22, 22, 22]
- **Votação:** A resposta "22" aparece 3 de 3 vezes.
- **Resposta Final Consistente:** 22