# 📝 Tree of Thought (ToT)

## Descrição
Ao invés de um único caminho linear de raciocínio (CoT), o ToT explora múltiplos "pensamentos" ou "ramificações" simultaneamente, como um **nó de árvore**. A cada etapa do problema, o modelo gera várias opções de raciocínio e usa um processo de "poda" ou "votação" para escolher a ramificação mais promissora para o próximo passo. É ideal para problemas de planejamento e criatividade.

## Estrutura do Prompt (Exemplo Prático)

- **Prompt do Usuário:** "Estou planejando um jantar para três amigos. Um é vegetariano, o outro tem alergia a glúten e o terceiro não come carne de porco. Crie um menu completo (entrada, prato principal e sobremesa) que todos possam comer. Explore 3 ideias de prato principal e avalie qual é a melhor."

## Simulação da Resposta (ToT)

### Nível 1: Geração de Ideias (Prato Principal)
O modelo gera três possíveis caminhos para o prato principal, que é a parte mais complexa.

- **Ramo 1 (Ideia):** Risoto de Cogumelos com aspargos.
- **Ramo 2 (Ideia):** Moqueca de Banana da Terra com arroz e farofa de dendê.
- **Ramo 3 (Ideia):** Lasanha de abobrinha com ricota e espinafre.

### Nível 2: Avaliação e "Poda"
O modelo avalia a viabilidade e o apelo de cada ramo.

- **Avaliação do Ramo 1 (Risoto):**
  - *Prós:* Naturalmente sem glúten (se usar arroz arbóreo puro), vegetariano e sem porco. Prato sofisticado.
  - *Contras:* Requer atenção constante no preparo.
- **Avaliação do Ramo 2 (Moqueca):**
  - *Prós:* Prato criativo, saboroso, naturalmente sem glúten, vegetariano e sem porco.
  - *Contras:* O sabor do dendê pode ser muito forte para alguns paladares.
- **Avaliação do Ramo 3 (Lasanha):**
  - *Prós:* Saudável, vegetariano e sem porco.
  - *Contras:* A ricota pode conter glúten dependendo da marca (risco de contaminação cruzada). A montagem pode ser trabalhosa.

- **Decisão (Poda):** O Ramo 1 (Risoto) e o Ramo 2 (Moqueca) são os mais promissores. O Ramo 3 é descartado pelo risco de glúten e complexidade. O modelo escolhe o **Ramo 1** como o mais seguro e universalmente agradável.

### Nível 3: Construção da Resposta Final (Usando o Melhor Ramo)
Com o prato principal decidido, o modelo constrói o menu completo ao redor dele.

- **Resposta Final:**
  "Aqui está um menu delicioso e seguro para todos os seus convidados:
  - **Entrada:** Salada caprese no palito (tomate cereja, mussarela de búfala, manjericão e molho pesto).
  - **Prato Principal:** Risoto de cogumelos frescos com lascas de aspargos e finalizado com azeite trufado.
  - **Sobremesa:** Mousse de maracujá."