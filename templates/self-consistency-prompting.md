# 📝 Self-consistency (Auto-consistência)

## Descrição
O prompt é executado **várias vezes** com diferentes caminhos de raciocínio (Chain-of-Thought) para a mesma pergunta. Depois, os resultados são **agregados** e a resposta mais frequente ou consistente entre as diversas execuções é selecionada como a resposta final. Aumenta a confiabilidade do resultado, especialmente em problemas de raciocínio e matemática.

## Estrutura do Prompt
**Exemplo:**
- Calcule $(15 \times 3) + 7$. Gere **três** caminhos de raciocínio diferentes e selecione a resposta que aparece mais vezes.

## Resultado Esperado (Conceitual)
- **Caminho 1:** $15 \times 3 = 45$. $45 + 7 = 52$.
- **Caminho 2:** $15 + 7 = 22$. Não, o modelo deve seguir a ordem das operações.
- **Caminho 3:** $15 \times 3 = 45$. $45 + 7 = 52$.
- **Caminho 4:** $15 \times 3 = 45$. $45 + 7 = 52$.
- **Resposta Selecionada (Consistente):** 52 (Com base na maioria dos caminhos corretos).