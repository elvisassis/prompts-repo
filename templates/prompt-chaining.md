# 📝 Prompt Chaining

## Descrição
Envolve quebrar uma tarefa complexa em **múltiplas etapas sequenciais**, onde a saída de um prompt se torna o contexto ou a entrada para o prompt seguinte. Isso permite que o modelo lide com tarefas muito grandes ou multifacetadas de forma mais controlada.

## Estrutura do Prompt
**Exemplo (Prompt 1 de 3):**
- Gere 5 tópicos principais para um e-book sobre "Trabalho Remoto".

**Exemplo (Prompt 2 de 3):**
- Com base nos tópicos gerados no Passo 1, crie um subtítulo de 1 linha para cada um dos 5 tópicos.

**Exemplo (Prompt 3 de 3):**
- Usando o Tópico 1 e seu subtítulo (gerados nos passos 1 e 2), escreva um parágrafo introdutório de 5 linhas.

## Resultado Esperado
- (Continuação do processo passo a passo, como a geração do parágrafo final)