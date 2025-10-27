# 🤝 Guia de Contribuição

Obrigado por contribuir com este repositório de **prompts versionados!**  
Nosso objetivo é manter uma coleção organizada, reutilizável e padronizada de prompts voltados para **IA, automação e desenvolvimento de software**.

---

## 🧩 Como contribuir

### 1️⃣ Faça um fork do repositório
Clique em **Fork** no canto superior direito do GitHub para criar uma cópia do repositório na sua conta.

---

### 2️⃣ Crie um branch para sua contribuição
**Crie um branch descritivo antes de realizar alterações:**

- git checkout -b feat/novo-prompt-spring-security

**Use prefixos para indicar o tipo de alteração:**

 - feat/ → nova funcionalidade ou prompt

- fix/ → correção de erro

- docs/ → documentação

- refactor/ → melhorias estruturais sem alterar funcionalidade

✍️ Estrutura de um novo prompt Cada prompt deve seguir o modelo padrão e estar em Markdown (.md).

Exemplo:

# 🧩 Prompt – Spring Boot Authentication

**Objetivo:** auxiliar na criação e validação de autenticação customizada no Spring Boot 3.

---

### 🎯 Contexto
O prompt será utilizado por desenvolvedores que desejam configurar múltiplos `AuthenticationProviders com `@PreAuthorize`.

---

### 💬 Prompt
> Você é um especialista em Spring Security.  
> Ajude a criar uma configuração que suporte múltiplos provedores de autenticação (header, form, OAuth2).

---

### ✅ Exemplos de uso
- “Crie um `CustomAuthenticationFilter` com validação de token.”
- “Explique como registrar múltiplos `AuthenticationProviders`.”

---

### 📚 Referências
- [Spring Security Docs](https://docs.spring.io/spring-security/)

# Estrutura de Diretórios para Prompts

|  Onde colocar seu prompt                     | Diretório                      |
|-----------------------------------------------|--------------------------------|
| Prompts para ChatGPT                           | prompts/ai/chatgpt/            |
| Prompts para Gemini                            | prompts/ai/gemini/             |
| Templates genéricos (feature, bug, etc.)      | prompts/templates/             |
| Ideias experimentais                           | prompts/experiments/           |

## 🧱 Padrões e estilo
- Siga o formato descrito em `docs/STYLE_GUIDE.md`.
- Nomeie os arquivos seguindo `docs/NAMING_CONVENTIONS.md`.
- Prefira títulos claros e objetivos: `spring-boot-authentication.md` em vez de `prompt1.md`.
- Sempre escreva em **português** (exceto prompts projetados para inglês).
- Inclua exemplos práticos de uso do prompt.

## 📝 Teste localmente antes de abrir PR
Antes de enviar seu Pull Request:

1. Verifique se o Markdown está bem formatado.
2. Teste o prompt no modelo de IA (ChatGPT, Gemini, etc.).
3. Assegure-se de que o prompt produz o resultado esperado.
