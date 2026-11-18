# US07 - Baixar lições para estudar sem internet

Categoria: RSD / Backlog v2
Prioridade: Média
Rastreabilidade Ética: UE07, UE19

<aside>
💡

*"Como estudante, quero baixar lições compatíveis com uso offline, para estudar mesmo quando estiver sem conexão."*

</aside>

# Goals

- Viabilizar o estudo em locais sem acesso constante à internet.

### Context

- Estudantes em deslocamento ou áreas com conectividade limitada ficam impedidos de estudar.

# Story

When o estudante solicita o download de uma lição compatível e conclui com sucesso, Then a lição é marcada como disponível offline.

# Requirements

**Functional requirements**

- Iniciar download de pacote de lição; confirmar conclusão ou informar falha; permitir remoção do armazenamento local.

**Non-Functional requirements**

- Transparência sobre o que funciona offline (UE07); armazenamento local seguro sem dados pessoais desnecessários (UE19).

**Out of Scope**

- Sincronização automática em segundo plano não configurada.

# Acceptance Criteria

**Scenario Principal:**

- Given conexão disponível, When baixar lição compatível com sucesso, Then ela é identificada como disponível offline.
