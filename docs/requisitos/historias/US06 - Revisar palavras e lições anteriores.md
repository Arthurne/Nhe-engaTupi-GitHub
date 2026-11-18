# US06 - Revisar palavras e lições anteriores

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE10

<aside>
💡

*"Como estudante, quero reabrir palavras e lições que já estudei, para revisar conteúdos e retomar minha aprendizagem."*

</aside>

# Goals

- Facilitar a revisão periódica de conteúdos já estudados sem expor dificuldades.

### Context

- Sem revisão estruturada, o estudante esquece vocabulário aprendido anteriormente.

# Story

When o estudante acessa a área de revisão e seleciona uma lição concluída, Then o sistema reabre o conteúdo de forma privada.

# Requirements

**Functional requirements**

- Listar palavras e lições concluídas; permitir reabertura imediata; informar quando o histórico estiver vazio.

**Non-Functional requirements**

- Revisão privada por padrão sem exposição de erros anteriores (UE10).

**Out of Scope**

- Publicação automática de erros em feed social.

# Acceptance Criteria

**Scenario Principal:**

- Given lição concluída anteriormente, When selecionar na Tela 4 (Revisão), Then o conteúdo é reaberto.

**Cenário alternativo: histórico vazio**

- **Dado** que a pessoa usuária ainda não concluiu lições nem possui palavras registradas
- **Quando** acessar a área de revisão
- **Então** o sistema deve informar que não há conteúdos para revisar
