# US05 - Acompanhar progresso

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE01, UE14, UE24

<aside>
💡

*"Como estudante, quero visualizar meus registros de aprendizagem, para acompanhar as lições e atividades concluídas."*

</aside>

# Goals

- Permitir monitoramento individual e privado da evolução nos estudos.

### Context

- Acompanhar o avanço ajuda a manter a rotina, mas indicadores mal explicados podem gerar falsa impressão de fluência.

# Story

When o estudante acessa a área de progresso, Then o sistema exibe lições concluídas e explica que conclusão não significa fluência.

# Requirements

**Functional requirements**

- Exibir registros de atividades concluídas; atualizar indicadores após conclusão; explicar significado dos indicadores.

**Non-Functional requirements**

- Privacidade por padrão (UE01); distinção clara entre conclusão e fluência (UE14); compartilhamento apenas com consentimento (UE24).

**Out of Scope**

- Certificação oficial de fluência linguística.

# Acceptance Criteria

**Scenario Principal:**

- Given atividades concluídas, When abrir a Tela 7 (Progresso), Then os registros são exibidos de forma privada e com nota explicativa.
