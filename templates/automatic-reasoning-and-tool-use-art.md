# 📝 Automatic Reasoning and Tool-use (ART)

## Descrição
Uma técnica que automatiza a geração de um **plano de raciocínio (CoT)** e, em seguida, decide e executa o uso de **ferramentas externas** (como código Python, calculadora ou APIs de busca/clima) para auxiliar na resposta. O LLM atua como um 'agente' que pensa e interage com o ambiente.

## Estrutura do Prompt
**Exemplo:**
- Calcule a média de temperatura dos últimos 7 dias em Lavras, MG, e sugira a melhor roupa para amanhã. (O modelo deve usar uma ferramenta de busca/clima).

## Resultado Esperado
- **Raciocínio:** 1. Preciso usar a Ferramenta de Busca para obter as temperaturas dos últimos 7 dias em Lavras, MG. 2. Calculo a média. 3. Uso a previsão de amanhã e a média para sugerir a roupa.
- **Ferramenta de Busca:** Temperaturas: [25, 27, 24, 26, 28, 27, 25]. Previsão para amanhã: 29ºC.
- **Cálculo:** Média de $26$ºC.
- **Resposta Final:** A temperatura média dos últimos 7 dias foi de 26ºC. Como a previsão para amanhã é de 29ºC, sugiro roupas leves, como camiseta e shorts.