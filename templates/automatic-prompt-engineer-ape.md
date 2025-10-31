# 📝 Automatic Prompt Engineer (APE)

## Descrição
Utiliza um LLM para **gerar, testar e selecionar o melhor prompt de instrução** para uma tarefa específica. Em vez de o humano criar o prompt, um LLM de "nível superior" experimenta e otimiza automaticamente o prompt para maximizar o desempenho.

## Estrutura do Prompt (Exemplo Prático)

- **Prompt do Usuário (para o APE):**
  "Preciso de um prompt para extrair o nome do produto e o principal defeito de reclamações de clientes.
  **Exemplos de input/output:**
  - *Input:* 'A tela do meu celular novo, o Galaxy S25, quebrou sem motivo.' -> *Output:* `{"produto": "Galaxy S25", "defeito": "tela quebrou"}`
  - *Input:* 'A bateria do notebook FireBook não dura nada, mal consigo usar por 2 horas.' -> *Output:* `{"produto": "FireBook", "defeito": "bateria não dura"}`

  Gere 5 prompts candidatos, teste-os com os exemplos e me diga qual é o melhor."

## Simulação da Resposta (APE)

### 1. Geração de Prompts Candidatos
O modelo APE gera várias abordagens para a mesma tarefa.

1.  **Prompt 1 (Básico):** "Extraia o produto e o defeito do texto."
2.  **Prompt 2 (Com Formato):** "Analise a reclamação e retorne o produto e o defeito em formato JSON: `{\"produto\": \"nome\", \"defeito\": \"descrição\"}`."
3.  **Prompt 3 (Persona):** "Você é um analista de suporte. Leia a reclamação, identifique o produto e o principal problema."
4.  **Prompt 4 (Few-Shot no Prompt):** "Dado o texto, extraia o produto e o defeito. Exemplo: 'O mouse X parou de funcionar' -> `{\"produto\": \"Mouse X\", \"defeito\": \"parou de funcionar\"}`. Agora, analise a seguinte reclamação:..."
5.  **Prompt 5 (Detalhado):** "Leia a reclamação do cliente. Identifique o nome exato do produto mencionado. Em seguida, resuma o principal defeito ou problema relatado em poucas palavras."

### 2. Teste e Avaliação (Simulado)
O APE testa cada prompt com os dados fornecidos e avalia a precisão.

- **Prompt 1:** Falhou em 1 de 2 (não formatou como JSON).
- **Prompt 2:** Sucesso em 2 de 2.
- **Prompt 3:** Falhou em 2 de 2 (retornou texto livre, não JSON).
- **Prompt 4:** Sucesso em 2 de 2.
- **Prompt 5:** Falhou em 1 de 2 (não formatou como JSON).

### 3. Seleção do Melhor Prompt

- **Resposta Final do APE:**
  "O melhor prompt para sua tarefa é o **Prompt 2**:
  `Analise a reclamação e retorne o produto e o defeito em formato JSON: {\"produto\": \"nome\", \"defeito\": \"descrição\"}`.
  Ele teve 100% de acerto nos testes e é claro e direto."