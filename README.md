# Ideias de melhoria para o Fluxo AGES

Notas iniciais do grupo para a proposta do Trabalho Final de Melhoria de Processos. Estas ideias ainda devem ser discutidas e consolidadas antes de serem incorporadas ao fluxo BPMN e ao detalhamento da etapa escolhida.

## Participação dos grupos

- Promover a participação coletiva de todos os membros do grupo — AGES I, II, III e IV — desde a elicitação e análise até a especificação dos requisitos.
- Realizar demonstrações a cada entrega para cada grupo.

## Redesenho do Sprint 0

Substituir o Warm-Up atual por uma adaptação de Inception, com práticas de Design Sprint e validação rápida, mantendo o trabalho iterativo e colaborativo em vez de concentrar as definições em uma sequência que possa tornar o processo cascata.

### Inception como propósito da Sprint 0

- Entender Inception como um momento estruturado de alinhamento entre as pessoas envolvidas sobre problema, usuários, proposta de solução e o MVP a construir — não apenas como apresentação inicial, estudo de ferramentas ou preparação logística. A Lean Inception é descrita por seu autor como um workshop colaborativo para alinhar a proposta de solução e definir o MVP; suas práticas podem ser adaptadas ao contexto e ao tempo da Sprint 0 ([referência](https://caroli.org/lean-inception-3/)).
- Na proposta, a Sprint 0 combina esse alinhamento com uma Spike/PoC: depois de mapear e priorizar o core, a equipe constrói um protótipo funcional e o valida com Stakeholders/usuários. O resultado esperado é aprendizado e feedback que reduzam incerteza e orientem o backlog das sprints seguintes; não é necessário concluir um produto com backend.
- O User Story Mapping e o brainstorming com Stakeholders ajudam a formar entendimento comum do problema e do MVP. A equipe então consolida as histórias, explicita hipóteses e dependências e prepara uma PoC que permita validar os fluxos de maior risco ou valor.

1. **Apresentação e integração:** apresentar a equipe e seus membros. Prever conversas 1:1 com AGES IV ao longo do projeto.
2. **Elicitação com stakeholders:** no encontro de elicitação, todos os membros do grupo participam junto aos Stakeholders. Fazer uma dinâmica de brainstorming para levantar requisitos e construir colaborativamente o User Story Map, com participação dos Stakeholders.
3. **Consolidação, análise e priorização:** após o encontro, a equipe consolida o User Story Map, analisa as histórias e requisitos levantados, prioriza o backlog e define o core do produto (MVP), considerando também o retorno dos Stakeholders.
4. **Protótipos de baixa fidelidade:** dividir a equipe em grupos menores, de 2 a 4 pessoas, para criar wireframes dos fluxos core.
5. **Wireflows:** desenhar os fluxos de navegação entre os wireframes.
6. **Protótipo de alta fidelidade e preparação do ambiente:**
   - AGES IV definem o protótipo de alta fidelidade;
   - AGES III preparam o design system, configuram o Figma e configuram o agente de IA;
   - AGES I e II constroem o protótipo.
7. **Validação:** etapa mencionada nas notas originais como “Validação com”; participantes e forma de validação ainda precisam ser definidos.

## Ordem proposta para os encontros iniciais

- **Ordem atual, conforme anotação do grupo:** apresentação da AGES → apresentação do projeto/equipe → reunião de elicitação com Stakeholders.
- **Ordem proposta:** apresentação da AGES → reunião de elicitação com Stakeholders (brainstorming e User Story Mapping colaborativo) → apresentação do projeto/equipe.
- A mudança antecipa a conversa sobre necessidades e requisitos. Depois da elicitação, a equipe consolida e analisa o mapa, prioriza as histórias e define o core/MVP; os resultados podem ser retomados com os Stakeholders para alinhamento.

## Papéis e responsabilidades

- **AGES IV Coordenador:** coordena o trabalho dos grupos.
- **Demais AGES IV:** atuam como líderes/gestores de cada squad e criam e especificam os épicos, compostos por uma ou mais User Stories (USs). A gerência também cuida das features/histórias e de sua priorização.
- **AGES III:** atuam como Tech Leads de cada squad, com autonomia técnica. Trazem o conhecimento de arquitetura — componentes, serviços, infraestrutura e dependências entre módulos — para aproximar os requisitos do trabalho técnico. Junto com o restante da squad, auxiliam na decomposição das USs em tasks: unidades técnicas de trabalho necessárias para concluir as histórias e, consequentemente, os épicos.
- **AGES I e II:** compõem a equipe da squad, executam as tasks e se reportam ao AGES III.

## Planejamento e colaboração

- Todos os membros — AGES I, II, III e IV — participam da planning, realizada logo após o encontro com stakeholders na review, além das atividades de especificação e priorização.
- A gerência (AGES IV) mantém a responsabilidade pelos épicos e features/histórias; a equipe da squad, com liderança técnica do AGES III, organiza o trabalho técnico em tasks.
- A participação conjunta busca reduzir a distância entre os requisitos e sua implementação, incorporando desde o planejamento o conhecimento técnico do AGES III sobre arquitetura e dependências.

## Direcionamento para o fluxo proposto

Estas notas orientam o primeiro rascunho de **O Fluxo AGES Proposto**. O arquivo `O_Fluxo_AGES_Atual.bpmn` permanece como referência do processo atual; as propostas devem ser avaliadas contra ele, sem misturar as duas versões. O rascunho está em `O_Fluxo_AGES_Proposto.bpmn`.

## Etapas do fluxo atual

Esta síntese alinha o BPMN atual (`O_Fluxo_AGES_Atual.bpmn`) ao material visual `ProcessosAGES-ProcessoAGES-v6.png` e ao Anexo 1 do enunciado. Os nomes das quatro etapas abaixo são os do Anexo 1. **Pré-AGES** é usado aqui somente como apelido para o processo de identificação, seleção e definição de projetos que antecede a execução.

1. **Etapa 1: Identificação, seleção e definição de projetos: Semestre que antecede a execução do projeto na AGES.** O material mostra `Apresentação da Ideia pelos stakeholder`, `Validação da Ideia`, `Definição do semestre que o projeto irá ser executado`, `Reuniões mensais com os Stakeholders`, `Validação dos Requisitos` e `Elaboração do Termo de Abertura de Projetos`. As reuniões, validação dos requisitos e elaboração do termo aparecem em um ciclo de alinhamento antes da execução.
2. **Etapa 2: Organização e kick-off do projeto.** Na `Semana Inicial`, aparecem `Apresentação Inicial AGES e do Fluxo AGES.` e `Apresentação do Processo da AGES, responsabilidades e artefatos, apresentação dos relatórios (sprint, andamento e final)`. O `Warm Up (Sprint 0)` começa com `Apresentação dos projetos pelos stakeholders`; em seguida, o material apresenta `Documentação dos Requisitos e Mockups (Time)`, `Definição Arquitetura ou revisão (AGES III)` e `EAP / Cronograma / Plano de Comunicação / U.S. (AGES IV)`, antes de `Apresentação para stakeholders`. Também registra `Estudos das tecnologias utilizadas nos projetos (linguagens e metodologias TDD, BDD, Code review, pair programming, etc..)`. O BPMN atual representa os três trabalhos intermediários em paralelo.
3. **Etapa 3: Sprints iniciais e Revisão intermediária.** O material agrupa `Sprints 1 e 2`, apresenta um ponto `Após a sprint 1` e depois agrupa `Sprints 3 e 4`. Cada `Sprint Duas Semanas` contém `Planning`; `Aula Meeting` e `Desenvolvimento Documentação` em paralelo; `Entrega para os Stakeholders`; `Retrospectiva`; e `Entrega do relatório da Sprint`. Após a Sprint 1 também ocorrem `Entrega Relatório de Andamento` e `ONE on ONE (com os alunos)`. No BPMN atual, esse ONE on ONE está na lane `Professor Orientador`; as anotações do grupo especificam que é individual, com cada aluno.
4. **Etapa 4: Encerramento.** O material registra `Retrospectiva geral da AGES + Confraternização`, `Entrega Relatório Final`, `Apresentação dos projetos da AGES (estudantes + stakeholders + professores)` e `ONE on ONE (com os alunos)` na `Semana Final`. O BPMN atual posiciona a apresentação das bancas após os Sprints 3 e 4 e antes dessa semana. **Correção informada pelo grupo:** na prática, `Apresentação das BANCAS` para AGES IV acontece depois das atividades da Semana Final. Manter essa diferença explícita nas anotações até atualizar o diagrama de referência; no fluxo proposto, representar as bancas após a semana final.

Assim, os nomes e agrupamentos das etapas permanecem fiéis ao Anexo 1, enquanto a informação mais recente do grupo sobre o momento das bancas fica identificada como correção da sequência representada no material original.

### Requisitos não funcionais no Pré-AGES

- Durante a **Etapa 1: Semestre que antecede a execução do projeto na AGES**, a Coordenação deve elicitar e validar com os Stakeholders os requisitos não funcionais relevantes ao projeto, aproveitando as `Reuniões mensais com os Stakeholders` e a `Validação dos Requisitos` do processo atual.
- Registrar esses requisitos com critérios verificáveis e exemplos de aceitação, conforme o contexto do projeto: por exemplo, segurança e privacidade, desempenho, disponibilidade, usabilidade, acessibilidade, manutenibilidade ou restrições de plataforma. A lista deve ser acordada com os Stakeholders, não presumida como igual para todos os projetos.
- Esses acordos devem integrar os requisitos e o Termo de Abertura antes do início do trabalho da equipe AGES. Na etapa seguinte, servem de entrada para arquitetura e planejamento da PoC; na validação, ajudam a definir o que precisa ser demonstrado ou medido, mesmo quando o protótipo usa dados mockados ou não possui backend.

- **Descoberta antes da entrada da equipe:** adaptar a referência ao “modelo Gartner” trazida pelo grupo, usando o Double Diamond na relação entre Coordenação e Stakeholders. A Coordenação conduz Descobrir/Definir, valida requisitos funcionais e não funcionais e esclarece critérios de qualidade, segurança, desempenho e demais restrições. A equipe discente AGES I–IV concentra sua atuação no segundo diamante — Desenvolver/Entregar soluções — depois desse alinhamento inicial.
- **Sprint 0 como Inception + Spike/PoC:** incorporar práticas de Lean Inception para alinhar problema, usuários, solução e MVP, e então investigar o core por meio de um protótipo funcional. A equipe pode construir uma PoC sem backend ou usando dados mockados, para representar os fluxos principais e permitir que Stakeholders/usuários experimentem a solução e deem feedback específico. Lean Startup pode complementar a validação de hipóteses; a combinação de práticas ainda será decidida pelo grupo.
- **Trabalho da Sprint 0:** AGES IV coordena o fluxo de construção do protótipo; AGES III prepara o design system (incluindo variables e styles com base na identidade visual) e o ambiente/agente de IA; AGES I e II usam IA como apoio para construir os protótipos de alta fidelidade dos fluxos trabalhados pelas squads. O protótipo pode incluir interação e dados simulados, sem exigir implementação do backend.
- **Revisão técnica e gerencial:** cada task passa por code review do AGES III e aprovação do AGES III e do AGES IV antes de ser considerada concluída. Se houver ajustes, retorna para execução e nova revisão. Nas sprints seguintes, o mesmo ponto de controle deve fazer parte do fluxo de desenvolvimento.
- **Validação com usuários ao final da Sprint 0:** observar usuários representativos usando o protótipo e registrar dúvidas, dificuldades e feedback. Observação e uso são uma técnica candidata; a técnica de UX, os participantes, os critérios de sucesso e a decisão de seguir/iterar ainda precisam ser combinados com Stakeholders.
- **Ciclo de feedback:** se a PoC não validar o core ou revelar problemas relevantes, atualizar o protótipo/backlog e repetir a validação; se atingir os critérios acordados, seguir para as sprints regulares. O feedback de Stakeholders e usuários alimenta a priorização e o refinamento das histórias.
- **Uso de IA:** explicitar no fluxo onde a IA apoia a produção do protótipo de alta fidelidade. A IA não substitui code review, validação humana, critérios não funcionais nem aprovação dos responsáveis.

### Pontos para decidir durante a revisão

- Quais práticas de Lean Inception serão usadas na Sprint 0 e se práticas de Lean Startup serão combinadas para testar hipóteses da PoC.
- Qual técnica de validação de UX será aplicada, quem serão os usuários e quais critérios indicam que a PoC pode avançar.
- Como os requisitos não funcionais serão registrados, priorizados e verificados nas tarefas e entregas.
- Como serão definidos os limites de uso do agente de IA, os dados de entrada permitidos e a revisão dos artefatos gerados.
- Se a aprovação de AGES III e AGES IV será exigida em toda task ou se haverá critérios por tipo/risco da task, conforme a proposta anotada pelo grupo.
