# 📝 Tree of Thought (ToT)

## Descrição
Ao invés de um único caminho linear de raciocínio (CoT), o ToT explora múltiplos "pensamentos" ou "ramificações" simultaneamente, como um **nó de árvore**. A cada etapa do problema, o modelo gera várias opções de raciocínio e usa um processo de "poda" ou "votação" para escolher a ramificação mais promissora para o próximo passo. É ideal para problemas de planejamento e criatividade.

## Estrutura do Prompt
**Exemplo:**
- Gere 3 opções de títulos para uma campanha de marketing sobre eficiência energética. Avalie a eficácia e o público-alvo de cada título, escolhendo o melhor.

## Resultado Esperado (Conceitual)
- **Nível 1 (Geração de Ideias):**
    - **Opção A:** "Apague a Luz e Salve o Planeta."
    - **Opção B:** "Sua Conta de Luz Pode Ser Menor: Guia Rápido."
    - **Opção C:** "Energia Inteligente: O Futuro da Sua Casa."
- **Nível 2 (Avaliação):**
    - A: Muito genérico. Público: Crianças/Geral.
    - B: Foco em economia (dinheiro). Público: Adultos preocupados com orçamento.
    - C: Foco em tecnologia e longo prazo. Público: Proprietários de casa, entusiastas de tecnologia.
- **Resposta Final (Melhor Ramo):** Opção C. É aspiracional, foca na modernidade e tem um apelo duradouro para proprietários.