# US04 - Ouvir áudios das palavras em Tupi

Categoria: RSD / Backlog v2
Prioridade: Alta
Rastreabilidade Ética: UE06, UE17

<aside>
💡

*"Como estudante, quero reproduzir o áudio associado às palavras em Tupi, para ter apoio auditivo durante o estudo da pronúncia."*

</aside>

# Goals

- Fornecer referência auditiva de pronúncia sempre acompanhada da grafia escrita.

### Context

- Estudantes autodidatas têm dificuldade em saber a pronúncia correta apenas lendo a palavra.

# Story

When o estudante aciona o controle de áudio de uma palavra, Then o sistema reproduz o som mantendo a forma escrita visível.

# Requirements

**Functional requirements**

- Botão de reprodução de áudio; manter palavra escrita visível; informar claramente quando o áudio estiver indisponível.

**Non-Functional requirements**

- Não rotular áudios provisórios como definitivos (UE06); alternativa textual obrigatória para acessibilidade (UE17).

**Out of Scope**

- Síntese de voz artificial não validada.

# Acceptance Criteria

**Scenario Principal:**

- Given palavra com áudio associado, When acionar reprodução, Then o áudio toca e a grafia permanece visível.
