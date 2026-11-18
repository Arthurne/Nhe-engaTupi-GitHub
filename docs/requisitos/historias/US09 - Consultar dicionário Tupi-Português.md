# US09 - Consultar dicionário Tupi-Português

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE09, UE21

<aside>
💡

*"Como estudante, quero pesquisar palavras em um dicionário Tupi-Português, para consultar seus significados e informações complementares disponíveis."*

</aside>

# Goals

- Oferecer ferramenta rápida de consulta lexical com contexto e variantes.

### Context

- Estudantes precisam verificar rapidamente o significado e o contexto de uso de palavras encontradas.

# Story

When o estudante pesquisa um termo no dicionário, Then o sistema exibe significado, contexto, variante e fonte quando disponíveis.

# Requirements

**Functional requirements**

- Campo de busca; exibição de significado, contexto, variante e fonte; mensagem clara para busca sem resultado.

**Non-Functional requirements**

- Contextualização linguística sem atribuir significado único universal (UE09); sinalização de incertezas (UE21).

**Out of Scope**

- Tradução automática de textos longos.

# Acceptance Criteria

**Scenario Principal:**

- Given termo existente no dicionário, When realizar busca na Tela 5, Then exibe significado e contexto/fonte.
