
### 📘 Descrição dos Diretórios

| Diretório | Descrição |
|------------|------------|
| **.github/** | Contém templates para Issues e Pull Requests, garantindo consistência nas contribuições. |
| **prompts/** | Diretório principal com todos os prompts organizados por tipo, modelo e categoria. |
| **templates/** | Modelos reutilizáveis para criação de novos prompts (como few-shot e chain-of-thought). |
| **scripts/** | Scripts utilitários, como testes automáticos de prompts e upload para plataformas externas. |
| **LICENSE** | Define os termos de uso e redistribuição dos prompts. |
| **CONTRIBUTING.md** | Guia detalhado para contribuir com o repositório. |
| **README.md** | Este arquivo — documentação principal do projeto. |

---

## 🧩 Estrutura dos Arquivos de Prompt

Cada arquivo `.md` de prompt segue um formato padronizado para manter consistência e facilitar o uso:

```markdown
---
name: Nome Descritivo do Prompt
model: [gpt-3.5, gemini-pro, stable-diffusion, dall-e]
category: [categoria-principal, sub-categoria]
tags: [tag1, tag2, tag3]
complexity: [easy, medium, hard]
version: 1.0.0
---

# Título do Prompt

## 📝 Descrição
Breve resumo do que o prompt faz e seu propósito.

## 🚀 Instruções (Prompt em si)

## 💡 Exemplo de Uso
    - prompt-exemplo = "Escreva um poema sobre {{TEMA}} em estilo - --  {ESTILO}}."
    - input_tema = "a natureza"
    - input_estilo = "haicai"


## 🧾 Exemplo de Saída
(Aqui pode ser incluído um exemplo gerado pelo modelo.)

## 🧠 Notas Adicionais
Dicas e variações para otimizar o uso do prompt.
