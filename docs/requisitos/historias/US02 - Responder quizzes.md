# US02 - Responder quizzes

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE04, UE20

<aside>
💡

*"Como estudante, quero responder quizzes relacionados às lições, para verificar minha compreensão e receber retorno sobre minhas respostas."*

</aside>

# Goals

- Permitir prática ativa e fixação do vocabulário estudado nas lições.

### Context

- Apenas ler conteúdo passivamente reduz a retenção; o estudante precisa testar o aprendizado sem constrangimento.

# Story

When o estudante responde a uma pergunta do quiz e confirma, Then o sistema valida a resposta e exibe feedback explicativo e respeitoso.

# Requirements

**Functional requirements**

- Exibir enunciado e alternativas; diferenciar acerto e erro; permitir nova tentativa ou explicação; apresentar resultado final.

**Non-Functional requirements**

- Feedback respeitoso sem mensagens humilhantes (UE04); explicação educativa das respostas (UE20).

**Out of Scope**

- Ranking competitivo público entre estudantes.

# Acceptance Criteria

**Scenario Principal:**

- Given um quiz iniciado, When selecionar alternativa incorreta e confirmar, Then o sistema informa respeitosamente e apresenta explicação.
