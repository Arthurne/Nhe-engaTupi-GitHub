# Sprint 3

Date: 30 de janeiro de 2025 → 4 de fevereiro de 2025
Etapa: RSD
Status: In progress

# Sprint 3 — Planejamento e Detalhamento Funcional

- **Etapa:** RSD — Requisitos e Design de Software
- **Status:** Planejamento documental (proposta de continuidade)
- **Período registrado:** 30/01/2025 a 04/02/2025 *(confirmar manutenção antes da entrega)*

## 1. Objetivo e Contexto

Dar continuidade à Sprint 2, detalhando os fluxos de **revisão (`US06`)**, **frases cotidianas (`US11`)**, **dicionário Tupi–Português (`US09`)** e **acompanhamento de progresso (`US05`)**, definindo critérios verificáveis, mensagens de estado vazio e alinhamento entre protótipos conceituais, BDD e Matriz de Rastreabilidade (`UE01–UE25`).

- **Fora do escopo desta Sprint:** implementação de código, download offline (`US07`), pontos e metas (`US08`) e oferta Premium (`US10`).

## 2. Histórias Selecionadas e Critérios de Verificação

| História | Objetivo na Sprint 3 | Critério de Verificação |
| :--- | :--- | :--- |
| **US06 — Revisar palavras e lições** | Permitir retomar conteúdos estudados sem perder referência. | Identificar e reabrir lição/palavra estudada; exibir mensagem clara se o histórico estiver vazio; histórico privado por padrão. |
| **US11 — Visualizar frases cotidianas** | Organizar frases por categoria com tradução e contexto. | Exibir tradução e contexto quando disponíveis; não publicar expressões sem fonte validada como definitivas. |
| **US09 — Consultar dicionário Tupi–Português** | Facilitar busca por palavras com significado, variante e fonte. | Exibir significado/contexto/variante/fonte quando encontrado; informar ausência de resultado e permitir nova busca. |
| **US05 — Acompanhar progresso** | Mostrar registros de aprendizagem de forma simples e privada. | Exibir indicadores compreensíveis, privados por padrão, explicitando que conclusão de lições não equivale a fluência. |

## 3. Atividades, Entregáveis e Definition of Done (DoD)

- **Atividades:** revisar fluxos nos protótipos conceituais; conferir cenários BDD de `US05, US06, US09, US11`; definir mensagens para estados vazios; checar fontes/variantes; atualizar Matriz de Rastreabilidade.
- **Cuidados e Riscos:** evitar traduções apresentadas como universais sem fonte; definir retenção/privacidade do histórico; evitar indicadores visuais que sugiram falsa fluência; não declarar testes ou implementação sem evidência.
- **Definition of Done (DoD):**
  - [ ] Critérios de aceitação revisados para as 4 histórias.
  - [ ] Protótipos conceituais cobrindo fluxos principais e estados vazios/sem resultado.
  - [ ] Cenários BDD alinhados aos critérios (mantidos como "não executados").
  - [ ] Fontes e incertezas registradas; Matriz de Rastreabilidade atualizada.
