# Sprint 2

Date: 19 de dezembro de 2024 → 30 de janeiro de 2025
Etapa: RSD
Status: Done

# Sprint 2 — Backlog v2, Protótipos e BDD

Transformar o backlog v2 em um plano funcional verificável, com prioridades, protótipos conceituais e cenários BDD.

## Backlog v2 consolidado

A versão v1 deve permanecer preservada. A v2 descrita no documento tem 11 histórias:

- **US01 — Acessar lições básicas:** prioridade original alta; mantida.
- **US02 — Responder quizzes:** prioridade original alta; mantida.
- **US03 — Conhecer história e cultura indígena:** prioridade original alta; mantida e ampliada para enfatizar contexto e fontes confiáveis.
- **US04 — Ouvir áudios das palavras em Tupi:** incluída; prioridade original alta.
- **US05 — Acompanhar progresso:** incluída; prioridade original alta.
- **US06 — Revisar palavras e lições anteriores:** incluída; prioridade original alta.
- **US07 — Baixar lições para estudar sem internet:** incluída; prioridade original média.
- **US08 — Receber pontos e cumprir metas:** prioridade original média; mantida e aprimorada.
- **US09 — Consultar dicionário Tupi-Português:** incluída; prioridade original alta.
- **US10 — Acessar conteúdos Premium por preço acessível:** prioridade original média; mantida e detalhada.
- **US11 — Visualizar frases cotidianas:** incluída; prioridade original alta.

Nenhuma história foi excluída, conforme o backlog v2 fornecido.

## Ordem sugerida para desenvolvimento

Esta ordem é uma proposta de planejamento e precisa ser validada pela equipe; não substitui as prioridades originais.

1. US01 — Lições básicas: núcleo do produto.
2. US02 — Quizzes: praticar e verificar compreensão.
3. US04 — Áudio: apoiar pronúncia com texto e validação adequada.
4. US03 — Contexto cultural: evitar conteúdo descontextualizado e indicar fontes.
5. US06 — Revisão: retomar conteúdos estudados.
6. US11 — Frases cotidianas: apresentar usos práticos com contexto.
7. US09 — Dicionário: consultar palavras, significados e variantes.
8. US05 — Progresso: acompanhar conclusão sem confundir com fluência.

US07 (offline), US08 (gamificação) e US10 (Premium) permanecem no backlog e devem ser planejadas conforme capacidade, dependências e retorno esperado.

## Critérios de priorização

- Valor direto para aprendizagem e experiência inicial.
- Relação com necessidades registradas na entrevista simulada.
- Dependências entre funcionalidades.
- Responsabilidade cultural, precisão linguística, acessibilidade e privacidade.
- Viabilidade de implementação e validação em etapas.

## Protótipos de baixa fidelidade

Os wireframes são conceituais; não representam telas implementadas nem validação real com usuários.

- **Tela 1 — Início e lições (US01):** continuar lição, lista de lições e navegação Início/Aprender/Perfil.
- **Tela 2 — Quiz (US02):** enunciado, alternativas, confirmação e feedback após responder.
- **Tela 3 — Palavra, áudio e cultura (US03/US04):** palavra em Tupi, reprodução de áudio, significado, contexto cultural e fonte.
- **Tela 4 — Revisão (US06):** lista de palavras e lições anteriores, mantendo histórico privado.
- **Tela 5 — Dicionário (US09):** busca, resultado, significado, contexto/variante e fonte quando disponível.
- **Tela 6 — Frases cotidianas (US11):** categorias, frase, tradução, contexto de uso e fonte/nota.
- **Tela 7 — Progresso (US05):** lições concluídas, palavras estudadas e explicação de que concluir lições não significa fluência.

## Cenários BDD detalhados (proposta para validação)

Os cenários abaixo transformam os comportamentos esperados em passos verificáveis. São especificações propostas, não evidência de implementação nem de testes executados. A equipe deve conferir os detalhes com os critérios de aceitação definitivos antes da entrega.

### US01 — Acessar lições básicas

**Cenário: abrir uma lição disponível**

- **Dado** que existe ao menos uma lição publicada
- **Quando** a pessoa usuária abrir a área de aprendizagem e selecionar uma lição
- **Então** o sistema deve exibir o conteúdo da lição selecionada e permitir avançar conforme a navegação prevista

**Cenário: não há lições publicadas**

- **Dado** que nenhuma lição está disponível
- **Quando** a pessoa usuária abrir a área de aprendizagem
- **Então** o sistema deve informar que não há lições disponíveis, sem exibir uma tela vazia ou erro técnico

### US02 — Responder quizzes

**Cenário: resposta correta**

- **Dado** que a pessoa usuária iniciou um quiz com uma pergunta e alternativas
- **Quando** selecionar a alternativa correta e confirmar a resposta
- **Então** o sistema deve informar que a resposta está correta e apresentar o feedback previsto

**Cenário: resposta incorreta**

- **Dado** que a pessoa usuária iniciou um quiz
- **Quando** selecionar uma alternativa incorreta e confirmar a resposta
- **Então** o sistema deve informar o resultado de forma respeitosa e apresentar explicação ou possibilidade de nova tentativa, conforme as regras do quiz

### US03 — Conhecer história e cultura

**Cenário: consultar conteúdo com fonte**

- **Dado** que existe um conteúdo histórico ou cultural publicado com fonte registrada
- **Quando** a pessoa usuária abrir esse conteúdo
- **Então** o sistema deve apresentar o texto e a referência da fonte disponível

**Cenário: informação incerta**

- **Dado** que um conteúdo possui uma incerteza ou divergência registrada
- **Quando** a pessoa usuária consultar esse conteúdo
- **Então** o sistema deve explicitar a limitação, sem apresentar a informação como certeza absoluta

### US04 — Ouvir áudios das palavras em Tupi

**Cenário: áudio disponível**

- **Dado** que uma palavra possui áudio associado
- **Quando** a pessoa usuária acionar a reprodução
- **Então** o áudio deve ser reproduzido e a forma escrita da palavra deve continuar visível

**Cenário: áudio indisponível**

- **Dado** que a palavra não possui áudio disponível
- **Quando** a pessoa usuária abrir a entrada
- **Então** o sistema deve informar que o áudio não está disponível, sem simular uma reprodução

### US05 — Acompanhar progresso

**Cenário: visualizar atividades concluídas**

- **Dado** que a pessoa usuária concluiu uma ou mais lições
- **Quando** abrir a área de progresso
- **Então** o sistema deve apresentar os registros de conclusão e explicar o significado dos indicadores

**Cenário: preservar privacidade**

- **Dado** que existe um histórico individual de aprendizagem
- **Quando** a pessoa usuária consultar o progresso
- **Então** os dados devem ser exibidos de forma privada por padrão, sem publicação automática para outras pessoas

### US06 — Revisar palavras e lições anteriores

**Cenário: reabrir conteúdo concluído**

- **Dado** que a pessoa usuária concluiu uma lição anteriormente
- **Quando** acessar a área de revisão e selecionar essa lição
- **Então** o sistema deve permitir consultar novamente o conteúdo

**Cenário: histórico privado**

- **Dado** que existem respostas ou dificuldades anteriores registradas
- **Quando** a pessoa usuária realizar uma revisão
- **Então** o sistema não deve publicar o histórico sem consentimento

### US07 — Baixar lições para estudar sem internet

**Cenário: download concluído**

- **Dado** que uma lição permite uso offline e há conexão disponível
- **Quando** a pessoa usuária solicitar o download e ele terminar com sucesso
- **Então** o sistema deve confirmar a conclusão e identificar a lição como disponível offline

**Cenário: download falhou**

- **Dado** que a pessoa usuária solicitou o download de uma lição
- **Quando** ocorrer uma falha no processo
- **Então** o sistema deve informar a falha e não marcar a lição como disponível offline

### US08 — Receber pontos e cumprir metas

**Cenário: atividade válida concluída**

- **Dado** que as regras de pontuação estão definidas e a pessoa usuária concluiu uma atividade elegível
- **Quando** o sistema registrar a conclusão
- **Então** deve atualizar a pontuação conforme as regras e explicar a recompensa concedida

**Cenário: meta ajustada**

- **Dado** que a pessoa usuária pode configurar uma meta de estudo
- **Quando** alterar a meta para um valor permitido
- **Então** o sistema deve salvar e apresentar a nova meta sem mensagens punitivas por metas não cumpridas

### US09 — Consultar dicionário Tupi-Português

**Cenário: termo encontrado**

- **Dado** que o dicionário contém uma entrada correspondente ao termo pesquisado
- **Quando** a pessoa usuária realizar a busca
- **Então** o sistema deve apresentar o significado e o contexto, variante ou fonte quando essas informações estiverem disponíveis

**Cenário: nenhum resultado**

- **Dado** que não existe entrada correspondente à busca
- **Quando** a pessoa usuária pesquisar o termo
- **Então** o sistema deve informar que não encontrou resultados e permitir uma nova consulta

### US10 — Acessar conteúdos Premium

**Cenário: consultar condições antes de contratar**

- **Dado** que a pessoa usuária abriu a área Premium
- **Quando** visualizar a oferta
- **Então** o sistema deve apresentar preço, benefícios, condições e limites antes de qualquer confirmação de contratação

**Cenário: acessar recursos gratuitos**

- **Dado** que a pessoa usuária não possui assinatura Premium
- **Quando** acessar os recursos gratuitos previstos
- **Então** o sistema deve permitir o uso desses recursos e identificar claramente quais itens exigem assinatura

### US11 — Visualizar frases cotidianas

**Cenário: consultar frase por categoria**

- **Dado** que existem frases cadastradas em uma categoria
- **Quando** a pessoa usuária selecionar essa categoria
- **Então** o sistema deve apresentar as frases com tradução e contexto de uso quando disponíveis

**Cenário: frase sem validação adequada**

- **Dado** que uma expressão ainda não foi validada por fonte adequada
- **Quando** o conteúdo for preparado para publicação
- **Então** a expressão não deve ser apresentada como autêntica ou definitiva até que a validação necessária seja realizada

## Relação entre requisitos funcionais e éticos

- US01 — UE02, UE15, UE22.
- US02 — UE04, UE20.
- US03 — UE03, UE12, UE25, UE21.
- US04 — UE06, UE17.
- US05 — UE01, UE14, UE24.
- US06 — UE10.
- US07 — UE07, UE19.
- US08 — UE08, UE18, UE23.
- US09 — UE09, UE21.
- US10 — UE05, UE16.
- US11 — UE11, UE12, UE25.

## Checklist antes da entrega

- [ ]  Preservar o backlog v1 e identificar a v2 separadamente.
- [ ]  Manter as prioridades originais e marcar a ordem de execução como proposta.
- [ ]  Validar nomes dos integrantes e divisão de responsabilidades.
- [ ]  Revisar os protótipos e redesenhá-los em ferramenta visual se solicitado.
- [ ]  Conferir cenários BDD sem apresentá-los como testes já executados.
- [ ]  Preencher atas somente com reuniões e decisões reais.
- [ ]  Verificar fontes linguísticas e culturais antes de publicar conteúdo no aplicativo.

> Nota de escopo: este material é uma proposta de planejamento e documentação. A equipe deve validar o conteúdo com as orientações da disciplina antes da entrega.
> 

## Tabela de correspondência — Backlog v1 × Backlog v2

**Como ler:** “Correspondência parcial” significa que a v2 cobre apenas parte do objetivo da história antiga. “Não identificada” significa que a funcionalidade não aparece como história própria na v2; não significa que foi cancelada ou implementada. A equipe deve confirmar estas relações.

| História v1 | Tema da v1 | História v2 relacionada | Tipo de relação | Observação / ação recomendada |
| --- | --- | --- | --- | --- |
| US01 | Cadastro de usuário | — | Não identificada | Cadastro não aparece como história própria na v2. Decidir se precisa voltar ao backlog e como se relaciona com privacidade e conta. |
| US02 | Acesso à conta | — | Não identificada | Login não aparece como história própria na v2. Confirmar se a v2 pressupõe acesso sem conta ou se faltou documentar autenticação. |
| US03 | Módulos de vocabulário | US01 — Acessar lições básicas; US09 — Dicionário Tupi-Português | Parcial / dividida | Lições cobrem aprendizagem organizada; dicionário cobre consulta de palavras. Conferir se todo o vocabulário previsto está contemplado. |
| US04 | Módulos de gramática | US01 — Acessar lições básicas | Parcial | A v2 fala em lições básicas, mas não explicita gramática. Confirmar e acrescentar critérios de gramática se continuar no escopo. |
| US05 | Conteúdos históricos e culturais | US03 — Conhecer história e cultura indígena | Direta / ampliada | A v2 reforça contexto, fontes confiáveis e explicitação de incertezas. |
| US06 | Quizzes | US02 — Responder quizzes | Direta | Mesma finalidade geral; conferir os critérios de aceitação finais. |
| US07 | Pontuação | US08 — Receber pontos e cumprir metas | Direta / ampliada | A v2 reúne pontuação e metas de estudo. |
| US08 | Progresso de aprendizagem | US05 — Acompanhar progresso | Direta | A v2 descreve indicadores de conclusão e privacidade por padrão. |
| US09 | Recompensas | US08 — Receber pontos e cumprir metas | Parcial | Pontos e metas não equivalem necessariamente a todas as recompensas. Decidir se recompensas específicas ainda são necessárias. |
| US10 | Ranking | — | Não identificada | Ranking não aparece na v2. Confirmar se foi retirado intencionalmente; considerar implicações de privacidade e bem-estar antes de reintroduzir. |
| US11 | Certificado digital | — | Não identificada | Certificados não aparecem na v2. Confirmar se estão fora do escopo ou precisam ser planejados. |
| US12 | Comunidade online | — | Não identificada | Comunidade não aparece na v2. Confirmar decisão de escopo e necessidades de moderação/segurança caso retorne. |
| US13 | Chatbot de suporte | — | Não identificada | Chatbot não aparece na v2. Confirmar se foi adiado ou removido do escopo. |
| US14 | Acessibilidade | Todas as histórias v2 (requisito transversal) | Transversal, não explícita como história | Garantir critérios verificáveis de acessibilidade nos protótipos e critérios de aceitação; a relação não substitui uma história própria, se exigida. |
| US15 | Segurança dos dados | US05 — Progresso; US06 — Revisão; US10 — Premium (e requisito transversal) | Parcial / transversal | A v2 menciona privacidade em alguns cenários, mas não substitui requisitos completos de segurança e LGPD. Manter critérios explícitos. |
| US16 | Desempenho do aplicativo | — | Não identificada | Meta de 10.000 usuários simultâneos e resposta inferior a 2 segundos não aparece como história própria na v2. Preservar como requisito não funcional e validar viabilidade. |
| US17 | Android e iOS | — | Não identificada | Plataformas não são explicitadas na v2. Registrar como restrição/requisito de plataforma se continuar no escopo. |
| US18 | Acompanhamento dos usuários por educador | US05 — Acompanhar progresso | Parcial | A v2 foca o progresso individual do estudante; acompanhamento por educador e permissões não estão descritos. Confirmar se esse perfil continua necessário. |
| — | Áudio de palavras em Tupi | US04 — Ouvir áudios das palavras em Tupi | Nova na v2 | Não há história equivalente explícita na v1. Validar fontes, pronúncia e disponibilidade dos áudios. |
| — | Revisar palavras e lições anteriores | US06 — Revisar palavras e lições anteriores | Nova na v2 | Funcionalidade nova explícita. |
| — | Baixar lições para estudar sem internet | US07 — Baixar lições para estudar sem internet | Nova na v2 | Funcionalidade nova explícita; definir limites e comportamento offline. |
| — | Dicionário Tupi-Português | US09 — Consultar dicionário Tupi-Português | Nova como história própria na v2 | Pode aproveitar parte do objetivo de vocabulário da v1 US03, mas o dicionário não estava explícito como história própria. |
| — | Conteúdos Premium | US10 — Acessar conteúdos Premium por preço acessível | Nova na v2 | Definir claramente preço, benefícios, condições e recursos gratuitos. |
| — | Frases cotidianas | US11 — Visualizar frases cotidianas | Nova na v2 | Validar expressões e contexto de uso com fontes adequadas. |

### Decisões pendentes da equipe

- [ ]  Confirmar se cadastro e login (v1 US01–US02) continuam necessários.
- [ ]  Confirmar o destino de ranking, certificado, comunidade e chatbot (v1 US10–US13).
- [ ]  Garantir que acessibilidade, segurança, desempenho e plataformas (v1 US14–US17) permaneçam registrados, mesmo que sejam requisitos transversais.
- [ ]  Confirmar se o acompanhamento por educadores (v1 US18) continua no escopo.
- [ ]  Validar se gramática e recompensas estão suficientemente cobertas pela v2.
- [ ]  Registrar a decisão de cada item como **mantido**, **reformulado**, **adiado** ou **retirado**, com justificativa e aprovação da equipe.

**Importante:** esta é uma correspondência inicial baseada no conteúdo dos dois documentos, não uma aprovação oficial nem prova de implementação. A v1 deve permanecer preservada como histórico até a equipe validar as decisões.

## Critérios de aceitação verificáveis — complemento proposto

Os critérios abaixo tornam os comportamentos das US01–US11 mais fáceis de verificar. São **propostas documentais** para revisão, não aprovação formal nem evidência de implementação. Como o prazo é curto, podem ser revisados de forma assíncrona.

| História | Critérios de aceitação mínimos propostos |
| --- | --- |
| US01 — Lições básicas | A lista apresenta apenas lições disponíveis; ao selecionar uma lição, o conteúdo correspondente é exibido; quando não houver lições, aparece uma mensagem explicativa; a navegação não perde o conteúdo selecionado sem aviso. |
| US02 — Quizzes | Cada pergunta apresenta alternativas; a pessoa consegue selecionar e enviar uma resposta; o sistema diferencia resposta correta e incorreta; o feedback é compreensível e respeitoso; o resultado final é apresentado ao encerrar o quiz. |
| US03 — História e cultura | O conteúdo publicado apresenta fonte e contexto quando disponíveis; divergências ou incertezas conhecidas são indicadas; conteúdos sem fonte adequada não são apresentados como fato definitivo. |
| US04 — Áudio | Quando houver áudio associado, o controle inicia a reprodução; a palavra escrita permanece visível; quando o áudio não estiver disponível ou falhar, o sistema informa isso e não simula sucesso; existe alternativa textual para a informação relevante. |
| US05 — Progresso | A área de progresso exibe atividades concluídas registradas; após concluir uma atividade, o indicador é atualizado; a interface explica o significado dos indicadores; os dados ficam privados por padrão. |
| US06 — Revisão | A pessoa consegue localizar e reabrir conteúdo concluído; o conteúdo selecionado é exibido corretamente; o histórico individual não é publicado automaticamente. |
| US07 — Offline | Uma lição só é marcada como disponível offline após o download terminar com sucesso; uma falha é informada; conteúdo ainda não baixado não é apresentado como disponível sem conexão. |
| US08 — Pontos e metas | Uma atividade elegível atualiza pontos conforme regras definidas; a pessoa consegue consultar o total e a meta; metas inválidas são rejeitadas com explicação; metas não cumpridas não geram mensagens punitivas. |
| US09 — Dicionário | Uma busca com resultado apresenta termo e significado; contexto, variante e fonte são exibidos quando conhecidos; busca sem resultado mostra mensagem clara e permite nova tentativa. |
| US10 — Premium | Antes de contratar, a pessoa visualiza preço, benefícios, cobrança, limites e condições; recursos gratuitos são identificados; não ocorre contratação sem confirmação explícita. |
| US11 — Frases cotidianas | A categoria selecionada apresenta frases relacionadas; tradução e contexto são mostrados quando disponíveis; expressão sem validação adequada não é apresentada como forma autêntica ou definitiva. |

### Regras de teste e rastreabilidade

- Cada critério deve ser ligado a pelo menos um cenário BDD relevante.
- Para considerar um teste executado, registrar ambiente/versão, entrada, resultado esperado, resultado observado e status (passou/falhou/bloqueado).
- Cenário escrito não é teste executado. Sem implementação ou registro de execução, o status deve permanecer “não executado”.
- Se um critério depender de conteúdo linguístico, áudio ou referência cultural, registrar a fonte e a validação necessária antes da publicação.

## Registro de requisitos não funcionais e lacunas da v1

A v1 contém requisitos transversais que não aparecem como histórias próprias na v2. Para evitar perda de escopo, mantê-los no registro abaixo até uma decisão explícita.

| Tema | Registro conhecido | Tratamento documental recomendado | Estado |
| --- | --- | --- | --- |
| Acessibilidade | v1 US14: boas práticas, elementos identificáveis e navegação móvel adequada | Aplicar verificações de acessibilidade às telas e registrar critérios verificáveis; incluir alternativa textual para áudio | Pendente de detalhamento/verificação |
| Segurança e LGPD | v1 US15: proteção de dados, boas práticas LGPD e não exposição indevida | Definir dados coletados, finalidade, acesso, retenção e consentimento antes de implementação | Pendente de detalhamento/verificação |
| Desempenho | v1 US16 registra meta de até 10.000 usuários simultâneos e resposta inferior a 2 segundos nas condições previstas | Preservar como meta herdada; definir cenário de carga, operação medida e método de teste antes de afirmar conformidade | Meta registrada; não testada |
| Plataformas | v1 US17 prevê Android e iOS | Confirmar se ambas as plataformas continuam no escopo da v2 e listar funcionalidades essenciais por plataforma | Decisão de escopo pendente |
| Educadores | v1 US18 prevê acompanhamento conforme permissões | Se mantido, definir papéis, permissões e limites de acesso ao progresso individual | Decisão de escopo pendente |

## Decisões de escopo que podem ser registradas sem reunião

Para cada item abaixo, a documentação ainda não fornece uma decisão definitiva. Não presumir que foi removido. Se o prazo não permitir decisão, manter como “fora da v2 / decisão pendente” na apresentação:

- Cadastro e login (v1 US01–US02).
- Ranking e certificado (v1 US10–US11).
- Comunidade e chatbot (v1 US12–US13).
- Acompanhamento por educador (v1 US18).
- Cobertura explícita de gramática e recompensas da v1.

**Recomendação para entrega curta:** mostrar a v2 como escopo funcional de referência para esta documentação, preservar a v1 como histórico e apresentar as lacunas como decisões pendentes — nunca como funcionalidades entregues, testadas ou oficialmente canceladas.