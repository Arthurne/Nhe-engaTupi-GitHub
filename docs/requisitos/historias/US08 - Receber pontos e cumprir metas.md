# US08 - Receber pontos e cumprir metas

Categoria: RSD / Backlog v2
Prioridade: Média
Rastreabilidade Ética: UE08, UE18, UE23

<aside>
💡

*"Como estudante, quero acompanhar pontos e metas de estudo, para visualizar minha evolução e organizar minha rotina de aprendizagem."*

</aside>

# Goals

- Incentivar a constância nos estudos de forma saudável e autônoma.

### Context

- Gamificação agressiva gera culpa e abandono quando o estudante precisa fazer pausas.

# Story

When o estudante conclui atividade elegível ou ajusta sua meta diária, Then o sistema atualiza pontos/meta sem mensagens punitivas.

# Requirements

**Functional requirements**

- Atribuir pontos por atividade elegível; permitir ajuste de meta; rejeitar metas inválidas com explicação.

**Non-Functional requirements**

- Gamificação sem pressão excessiva (UE08); metas ajustáveis à rotina (UE18); regras transparentes (UE23).

**Out of Scope**

- Punição por perda de ofensiva/streak.

# Acceptance Criteria

**Scenario Principal:**

- Given meta configurável, When alterar para valor permitido, Then o sistema salva sem mensagens punitivas.
