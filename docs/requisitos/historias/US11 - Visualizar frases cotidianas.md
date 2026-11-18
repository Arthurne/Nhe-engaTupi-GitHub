# US11 - Visualizar frases cotidianas

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE11, UE12, UE25

<aside>
💡

*"Como estudante, quero consultar frases cotidianas organizadas por categoria, para conhecer exemplos de expressões e seus contextos de uso."*

</aside>

# Goals

- Apresentar exemplos práticos de uso da língua em situações do dia a dia.

### Context

- Aprender expressões situacionais facilita a compreensão prática do idioma.

# Story

When o estudante seleciona uma categoria de frases, Then visualiza expressões com tradução e contexto de uso validados.

# Requirements

**Functional requirements**

- Filtrar frases por categoria; exibir frase, tradução e nota de contexto/fonte; bloquear publicação de frases não validadas.

**Non-Functional requirements**

- Contexto cultural adequado sem inventar expressões (UE11); respeito cultural e fontes confiáveis (UE12, UE25).

**Out of Scope**

- Chat aberto entre usuários.

# Acceptance Criteria

**Scenario Principal:**

- Given categoria selecionada na Tela 6, When abrir, Then exibe frases validadas com tradução e contexto.

**Cenário alternativo: frase sem validação adequada**

- **Dado** que uma expressão ainda não foi validada por fonte adequada
- **Quando** o conteúdo for preparado para publicação
- **Então** a expressão não deve ser apresentada como autêntica ou definitiva até que a validação necessária seja realizada
