# 📝 Retrieval Augmented Generation (RAG)

## Descrição
O sistema **busca ("retrieval")** informações em uma base de dados externa (documentos, artigos, banco de dados proprietário) e **anexa este contexto** ao prompt do usuário. O LLM, então, usa esse novo contexto para **gerar ("generation")** uma resposta fundamentada, reduzindo alucinações e fornecendo dados atualizados.

## Estrutura do Prompt
**Exemplo:**
- **[Contexto Anexado pelo Sistema]:** "A nova Política de Férias da Empresa X (2025) estabelece que todos os funcionários têm direito a 30 dias após 1 ano e um bônus de 1/3 do salário. O período de aviso prévio para solicitação é de 60 dias."
- **[Pergunta do Usuário]:** De acordo com a nova política, qual o bônus de férias e com quanto tempo de antecedência devo avisar?

## Resultado Esperado
- De acordo com a Política de Férias (2025), o bônus de férias é de **1/3 do seu salário** e você deve solicitar com **60 dias** de aviso prévio.