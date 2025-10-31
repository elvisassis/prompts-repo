# 📝 Basic Prompt Template

# 📝 Basic Prompt Template

## Descrição
Este template é a forma mais fundamental de interação com um LLM. Ele consiste em dar uma instrução direta e clara para o modelo, sem o uso de exemplos (`few-shot`) ou passos de raciocínio complexos (`Chain-of-Thought`).

**✅ Cenários Ideais:**
- **Tarefas de baixa complexidade:** Resumir um texto curto, traduzir uma frase, gerar ideias (brainstorming).
- **Respostas rápidas e diretas:** Quando você precisa de uma informação específica sem um processo de análise profundo.
- **Início de uma exploração:** Usar um prompt básico para obter uma resposta inicial e, a partir dela, refinar com prompts mais complexos.

**❌ Limitações (Quando não usar):**
- **Problemas de múltiplos passos:** Tarefas que exigem raciocínio lógico, cálculo ou planejamento (use `Chain-of-Thought` ou `ReAct`).
- **Formatação de saída específica:** Quando você precisa que a resposta siga um padrão rigoroso, como JSON (use `Few-Shot` para ensinar o formato).
- **Tarefas que exigem conhecimento profundo e específico:** Para isso, `RAG` (Retrieval Augmented Generation) é mais indicado.

## Estrutura do Prompt
**Exemplo:**
- Gere uma lista de 5 ideias criativas para nomes de uma nova startup de tecnologia voltada para sustentabilidade.

## Resultado Esperado
- EcoTech Solutions
- Green Innovators
- SustainaLabs
- TerraTech
- FutureEco
