# 📝 Assistente de Fórmulas Excel

## Descrição
Este prompt é usado para solicitar ao modelo a criação, explicação ou depuração de fórmulas e funções para o Microsoft Excel ou Google Sheets, focando na lógica necessária para processar dados.

## Estrutura do Prompt
**Exemplo:**
- Gere uma fórmula do Excel que conte o número de células na coluna C que contêm a palavra "Pendente" E cujo valor correspondente na coluna D seja maior que 1000.

## Resultado Esperado
- `=CONT.SE.S(C:C,"*Pendente*", D:D, ">1000")`