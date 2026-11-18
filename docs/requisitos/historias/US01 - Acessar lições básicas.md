# US01 - Acessar lições básicas

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE02, UE15, UE22

<aside>
💡

*"Como estudante, quero acessar lições básicas de Tupi organizadas para aprendizagem progressiva, para estudar vocabulário e conteúdos introdutórios."*

</aside>

# Goals

- Oferecer trilha introdutória estruturada em etapas curtas para iniciantes na língua Tupi.

### Context

- Pessoas iniciantes enfrentam dificuldade com materiais dispersos e sem progressão didática.

# Story

When o estudante abre a área de aprendizagem e seleciona uma lição publicada, Then o sistema exibe o conteúdo da lição e permite avançar entre etapas.

# Requirements

**Functional requirements**

- Listar lições disponíveis; exibir conteúdo da lição selecionada; informar de forma clara quando não houver lições publicadas.

**Non-Functional requirements**

- Navegação acessível e legível (UE02); sem exigência de dados desnecessários para lições básicas (UE15); interface previsível (UE22).

**Out of Scope**

- Implementação do conteúdo completo de todos os módulos avançados.

# Acceptance Criteria

**Scenario Principal:**

- Given que existe ao menos uma lição publicada, When o usuário selecionar a lição na Tela 1, Then o conteúdo é exibido e permite avançar.

**Cenário alternativo: nenhuma lição publicada**

- **Dado** que nenhuma lição está disponível
- **Quando** a pessoa usuária abrir a área de aprendizagem
- **Então** o sistema deve informar que não há lições disponíveis, sem exibir uma tela vazia ou erro técnico
