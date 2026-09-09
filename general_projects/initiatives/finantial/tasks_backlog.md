# Backlog de Tasks — Integração Papel FDE x Área Financeira Global (Anna Hoover)

> Gerado a partir de `iniciativas.md`. Cada item de ação do checklist original foi convertido em uma task pronta para importação em Jira/Bitrix. A ordem das frentes e dos itens dentro de cada frente segue o arquivo original.
>
> **Legenda de sequência:**
> - 🔴 **Iniciar de imediato** — faz parte da ordem 1→4 combinada ao final da call (Vitor + Lorena)
> - 🟡 **Em paralelo** — pode rodar em paralelo à sequência principal
> - ⏸️ **Em hold** — só avança depois que a sequência 1→4 estiver concluída
> - ⚪ **Sem sequência definida** — decidir quando/quem depois

---

## Frente 1 — Discovery com a área de negócio (entrevistas)

### Task 1.1 — Compartilhar materiais e diagramas de processos da área da Ana
**Descrição:** Vitor deve reunir e compartilhar com o time os materiais e diagramas de processos já existentes da área financeira global liderada pela Ana (Anna Hoover), para servir de base de contexto antes da fase de entrevistas de discovery.
**Definition of Done:** Materiais e diagramas recebidos e disponibilizados em local acessível ao time (ex: pasta compartilhada), com confirmação de recebimento.
**Tempo estimado:** 1-2 horas (coleta e compartilhamento; depende de disponibilidade do material já existente).

### Task 1.2 — Estudar materiais recebidos e pesquisar vocabulário financeiro
**Descrição:** Lorena deve estudar os materiais e diagramas de processo compartilhados pelo time da Ana e pesquisar contexto/terminologia da área financeira, de forma a alinhar vocabulário antes de conduzir entrevistas de discovery.
**Definition of Done:** Resumo escrito (ex: notas ou glossário) cobrindo os principais processos e termos financeiros identificados, pronto para orientar a construção do roteiro de entrevista.
**Tempo estimado:** 4-6 horas.

### Task 1.3 — Alinhar iniciativa com Nathan (par de Global Tech) antes da entrevista com Ana
**Descrição:** Conversar com Nathan, par de Global Tech, sobre a iniciativa de integração com a área financeira, antes de agendar a entrevista de discovery com a Ana. Nathan estava de férias no momento da call; conversa estava prevista para a semana seguinte.
**Definition of Done:** Conversa realizada com Nathan, com registro de eventuais pontos de atenção, expectativas ou alinhamentos levantados por ele.
**Tempo estimado:** 30-45 minutos (reunião) + agendamento.

### Task 1.4 — Definir formato estruturado de entrevista de discovery
**Descrição:** 🔴 Definir, em grupo, o formato estruturado a ser usado na entrevista de discovery com a Ana, revisando metodologias já conhecidas (ex: framework "4D", skill de PRD) e pesquisando como esse tipo de entrevista é conduzido atualmente no mercado/área.
**Definition of Done:** Roteiro/formato de entrevista documentado (perguntas-chave, estrutura, objetivos de cada bloco), validado internamente pelo grupo.
**Tempo estimado:** 4-8 horas (pesquisa + elaboração do roteiro).

### Task 1.5 — Testar formato de entrevista com colega próximo
**Descrição:** 🔴 Aplicar o roteiro de entrevista de discovery definido na Task 1.4 com um colega próximo (ex: Jaime) antes de usá-lo com a Ana, para validar clareza das perguntas e ajustar o formato conforme necessário.
**Definition of Done:** Entrevista piloto realizada, feedback coletado e ajustes incorporados ao roteiro final.
**Tempo estimado:** 1-2 horas (entrevista + ajustes no roteiro).

### Task 1.6 — Conversar com financeiro interno (Brasil) para contexto/vocabulário
**Descrição:** Identificar e conversar com alguém da área financeira interna no Brasil, para obter contexto e alinhar vocabulário financeiro antes de realizar a entrevista de discovery com a Ana.
**Definition of Done:** Conversa realizada com pelo menos uma pessoa do financeiro interno, com notas sobre termos, processos e pontos de atenção relevantes para a entrevista com a Ana.
**Tempo estimado:** 1-2 horas (inclui identificação do contato + conversa).

### Task 1.7 — Identificar contato ideal no Brasil para o assunto financeiro
**Descrição:** Vitor deve identificar e indicar o nome do contato mais adequado dentro da operação no Brasil para tratar do assunto financeiro relacionado à iniciativa, para viabilizar a Task 1.6.
**Definition of Done:** Nome e contato da pessoa indicada, compartilhado com o time.
**Tempo estimado:** 30 minutos - 1 hora.

### Task 1.8 — Realizar entrevista de discovery com a Anna Hoover
**Descrição:** 🔴 Conduzir a entrevista de discovery com a Anna Hoover usando o formato validado (Tasks 1.4 e 1.5), com o objetivo de entender os gargalos reais da área financeira global, sem presumir de antemão que a solução será um dashboard.
**Definition of Done:** Entrevista realizada e documentada (gargalos, necessidades, processos atuais registrados), sem conclusões prematuras sobre a solução técnica.
**Tempo estimado:** 1-1,5 hora de entrevista + 2 horas de consolidação das notas.

---

## Frente 2 — Prototipagem de soluções

### Task 2.1 — Criar protótipos realistas para validação com stakeholders
**Descrição:** 🔴 Com base nos achados da entrevista de discovery com a Ana (Task 1.8), criar protótipos realistas (fake/HTML estático, dashboards com dados fictícios) para validar direção da solução com os stakeholders antes de qualquer investimento em infraestrutura real.
**Definition of Done:** Ao menos um protótipo navegável (HTML estático ou similar) apresentado e validado (ou refutado) junto aos stakeholders, com feedback registrado.
**Tempo estimado:** 2-4 dias, dependendo da complexidade dos achados da entrevista.

---

## Frente 3 — Arquitetura e governança da plataforma Databricks

> ⏸️ **Frente em hold**: por decisão de Vitor e Lorena, essa frente só deve avançar depois de concluídas as Tasks 1.4, 1.5, 1.8 e 2.1 (sequência 1→4). Cogitou-se paralelizar essa frente com outra pessoa enquanto o discovery/prototipagem acontece.

### Task 3.1 — Estruturar diagrama de arquitetura/fluxo de dados no Databricks
**Descrição:** ⏸️ Desenhar o diagrama de arquitetura e fluxo de dados da plataforma Databricks para a iniciativa, contemplando o uso do Unity Catalog e a separação de catálogos por área de negócio.
**Definition of Done:** Diagrama de arquitetura publicado (ex: ferramenta de diagramação ou documento), revisado e aprovado pelo time técnico.
**Tempo estimado:** 1-2 dias.

### Task 3.2 — Revisar e organizar roles e grupos de acesso
**Descrição:** ⏸️ Revisar e reorganizar os roles e grupos de acesso da plataforma Databricks para a nova área financeira, usando como referência o material de governança de acesso já produzido para o Snowflake (~15 páginas — Robson sabe localizar o documento).
**Definition of Done:** Proposta de estrutura de roles/grupos documentada, referenciando o material do Snowflake como base, revisada com o time responsável pela governança.
**Tempo estimado:** 1 dia (revisão do material existente + adaptação).

### Task 3.3 — Tornar a definição de roles e permissões mais estratégica/intencional
**Descrição:** ⏸️ Revisar o modelo atual de permissões do sandbox, hoje considerado permissivo demais, propondo uma abordagem mais estratégica e intencional na concessão de acessos e roles.
**Definition of Done:** Documento com diagnóstico do estado atual (permissivo) e proposta de novo modelo de permissões, com critérios claros de concessão de acesso.
**Tempo estimado:** 4-8 horas.

### Task 3.4 — Propor framework de governança de uso de IA
**Descrição:** ⏸️ Elaborar uma proposta de framework de governança para uso de IA na plataforma, com guard rails voltados a usuários sem conhecimento técnico, garantindo uso seguro e responsável das ferramentas de IA.
**Definition of Done:** Documento de framework de governança de IA elaborado, cobrindo ao menos: princípios, guard rails, e critérios de uso para usuários não técnicos; validado com stakeholders relevantes.
**Tempo estimado:** 1-2 dias.

---

## Frente 4 — Observabilidade / Command Center

### Task 4.1 — Avaliar deploy do "Command Center"
**Descrição:** ⚪ Avaliar a viabilidade e o esforço de deploy da ferramenta "Command Center" (desenvolvida pelo Li), voltada à visibilidade de uso da plataforma Databricks.
**Definition of Done:** Relatório/decisão documentada sobre viabilidade de deploy da ferramenta, incluindo pré-requisitos técnicos e próximos passos (go/no-go).
**Tempo estimado:** 4-6 horas.

### Task 4.2 — Definir métricas úteis e validar confiabilidade dos dados
**Descrição:** ⚪ Analisar quais métricas de uso da plataforma são relevantes para acompanhamento e quais devem ser descartadas, comparando os valores apresentados pela ferramenta com os dados brutos para checar sua confiabilidade.
**Definition of Done:** Lista final de métricas aprovadas (com justificativa) e relatório de validação de confiabilidade comparando ferramenta x dados brutos.
**Tempo estimado:** 1 dia.

### Task 4.3 — Conectar iniciativa de observabilidade com o trabalho do Daniel (AI Transformation Office)
**Descrição:** ⚪ Estabelecer conexão entre o trabalho de observabilidade/Command Center e as iniciativas já em curso do Daniel no AI Transformation Office, evitando duplicidade de esforços e buscando sinergias.
**Definition of Done:** Reunião de alinhamento realizada com Daniel (ou equipe do AI Transformation Office), com pontos de conexão e próximos passos documentados.
**Tempo estimado:** 1-2 horas.

---

## Frente 5 — Pesquisa sobre skills financeiras da Anthropic

### Task 5.1 — Pesquisar repositório open source de skills financeiras da Anthropic
**Descrição:** 🟡 Pesquisar o repositório open source publicado pela Anthropic contendo skills relacionadas a mercado/operação financeira, para entender o que já existe pronto e reaproveitável.
**Definition of Done:** Levantamento documentado das skills encontradas no repositório, com breve descrição de cada uma e link de referência.
**Tempo estimado:** 2-3 horas.

### Task 5.2 — Avaliar aplicabilidade das skills financeiras ao contexto interno
**Descrição:** 🟡 Avaliar se as skills financeiras identificadas (Task 5.1) — majoritariamente voltadas a mercado financeiro — podem ser adaptadas ou aplicadas ao contexto de operação financeira interna da empresa (não mercado financeiro).
**Definition of Done:** Análise de aplicabilidade documentada, indicando quais skills (se alguma) são reaproveitáveis, com recomendação de uso ou descarte.
**Tempo estimado:** 2-4 horas.

---

## Frente 6 — Desenvolvimento pessoal

### Task 6.1 — Concluir certificação Cloud Code Architecture
**Descrição:** 🟡 Lorena deve concluir a certificação Cloud Code Architecture, considerada relevante para embasar decisões técnicas no desenvolvimento da plataforma Databricks da iniciativa.
**Definition of Done:** Certificação concluída e certificado obtido.
**Tempo estimado:** Variável conforme carga horária do curso (estimar conforme cronograma do programa de certificação); tratar como estudo pessoal, sem alocação fixa de horas de projeto.

---

## Itens sem sequência definida (decidir quando/quem)

> ⚪ Estes itens correspondem às mesmas ações já detalhadas acima (Tasks 4.1, 4.2, 4.3 e 1.7), mas estavam listados separadamente no arquivo original como "sem sequência definida". Mantidos aqui como referência cruzada, sem duplicar o esforço de execução.

- **Avaliação do Command Center / observabilidade** → ver Tasks 4.1 e 4.2
- **Conexão com as iniciativas do Daniel (AI Transformation Office)** → ver Task 4.3
- **Identificação do contato ideal no Brasil para o assunto financeiro** → ver Task 1.7

---

## Resumo da sequência combinada (referência rápida)

| Ordem | Task | Status |
|---|---|---|
| 1 | Task 1.4 — Definir formato estruturado de entrevista | 🔴 Iniciar de imediato |
| 2 | Task 1.5 — Testar formato com colega próximo / financeiro interno | 🔴 Iniciar de imediato |
| 3 | Task 1.8 — Realizar entrevista de discovery com a Anna Hoover | 🔴 Iniciar de imediato |
| 4 | Task 2.1 — Prototipar soluções fake para validação com stakeholders | 🔴 Iniciar de imediato |
| 5 | Tasks 3.1–3.4 — Arquitetura/governança/roles do Databricks | ⏸️ Em hold até conclusão de 1-4 (pode ser paralelizada com outra pessoa) |

**Em paralelo à sequência acima:**
- Task 6.1 — Certificação Cloud Code Architecture 🟡
- Tasks 5.1 e 5.2 — Pesquisa de skills financeiras da Anthropic 🟡
