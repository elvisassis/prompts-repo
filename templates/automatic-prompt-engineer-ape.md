# 📝 Automatic Prompt Engineer (APE)

## Descrição
Utiliza um LLM para **gerar, testar e selecionar o melhor prompt de instrução** para uma tarefa específica. Em vez de o humano criar o prompt, um LLM de "nível superior" experimenta e otimiza automaticamente o prompt para maximizar o desempenho.

## Estrutura do Prompt (Conceitual)
**Exemplo (Prompt APE):**
- Dado um conjunto de dados de "Revisão de Produtos" e o resultado esperado de "Classificação de Sentimento", gere 5 prompts de instrução diferentes para a tarefa. Teste-os e retorne o prompt que obteve a maior precisão.

## Resultado Esperado (Prompt Otimizado)
- O prompt **"Classifique esta revisão estritamente como POSITIVA ou NEGATIVA e justifique brevemente sua decisão."** teve uma taxa de acerto de 92%.