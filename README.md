# Proposta de melhoria do processo AGES

Este README reúne o entendimento do grupo, a referência do processo atual e as decisões em discussão para o Trabalho Final de Melhoria de Processos. A proposta deve ser lida em níveis diferentes: primeiro, um processo geral que dá autonomia para cada AGES IV configurar o modo de trabalho de sua equipe; depois, uma instância concreta sugerida pelo grupo; por fim, a especificação detalhada de uma atividade.

## Separação lógica dos modelos e resultados

O trabalho terá três BPMNs relacionados, mas com propósitos distintos. O BPMN atual continua como referência de comparação.

1. **O Fluxo AGES Atual — referência _as is_.** `O_Fluxo_AGES_Atual.bpmn` reconstrói o fluxo dos materiais da AGES e do Anexo 1. Serve para entender o ponto de partida, não para prescrever a melhoria.
2. **Fluxo AGES — BPMN abstrato adicional.** `O_Fluxo_AGES_Proposto_Abstrato.bpmn` apresenta o processo geral, sem impor metodologia ou conjunto fixo de cerimônias. Mostra como a equipe se organiza e executa o trabalho e, sobretudo, como o AGES IV define/adapta o processo, cerimônias, políticas, artefatos e acordos de trabalho para aquela equipe. Esse processo é uma _sandbox_: dá autonomia ao AGES IV dentro das responsabilidades e guardrails acordados. O AGES III viabiliza tecnicamente o trabalho como Tech Lead/_Enabling Team_. A definição e aplicação desse processo próprio são parte do que se espera avaliar na banca.
3. **O Fluxo AGES Proposto Sugerido — Resultado 1 do enunciado.** `O_Fluxo_AGES_Proposto_Sugerido.bpmn` é um primeiro rascunho de uma instância concreta: a sugestão do grupo para um fluxo de desenvolvimento que inclui IA. É um modelo idealizado para discutir e testar, inspirado pela referência ao modelo Gartner trazida pelo grupo, pelo Double Diamond, Inception e outras práticas. Será refinado a partir destas notas e não deve ser interpretado como a única metodologia obrigatória para todas as equipes AGES.
4. **Resultado 2 — especificação de uma atividade.** Depois de escolher a etapa/atividade, detalhar seu propósito, os papéis envolvidos, o propósito dos artefatos e a estrutura/conteúdo de cada artefato. Esse detalhamento explica uma parte da instância do Resultado 1, sem substituir o BPMN abstrato nem a autonomia do AGES IV.

O objetivo dessa separação é distinguir **quem define o método de trabalho** (AGES IV no processo geral), **uma configuração possível desse método** (a instância proposta pelo grupo para o Resultado 1) e **como executar uma atividade específica** (Resultado 2). A equipe pode adaptar a instância às necessidades do projeto, mantendo explícitos os acordos e decisões.

O BPMN abstrato é adicional e complementar: ele explica a autonomia de AGES IV para desenhar o processo da própria equipe. O BPMN sugerido preserva a proposta concreta que o grupo vem construindo — Inception/Sprint 0, squads, pareamento, IA, PoCs e ciclos de feedback — como uma possível instância dessa autonomia.

## Referência: etapas do fluxo atual

Esta síntese cruza `O_Fluxo_AGES_Atual.bpmn`, `ProcessosAGES-ProcessoAGES-v6.png` e o Anexo 1 de `MPS2026_2_TF_Enunciado.pdf`. Os nomes das etapas são os do Anexo 1. **Pré-AGES** é apenas um apelido usado nas notas para o período de identificação, seleção e definição do projeto.

1. **Etapa 1: Semestre que antecede a execução do projeto na AGES.** O processo visual de identificação, seleção e definição mostra `Apresentação da Ideia pelos stakeholder`, `Validação da Ideia`, `Definição do semestre que o projeto irá ser executado`, `Reuniões mensais com os Stakeholders`, `Validação dos Requisitos` e `Elaboração do Termo de Abertura de Projetos`. Reuniões, validação de requisitos e elaboração do termo compõem um ciclo de alinhamento antes da execução.
2. **Etapa 2: Organização e kick-off do projeto.** Na `Semana Inicial`, aparecem `Apresentação Inicial AGES e do Fluxo AGES.` e `Apresentação do Processo da AGES, responsabilidades e artefatos, apresentação dos relatórios (sprint, andamento e final)`. No `Warm Up (Sprint 0)`, o material mostra `Apresentação dos projetos pelos stakeholders`; em paralelo, `Documentação dos Requisitos e Mockups (Time)`, `Definição Arquitetura ou revisão (AGES III)` e `EAP / Cronograma / Plano de Comunicação / U.S. (AGES IV)`; depois, `Apresentação para stakeholders`. Também registra `Estudos das tecnologias utilizadas nos projetos (linguagens e metodologias TDD, BDD, Code review, pair programming, etc..)`. O BPMN atual representa os três trabalhos intermediários em paralelo.
3. **Etapa 3: Sprints iniciais e Revisão intermediária.** O material agrupa `Sprints 1 e 2`, mostra o marco `Após a sprint 1` e depois agrupa `Sprints 3 e 4`. Cada `Sprint Duas Semanas` contém `Planning`; `Aula Meeting` e `Desenvolvimento Documentação` em paralelo; `Entrega para os Stakeholders`; `Retrospectiva`; e `Entrega do relatório da Sprint`. Após a Sprint 1 também aparecem `Entrega Relatório de Andamento` e `ONE on ONE (com os alunos)`. No BPMN atual, o ONE on ONE está na lane `Professor Orientador`; as anotações do grupo especificam que ocorre individualmente com cada aluno.
4. **Etapa 4: Encerramento.** Na `Semana Final`, o material registra `Retrospectiva geral da AGES + Confraternização`, `Entrega Relatório Final`, `Apresentação dos projetos da AGES (estudantes + stakeholders + professores)` e `ONE on ONE (com os alunos)`. O material e o BPMN atual posicionam `Apresentação das BANCAS` após os Sprints 3 e 4 e antes da Semana Final. **Correção informada pelo grupo:** na prática, as bancas de AGES IV acontecem depois das atividades da Semana Final; essa diferença deve ficar identificada até que a representação _as is_ seja atualizada.

### Requisitos não funcionais no Pré-AGES

- Durante a Etapa 1, Coordenação e Stakeholders devem elicitar, esclarecer e validar os requisitos não funcionais relevantes ao projeto, aproveitando as `Reuniões mensais com os Stakeholders` e a `Validação dos Requisitos` do processo atual.
- Registrar critérios verificáveis e exemplos de aceitação conforme o contexto: por exemplo, segurança e privacidade, desempenho, disponibilidade, usabilidade, acessibilidade, manutenibilidade e restrições de plataforma. Os critérios são acordados com Stakeholders, não presumidos iguais em todos os projetos.
- Esses acordos entram nos requisitos e no Termo de Abertura antes do início do trabalho da equipe. Depois orientam arquitetura, configuração das ferramentas e agente de IA, planejamento da PoC e sua validação, mesmo quando o protótipo usa dados mockados ou não tem backend.

## Fluxo AGES

Este é o nível geral que deve expressar a melhoria de governança proposta. O diagrama não deve fixar que toda equipe use Sprint 0, Scrum, Design Sprint, a mesma cadência ou os mesmos artefatos. Deve explicitar que AGES IV configura e mantém o processo de trabalho para sua equipe dentro dos objetivos, restrições e responsabilidades combinados.

- **AGES IV — gestão e desenho do processo:** entende o contexto e os objetivos do projeto; define ou adapta metodologia, etapas, cerimônias, papéis, artefatos, cadência, critérios de priorização e mecanismos de acompanhamento. Comunica os acordos à equipe, conduz o fluxo gerencial e revê o processo com base nos resultados e feedbacks. AGES IV também especificam épicos e features/histórias, priorizam o trabalho e definem guardrails, processos e políticas de uso da IA.
- **AGES III — liderança técnica e _Enabling Team_:** atua como Tech Lead das squads e viabiliza tecnicamente o modo de trabalho definido pela gestão. Em engenharia de plataforma, habilita recursos compartilhados de desenvolvimento e IA, apoia arquitetura, dependências e qualidade técnica e ajuda as squads a executar o processo sem assumir a responsabilidade gerencial de AGES IV.
- **AGES I e II — desenvolvimento:** executam o trabalho técnico e usam as capacidades de IA/plataforma conforme as políticas acordadas. Na proposta do grupo, o trabalho assistido por IA é feito em pares, com revisão crítica e compartilhamento de conhecimento.
- **Autonomia com prestação de contas:** o processo geral deve permitir escolhas adequadas ao contexto, mas AGES IV explicita as razões, acordos e resultados da metodologia adotada. A banca avalia a definição e a condução do processo da equipe, não a obediência a uma única receita predefinida.

O primeiro desenho deste ciclo está em `O_Fluxo_AGES_Proposto_Abstrato.bpmn`: AGES IV recebe objetivos e restrições → define/ajusta o processo da equipe com apoio técnico de AGES III → equipe executa o trabalho conforme os acordos → equipe demonstra resultados e coleta feedback → AGES IV e equipe avaliam resultados e ajustam o processo. O BPMN permanece abstrato; detalhes de atividades, gateways e artefatos podem ser refinados após a revisão destas notas.

## Instância sugerida para o Resultado 1

Esta seção descreve a configuração concreta que o grupo propõe para ilustrar o processo geral. O BPMN `O_Fluxo_AGES_Proposto_Sugerido.bpmn` representa este fluxo, não o processo abstrato de autonomia do AGES IV.

### Referências de desenho

- Adaptar a referência ao “modelo Gartner” trazida pelo grupo: o Double Diamond de Descobrir/Definir fica concentrado na relação Coordenação–Stakeholders; a equipe AGES I–IV trabalha no segundo diamante, Desenvolver/Entregar, depois do alinhamento inicial.
- Tratar Inception como alinhamento estruturado sobre problema, usuários, proposta de solução e MVP, e não como simples warm-up. A Lean Inception é descrita por seu autor como workshop colaborativo de alinhamento e definição do MVP; práticas podem ser selecionadas/adaptadas à Sprint 0 ([referência](https://caroli.org/lean-inception-3/)).
- A Sprint 0 junta Inception e Spike/PoC: a equipe constrói uma experiência funcional do fluxo core, que pode não ter backend ou usar dados mockados, para obter aprendizado e feedback antes das sprints regulares.

### Ordem dos encontros e atividades da Sprint 0

- **Ordem atual anotada pelo grupo:** apresentação da AGES → apresentação do projeto/equipe → reunião de elicitação com Stakeholders.
- **Ordem sugerida:** apresentação da AGES → elicitação com Stakeholders → apresentação do projeto/equipe. A mudança antecipa a escuta do cliente.
- **Elicitação colaborativa:** todos os níveis AGES e Stakeholders participam do levantamento de requisitos, com dinâmica de brainstorming.
- **User Story Mapping em dois momentos:** primeiro, brainstorming e construção do mapa com cliente/Stakeholders; depois, a equipe se reúne sem o cliente para consolidar e analisar o mapa, priorizar histórias e definir o MVP como um fluxo core ponta a ponta, transversal aos componentes da aplicação. Retomar decisões importantes com Stakeholders para confirmar o entendimento.
- **Formação de squads:** após o trabalho coletivo, dividir a equipe em squads com níveis AGES mistos. Os níveis são “tribos” de conhecimento; as squads desenvolvem uma PoC cada. Cada AGES IV é gestor de uma squad, e um deles também exerce a coordenação do projeto de forma transversal às squads.
- **Wireframing e wireflowing:** cada squad cria wireframes dos fluxos core e representa ligações e transições entre telas.
- **Preparação do ambiente de prototipação:** AGES IV define a direção visual e coordena a construção da PoC; AGES III prepara design system, variables, styles, componentes e Figma com base na identidade visual, além de configurar tecnicamente o agente de IA conforme os guardrails definidos pela gestão.
- **Uma PoC por squad:** cada squad transforma o fluxo core em protótipo funcional e experimentável. AGES I e II usam IA na ideação, prototipação e desenvolvimento. O backend é opcional; dados podem ser mockados. O objetivo é testar o conceito e revelar riscos, não concluir o produto.
- **Pair programming e pareamento entre níveis:** todo trabalho assistido por IA é feito em pares. Formar e rotacionar pares com níveis complementares conforme a task e o conhecimento a disseminar; exemplos: AGES IV–AGES I, AGES II–AGES III, AGES III–AGES I e AGES IV–AGES II. Alternar driver/navigator e explicitar o raciocínio para promover revisão crítica, aprendizagem e disseminação de conhecimento.
- **WIP 0,5:** cada task apoiada por IA é uma unidade de trabalho compartilhada por um par; a diretriz considera 0,5 unidade de WIP por integrante e uma task ativa por dupla.
- **Governança e plataforma de IA:** AGES IV define guardrails, processos e políticas; AGES III atua como _Enabling Team_ de engenharia de plataforma e viabiliza tecnicamente as diretrizes, incluindo ambiente, agente e recursos de desenvolvimento. Pair programming não substitui o code review (de ownership do AGES III, conduzido de forma síncrona em colaboração com os desenvolvedores da task) nem a aprovação de AGES III/IV previstos para as tasks.
- **Demos:** cada squad apresenta sua PoC, seguida de critique estruturada, tratamento das divergências e alinhamento com Stakeholders sobre a direção escolhida.
- **Validação com usuários:** ao final da Sprint 0, observar usuários representativos usando as PoCs, registrar evidências e feedback e decidir se o MVP/core avança ou retorna para ajuste.

### Método de critique e alinhamento com Stakeholders

- Conduzir uma sessão de _design critique_ facilitada pelo AGES IV coordenador do projeto. A dinâmica **I Like, I Wish, What If** (o que funciona, o que poderia melhorar, que possibilidades explorar) é um formato possível, com comentários dirigidos ao artefato e não às pessoas. A Stanford d.school oferece orientação para estruturar feedback construtivo ([guia de feedback](https://dschool.stanford.edu/tools/how-to-give-feedback); [I Like, I Wish, What If](https://dschool.sfo3.digitaloceanspaces.com/documents/dschool_bootleg_deck_2018_final_sm2-6.pdf)).
- Agrupar comentários, relacioná-los aos objetivos do MVP e requisitos acordados, e explicitar divergências de valor, uso e viabilidade técnica. AGES III esclarece implicações técnicas; AGES IV facilita; Stakeholders decidem prioridades do produto. Votação pode indicar preferências, mas não substitui a decisão do cliente.
- Fechar com direção acordada, justificativa, responsável pela decisão, itens a validar e dissensos ainda abertos. Consenso significa entendimento compartilhado da decisão, não esconder divergências nem exigir que todos tenham a mesma preferência. Uma prática de _design studio_ recomenda registrar áreas de acordo e desacordo ao trabalhar com Stakeholders ([guia do Digital.gov](https://digital.gov/guides/research-collaboration/aligning/engagement)).

### Sprints regulares após a Sprint 0

- Como instância sugerida, manter sprints de duas semanas. AGES IV gerencia épicos/features e prioridades; AGES III, junto com a squad, auxilia na decomposição das USs em tasks e orienta arquitetura e dependências; AGES I/II executam tasks em pares.
- Todos os níveis participam do planning, da especificação e da priorização. AGES IV é responsável pelos épicos e features/histórias (cada épico pode conter uma ou mais USs); AGES III atua como Tech Lead, conduz a decomposição técnica com a squad e orienta AGES I/II na execução das tasks. A equipe demonstra entregas para Stakeholders e grupos envolvidos.
- **Blocos curtos internos (“mini-sprints”):** na planning, AGES IV, AGES III e equipe combinam colaborativamente a duração, o objetivo/entregável e o momento de revisão de cada bloco. Ao final, demonstrar ou revisar o incremento, colher feedback e decidir se ajusta a solução ou inicia outro bloco prioritário dentro do tempo restante da mesma sprint. A intenção é acelerar feedback e permitir mudanças em tempo de sprint, sem esperar o ciclo seguinte. Os blocos são timeboxes internos, não uma metodologia obrigatória para todas as equipes.
- Cada task passa por code review de ownership do AGES III, conduzido de forma síncrona em colaboração com quem desenvolveu a tarefa (que demonstra o funcionamento da implementação), seguido da aprovação de AGES III/IV. Essa troca síncrona aproxima liderança técnica e desenvolvedores, promove transferência de conhecimento e assegura que a validação e os critérios de aceitação sejam efetivamente respeitados. Se houver ajuste, retorna à execução e revisão. A IA não substitui revisão humana, validação, critérios não funcionais ou aprovação.
- Cada sprint gera seu relatório. O fluxo também preserva a revisão intermediária e os ONE on ONE individuais com professor/alunos após a Sprint 1 e na semana final, além das demonstrações e entregas aos Stakeholders. Conversas 1:1 com AGES IV podem ocorrer ao longo do projeto.
- O feedback de Stakeholders e usuários orienta a priorização/refinamento do backlog. Na instância sugerida, a apresentação das BANCAS de AGES IV fica após as atividades da Semana Final, conforme esclarecimento do grupo.

### Fundamentação anotada para pair programming

- PLONKA, Laura; SHARP, Helen; VAN DER LINDEN, Janet; DITTRICH, Yvonne. “Knowledge transfer in pair programming: an in-depth analysis.” _International Journal of Human-Computer Studies_, v. 73, p. 66–78, 2015. [DOI: 10.1016/j.ijhcs.2014.09.001](https://doi.org/10.1016/j.ijhcs.2014.09.001).
- ZIERIS, Franz; PRECHELT, Lutz. “Observations on knowledge transfer of professional software developers during pair programming.” In: _Proceedings of the 38th International Conference on Software Engineering Companion_, 2016, p. 242–250. [DOI: 10.1145/2889160.2889249](https://doi.org/10.1145/2889160.2889249).
- LUI, Kim Man; CHAN, Keith C. C. “Pair programming productivity: novice–novice vs. expert–expert.” _International Journal of Human-Computer Studies_, v. 64, n. 9, p. 915–925, 2006. [DOI: 10.1016/j.ijhcs.2006.04.010](https://doi.org/10.1016/j.ijhcs.2006.04.010).
- Os estudos embasam a hipótese de usar pareamento para transferência de conhecimento e revisão crítica, mas não garantem que uma combinação específica de níveis seja sempre mais produtiva. A prática proposta deve ser avaliada pela aprendizagem, qualidade e fluxo observados na AGES.

## Resultado 2: especificação de uma atividade

### Atividade selecionada

**Construir, demonstrar e validar a PoC de uma squad na Sprint 0.** Esta atividade detalha um recorte da Inception representada em alto nível no Fluxo AGES Proposto Sugerido. O BPMN mantém as fases principais, enquanto esta especificação explicita as subtarefas, responsabilidades e artefatos.

### Propósito

Construir uma PoC por squad para tornar experimentável o fluxo core ponta a ponta definido no User Story Mapping. A PoC deve apoiar a validação de hipóteses e requisitos, incluindo critérios não funcionais pertinentes, e gerar feedback de Stakeholders e usuários antes das sprints regulares. Pode usar dados mockados e não requer backend completo.

### Papéis envolvidos

| Papel                              | Responsabilidades na atividade                                                                                                                                                                                       |
| ---------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AGES IV gestor da squad            | Prioriza épicos e histórias, coordena a PoC da squad, define o objetivo e os critérios de validação, garante alinhamento com Stakeholders e conduz a demonstração.                                                   |
| AGES IV coordenador do projeto     | Coordena transversalmente o trabalho entre squads, facilita a critique conjunta e registra decisões ou divergências que afetam o MVP transversal.                                                                    |
| AGES III Tech Lead / Enabling Team | Define e comunica decisões técnicas da squad, verifica arquitetura e dependências, prepara design system e ambiente/agente de IA sob os guardrails dos AGES IV, tem o ownership do code review — conduzido de forma síncrona em colaboração com os desenvolvedores da task — e realiza a aprovação técnica das tasks. |
| AGES I e II                        | Desenvolvem wireframes, wireflows e a PoC em pares, usam IA de forma crítica, verificam o que foi gerado e participam do code review síncrono com AGES III demonstrando o funcionamento da implementação e as evidências de atendimento aos critérios de aceite e à Definition of Done. |
| Stakeholders                       | Participam da elicitação e do User Story Mapping, avaliam a PoC na demonstração, respondem ao formulário de NPS e registram feedback de produto.                                                                     |
| Usuários representativos           | Experimentam os fluxos da PoC enquanto a equipe observa o uso, as dúvidas e as dificuldades, sem que a facilitação da sessão induza as respostas.                                                                    |

O pareamento pode cruzar níveis, como AGES IV com AGES I, AGES II com AGES III, AGES III com AGES I ou AGES IV com AGES II. Cada task assistida por IA é tratada como uma unidade de WIP compartilhada por um par, com WIP de 0,5 por integrante. O par revisa critérios de aceite e Definition of Done durante o trabalho, e a IA não substitui code review nem aprovação dos responsáveis.

### Subtarefas e sequência de trabalho

1. **Selecionar o fluxo core da squad.** Partir do User Story Map colaborativo, confirmar com Stakeholders a jornada prioritária e definir objetivo, hipóteses e requisitos a validar.
2. **Preparar a squad e os critérios.** AGES IV confirma histórias prioritárias e critérios de aceite, enquanto AGES III verifica dependências técnicas, define restrições da PoC e habilita design system, Figma e agente de IA conforme as políticas estabelecidas.
3. **Desenhar o fluxo.** A squad produz wireframes e wireflows que cobrem o caminho core ponta a ponta, e revisa com AGES IV e AGES III antes de construir a PoC.
4. **Construir a PoC em pares.** AGES I e II desenvolvem com apoio de IA, alternam driver e navigator e validam criticamente a saída da ferramenta. Os pares incorporam testes ou evidências adequados ao protótipo e atendem aos critérios de aceite e à Definition of Done.
5. **Revisar e aprovar as tasks.** AGES III (owner do code review) conduz uma sessão síncrona de code review em colaboração com quem desenvolveu a task, que demonstra o funcionamento da implementação. Essa troca promove transferência de conhecimento, aproxima liderança técnica e desenvolvedores e garante o cumprimento da validação e dos critérios de aceite. Na sequência, AGES III realiza a aprovação técnica e AGES IV verifica alinhamento com o objetivo e os critérios de produto. Tasks reprovadas retornam ao par para ajuste e nova revisão.
6. **Demonstrar cada PoC e conduzir a critique.** Cada squad apresenta a solução aos Stakeholders. A critique estrutura feedback sobre o artefato, registra convergências e divergências e resulta numa decisão de direção com justificativa, responsáveis e ações.
7. **Validar com usuários.** Observar usuários representativos tentando completar os fluxos core, registrar evidências e comparar os resultados com as hipóteses e critérios acordados.
8. **Consolidar feedback e atualizar a proposta.** Atualizar histórias, prioridades, riscos e plano das próximas sprints. O registro da decisão informa se a PoC atende ao objetivo ou precisa de ajuste.

### Artefatos da atividade

| Artefato                                       | Finalidade                                                                     | Conteúdo mínimo                                                                                                                                                                                                           |
| ---------------------------------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| User Story Map e definição do MVP              | Registrar a jornada, o fluxo transversal core e a fatia priorizada para a PoC. | Persona ou perfil de usuário, atividades da jornada, histórias, sequência ponta a ponta, recorte do MVP, prioridades, hipóteses e itens fora do escopo.                                                                   |
| Backlog da PoC e critérios de aceite           | Orientar o trabalho da squad e permitir verificar cada task.                   | Épico e história relacionados, task, prioridade, responsável/par, critérios de aceite verificáveis, dependências, requisito não funcional associado e Definition of Done aplicável.                                       |
| Guardrails e configuração de IA                | Orientar o uso permitido e registrar como a plataforma foi habilitada.         | Política aplicável, ferramentas/agentes autorizados, limites de dados, configuração relevante, restrições de segurança e responsável por AGES IV/III.                                                                     |
| Wireframes e wireflows                         | Representar telas e transições do fluxo core antes da PoC.                     | Telas, estados, entradas e saídas, transições, caminhos alternativos relevantes, dados simulados e ligação às histórias/critério de aceite.                                                                               |
| PoC da squad                                   | Permitir que Stakeholders e usuários experimentem a proposta.                  | Fluxo core navegável, versão identificada, componentes e dados mockados assinalados, requisitos atendidos, limitações conhecidas e instruções de demonstração.                                                            |
| Registro de pair programming e code review     | Evidenciar autoria compartilhada, revisão crítica síncrona e aprovação das tasks. | Task/versão, integrantes e níveis do par, alternância driver/navigator, uso de IA relevante, demonstração síncrona dos desenvolvedores no code review com AGES III, testes/evidências, critérios de aceite verificados, aprovação técnica de AGES III e aprovação de AGES IV ou ajustes solicitados. |
| Protocolo e registro de validação com usuários | Orientar observação e preservar evidências do teste da PoC.                    | Objetivo, perfil dos participantes, cenários/tarefas, instruções neutras, observações sem interpretação, dificuldades, dúvidas, resultados por critério e achados prioritários.                                           |
| Formulário NPS e síntese da Sprint Review      | Medir satisfação dos Stakeholders e reunir feedback a cada review.             | Pergunta padrão de recomendação em escala de 0 a 10, identificação opcional do projeto, comentário aberto sobre pontos fortes e oportunidades, cálculo do NPS, principais temas e ações propostas.                        |
| Registro da critique e decisão                 | Consolidar a direção acordada após a demo de cada PoC.                         | Versão demonstrada, feedback por tema, convergências, divergências, decisão, justificativa, responsável, riscos e ações para o backlog.                                                                                   |

O formulário NPS é enviado aos Stakeholders após cada Sprint Review, e a síntese das respostas integra a retrospectiva interna da equipe e o planejamento da sprint seguinte. O NPS é acompanhado junto dos comentários e temas qualitativos, pois a pontuação isolada não explica as causas da satisfação ou insatisfação.

### Critérios de conclusão

A atividade é concluída quando cada squad possui uma PoC demonstrável do fluxo core, as tasks associadas têm code review e aprovações registradas, os testes e critérios de aceite possuem evidências, e os feedbacks de Stakeholders e usuários estão consolidados em decisões e ações para o backlog.

## Parâmetros e acordos registrados na instância sugerida

- Lean Inception organiza o alinhamento do MVP; práticas de Lean Startup podem apoiar a formulação e validação de hipóteses da PoC.
- Coordenação e Stakeholders acordam requisitos não funcionais e critérios observáveis antes da entrada da equipe. A equipe usa esses critérios na arquitetura, nas tasks e na validação do protótipo.
- AGES IV estabelece guardrails, políticas e processos de uso da IA. AGES III os implementa e viabiliza tecnicamente por meio da plataforma, do ambiente e do agente disponíveis às squads.
- O pareamento é a unidade de execução para tarefas apoiadas por IA; a proposta representa WIP 0,5 por integrante e uma task compartilhada pelo par. Os pares são rotacionados para distribuir conhecimento entre níveis.
- A duração, o entregável e a revisão de cada bloco curto são acordados colaborativamente na planning de cada sprint, considerando o tempo restante e os ciclos de feedback previstos.
- A validação da PoC usa observação de usuários e feedback de Stakeholders; os critérios de avanço e os registros das decisões fazem parte dos acordos de trabalho da equipe.
- Após toda Sprint Review, Stakeholders recebem formulário de NPS, e a equipe usa pontuações e comentários para identificar forças, dificuldades e mudanças para o ciclo seguinte. Cada sprint segue um ciclo de planejar, executar, verificar e agir, de modo que as melhorias identificadas sejam incorporadas progressivamente.
- AGES IV registra o processo configurado para sua equipe, seus acordos e os resultados observados, oferecendo base para a reflexão e avaliação na banca.
