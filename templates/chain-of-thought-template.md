# 📝 Chain-of-Thought (CoT) Prompting

## Descrição
Instrui o modelo a gerar uma série de passos de raciocínio lógico (**cadeia de pensamento**) antes de fornecer a resposta final. Adicionar a frase "Pense passo a passo" ou similar melhora significativamente o desempenho do modelo em tarefas que exigem raciocínio complexo, matemática ou lógica.

## Estrutura do Prompt
**Exemplo:**
- Um trem sai de São Paulo às 10h00 e viaja a 80 km/h. Outro trem sai do Rio de Janeiro às 11h00 e viaja a 100 km/h na mesma linha em sentido oposto. As cidades estão separadas por 400 km. Pense passo a passo e diga a que horas eles se encontrarão.

## Resultado Esperado
- **Pensamento:** 1. O primeiro trem viaja 80km na primeira hora (até as 11h00).
    2. A distância restante é $400 - 80 = 320$ km.
    3. A velocidade combinada é $80 + 100 = 180$ km/h.
    4. O tempo para se encontrarem a partir das 11h00 é $320 / 180 \approx 1.77$ horas (ou 1 hora e 46 minutos).
    5. O encontro será $\text{11h00} + \text{1h46m} = \text{12h46m}$.
- **Resposta Final:** Eles se encontrarão às 12h46.