# 🔹 Few-Shot Prompt Template

# 🔹 Few-Shot Prompt Template

## Descrição
Este template fornece ao modelo alguns exemplos antes de pedir a resposta. Isso ajuda o modelo a entender o padrão desejado e gerar respostas mais consistentes.

## Estrutura do Prompt

### Exemplo 1: Tradução Simples

- **Instrução:** Forneça alguns exemplos de tradução para ensinar o padrão.

- **Prompt:**
  - Traduza "Hello" para francês -> "Bonjour"
  - Traduza "Goodbye" para francês -> "Au revoir"
  - Agora complete:
  - Traduza "Thank you" para francês ->

- **Resultado Esperado:** "Merci"

### Exemplo 2: Classificação e Extração em Formato JSON

- **Instrução:** Ensine o modelo a classificar o sentimento de uma frase e extrair a palavra-chave, retornando a saída em formato JSON.

- **Prompt:**
  - **Frase:** "Amei o novo celular, a câmera é incrível!"
  - **Análise:** `{"sentimento": "positivo", "palavra_chave": "câmera"}`

  - **Frase:** "O serviço de entrega demorou muito e o produto veio errado."
  - **Análise:** `{"sentimento": "negativo", "palavra_chave": "entrega"}`

  - **Frase:** "A bateria do notebook dura o dia todo, mas o teclado é um pouco barulhento."
  - **Análise:**

- **Resultado Esperado:** `{"sentimento": "misto", "palavra_chave": "bateria"}`
