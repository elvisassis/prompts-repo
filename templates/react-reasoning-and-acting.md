# 📝 ReAct (Reasoning and Acting)

## Descrição
Combina **Raciocínio (Reasoning)** e **Ação (Acting)** em um ciclo iterativo. O modelo gera um pensamento CoT (Raciocínio) para planejar, e então executa uma Ação (como usar uma ferramenta de busca ou código). O resultado da Ação é observado e alimenta o próximo ciclo de Raciocínio, até que a resposta final seja dada.

## Estrutura do Prompt
**Exemplo:**
- Quem foi o vencedor do último Campeonato Mundial de Fórmula 1 e qual a capital do país dele? (Requer o uso de uma ferramenta de Busca).

## Resultado Esperado (Formato ReAct)
- **Pensamento:** Preciso descobrir quem venceu o último Campeonato de F1 e qual é o país dele.
- **Ação:** Busca[Vencedor do último Campeonato Mundial de Fórmula 1]
- **Observação:** O vencedor foi Max Verstappen, que é holandês.
- **Pensamento:** Agora preciso saber a capital da Holanda.
- **Ação:** Busca[Capital da Holanda]
- **Observação:** A capital da Holanda é Amsterdã.
- **Resposta Final:** O vencedor foi Max Verstappen, e a capital do seu país (Holanda) é Amsterdã.