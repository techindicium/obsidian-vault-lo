# Scratchpad — Delivery Dashboard (R&D, Americas)

> Consolidado a partir de: (1) Transcrição da reunião "Validação Protótipo" — 20/07/2026, (2) PRD v3.2 (EN) — 22/07/2026, e (3) mensagens no Slack (canal `#C0BJMSCD92Q`) — 04–05/08/2026. Última atualização: 05/08/2026.

## 0. Papéis e stakeholders do projeto

**Owner do projeto (Business/Product Owner):**
- **Victória de Souza Beira** (VicOps) — Process Team Leader | Operational Efficiency. PM e autora do PRD; dona de praticamente todos os Open Issues de definição de regra de negócio e da matriz de acesso (OI-15).

**Stakeholders principais (Americas Leadership / VP — consumidores do Overview e da saúde do portfólio):**
- **Fernando de Souza**
- **Matheus Dellagnelo**
- **Daniel Quadros**

**Consulting Directors (CDs):** responsáveis pelo write-back qualitativo (Delivery/Risk/Commercial) na tela Portfolio, restrito às próprias contas.

**Time do produto/protótipo (participantes recorrentes nas discussões e no Slack):**
- **Vitor Avancini** — liderança de R&D; define a filosofia de execução (prototipagem rápida com feedback contínuo)
- **Joana Elisa Soares da Silva** — autora/mantenedora do protótipo e do PRD
- **Eduarda Gonçalves Prestes** — comunicação de status, updates no Slack, anúncio da V1
- **Gabriel Klock** — Head of Projects; principal interessado nos indicadores de utilization e contratos
- **Aluizio Cidral Júnior** — engenharia de dados (DBT, Kantata/Bitrix/Salesforce)
- **Ana Sara Silva Cunha** — participante da reunião de validação
- **Lorena Sales Santos**

## 1. Objetivo principal do projeto

- Reconstruir o dashboard de delivery para a **Americas** em **Databricks**, unificando a camada operacional (status de projetos, risco, margem, utilização, renovações) com a camada de reporte executivo — hoje fragmentada em planilhas isoladas e apresentações manuais.
- Fonte de verdade única: **Kantata/Salesforce** (BigQuery removido desde v3.0 — fora de escopo).
- **Instância europeia (`dashboard.indicium.ai`) permanece intocada** — deploy paralelo, sem cutover, sem disrupção. Time Americas não pode alterar o dashboard europeu (dependência atual que o projeto resolve).
- Filosofia de execução (definida por Vitor Avancini na reunião): **prototipagem rápida com loop de feedback constante**, evitando ciclos longos de entrega. O PRD deve ser atualizado continuamente a partir do uso real do protótipo ("Command Deck"), não escrito e travado de uma vez.

## 2. Decisões tomadas

### Da reunião (20/07)
- Integrar dados do **Salesforce** para permitir filtros regionais (Brasil / EUA / Europa) no dashboard.
- Separar **Utilization** (indicador operacional, por time/pessoa) de **Pessoas/Equipe** (senioridade, tempo no time, engajamento) — são visões distintas.
- Navegação **consolidada/hierárquica**: visão macro → clicar para detalhar por time → por pessoa. Evitar proliferação de abas.
- Priorizar **indicadores tangíveis** (contratos, dados quantitativos já existentes) antes de indicadores qualitativos, para não sobrecarregar os times com processos administrativos novos.
- Overview deve ser **enxuto** (poucas métricas, direto ao ponto) — não uma tela "com um milhão de coisas".
- Manter registros de observações **dentro do próprio app** (não baixar CSV) para viabilizar histórico de evolução.
- Aluizio Cidral Júnior priorizaria **adaptar o código do front-end**, não o modelo de dados/DBT, para reconciliar diferenças entre o modelo americano e o europeu — visão de longo prazo é unificar em um único DW da empresa.
- Aluizio Cidral Júnior comprometeu-se a disponibilizar dados de contratos na plataforma até **sexta-feira** (usando Salesforce).

### Do PRD v3.2 (formalizadas)
- Portfolio é a **tela prioritária** do produto (antes era só uma entre várias).
- Write-back qualitativo (Delivery/Risk/Commercial) feito pelos **Consulting Directors (CDs)** direto no app, via formulário "Engagement Status Update" — substitui a planilha semanal e o antigo "Account Executive Status" (4 quadrantes) da v3.1.
- **CSAT removido do escopo do V1** — será tratado no futuro via percepção qualitativa + análise de IA de transcrições, não formulário.
- Autenticação **nativa Databricks** (workspace SSO + Unity Catalog groups) — sem OAuth externo, sem Supabase.
- Todos os dados de write-back (riscos, RAG, status) vivem em **Delta tables no Unity Catalog**.
- Todos os projetos ativos serão migrados para o **Kantata**.
- CDs confirmados com acesso **restrito ao Portfolio**, escopado às próprias contas (leitura + write-back de status). Acesso às demais telas ainda em definição (ver OI-15).

## 3. Bloqueios / Open Issues (PRD, seção 11)

| # | Questão | Owner | Bloqueia |
|---|---|---|---|
| OI-1 | Qual objeto do Kantata guarda alocação diária/semanal por pessoa/projeto? | Kantata Admin | Calendar tab (V3) |
| OI-2 | O que substitui o score de moral/engajamento (antes vinha do BigQuery)? | Victória de Souza Beira + CDs | KPIs V1 |
| OI-3 | Fonte do headcount de serviço por prática (D&AI/Projects/Consulting)? | HR / Data Eng | Overview (V2) |
| OI-7 | Salesforce Account tem campo de região (BR/US) ou precisa criar mapeamento? | Salesforce Admin | Filtros Portfolio (V1), Rankings (V2) |
| OI-8 | O workspace Databricks suporta Databricks Apps? | Databricks Admin | Infra V1 |
| OI-11 (novo v3.2) | Salesforce expõe campo/objeto de intenção de renovação? | Salesforce Admin | Overview — Renewal risk (V2) |
| OI-12 (novo v3.2) | Salesforce armazena/pode receber headcount estimado por oportunidade? | Salesforce Admin / Sales | Pipeline — bench coverage (V3) |
| OI-13 (novo v3.2) | Quando o timesheet do Kantata estará disponível para utilização por pessoa em tempo real? | Kantata Admin / PMO | Operational Efficiency — drill-down (V4) |
| OI-14 (novo v3.2) | Regra exata de "no renewal": todo contrato sem oportunidade aberta vinculada é risco, independente da proximidade do fim? | Victória de Souza Beira + Sales | Overview — Renewal risk (V2) |
| **OI-15 (novo v3.2)** | **Matriz de acesso por tela**: quais personas (Leadership/VPs, PMO, Delivery Leads) têm leitura/escrita em Overview, Pipeline, Operational Efficiency, Rituals, PMO Indicators? Especialmente sensível — Operational Efficiency expõe dados de compensação, Pipeline expõe dados comerciais. | **Victória de Souza Beira** | **Bloqueia permission grants de V1–V4 para todas as telas além do Portfolio** |

**Riscos principais (seção 10 do PRD):**
- R1 — Schema do Kantata difere entre org EU e Americas → precisa audit completo antes do build V1.
- R2 — Kantata pode não ter alocação diária → calendar heatmap cai para granularidade semanal (fallback já definido).
- R4 — Databricks Apps pode ter limitações de UX vs. um app React completo → spike de validação na Fase 0 (semana 1).
- R5 — Baixa adoção do write-back pelos CDs se o formulário tiver fricção (planilha é "mais rápida") → sessão de design com 2 CDs + pilot com 1 conta antes do build V2.

**Preocupação levantada na reunião (Gabriel Klock):** risco de sobrecarregar os times com mais um processo/campo de preenchimento qualitativo sem garantia de adoção — motivo pelo qual o grupo priorizou indicadores tangíveis (contratos) antes do qualitativo.

## 4. Owners / responsáveis (ações da reunião)

- **Joana Elisa Soares da Silva, Gabriel Klock, Eduarda Gonçalves Prestes, Vitor Avancini** → dar feedback no PRD (comentários + screenshots).
- **Joana Elisa Soares da Silva** → atualizar o PRD com requisitos detalhados de utilização, contratos e status de projetos.
- **Gabriel Klock** → enviar indicadores/resumos que já acompanha com Fernando de Souza para o time.
- **Aluizio Cidral Júnior** → deploy do DBT para integração de contratos no Salesforce (prazo: sexta-feira); listar discrepâncias entre o modelo de dados americano e europeu.
- **Joana Elisa Soares da Silva + Eduarda Gonçalves Prestes** → alinhar e criar a primeira versão do protótipo.
- **Victória de Souza Beira** (owner central de negócio/produto) → dona de praticamente todos os Open Issues de definição de regra e da matriz de acesso (OI-15).

## 5. Roadmap (PRD, seção 12)

| Fase | Escopo | Semanas | Entrega-chave |
|---|---|---|---|
| 0 — Foundations | Ambiente Databricks, conector Salesforce, schema + tabelas suplementares, audit Kantata | 1 | Infra viva, SF fluindo pro Delta, auth via SSO |
| 1 — V1 Core | Squad grid, Portfolio read-only c/ filtro BR/US, Overview KPIs | 2–4 | Dashboard V1 read-only ao vivo — **✅ entregue em 04/08/2026, ver seção 7** |
| 2 — V2 Overview | Overview completo, rankings Top10 BR/Top5 US, renewal risk | 3–5 | Overview substitui slide 1 da liderança |
| 3 — V2 Portfolio write-back | Form "Engagement Status Update", write-back de CDs restrito às próprias contas | 5–7 | Status por conta ao vivo, substitui slide 2 |
| 4 — V3 Squad Detail | Calendar heatmap, Revenue chart, Burndown, Margin | 6–8 | Tabs completos de squad (read-only) |
| 5 — V3 Write-backs + Pipeline | Risks, RAG, Delivery Updates write-back, tela de Pipeline com bench coverage | 8–10 | Write-back completo + Pipeline |
| 6 — V4 PMO | Operational Efficiency (drill-down por pessoa), Gantt, Rituals c/ attachments, Permissions UI | 10–15 | Extensão PMO completa |

**Validação/change management combinada:**
- V1 (semana 4): onboarding com o time de delivery Americas, sanity check vs. dashboard europeu.
- V2 (semana 7): pilot do Overview com 1 VP; validar setas MoM em 3 contas.
- V3 (semana 10): acompanhar adoção do write-back via audit log das Delta tables.
- V4 (semana 15): revisão completa de adoção.
- Feedback loop: revisão estruturada de 30 dias após cada versão.

## 6. Pontos de atenção / não esquecer

- **PRD e protótipo devem evoluir juntos, diariamente se possível** — é o "maior desafio" citado por Vitor Avancini: manter cadência de feedback rápida enquanto dura a fase de prototipagem.
- Overview (v3.2) **removeu** CSAT, "needs justification" e "projects needing attention" — não recriar sem necessidade validada.
- **Não alterar o modelo de dados/DBT** para acomodar diferenças regionais — adaptar o front-end. Objetivo de longo prazo é um DW único da empresa.
- A tela de **observações/rituais** foi cogitada para reaproveitar o "agente de cerimônias" (hoje pensado para sprint ceremonies) — ainda não validado se a ferramenta entende reuniões de acompanhamento de projeto (não-sprint). Ideia paralela: monitorar "vibe"/sentimento das reuniões via IA.
- **OI-15 é o bloqueio mais crítico em aberto** — sem a matriz de acesso definida por Victória de Souza Beira, nenhuma tela alem do Portfolio pode liberar permissões em V1–V4.
- Dados sensíveis: Operational Efficiency (compensação) e Pipeline (comercial) exigem controle de acesso cuidadoso — mencionado tanto no PRD (OI-15) quanto implícito na discussão sobre visão de "Pessoas" (senioridade, alocação) na reunião.

## 7. Status atual e updates via Slack

> Fonte: canal Slack `#C0BJMSCD92Q`, thread iniciada por Eduarda Gonçalves.

### V1 entregue (04/08/2026)
- A **V1 do Delivery Dashboard já está no ar**: [link do app](https://prod-delivery-dashboard-2011778299619571.aws.databricksapps.com/) (login via SSO). ([Slack](https://indiciumai.slack.com/archives/C0BJMSCD92Q/p1785844027623429))
- Limitações conhecidas desta V1 (ainda pendentes):
  - Dados de **delivery US e BR ainda não disponíveis** — aguardando liberação no Kantata.
  - Aba **Pipeline** já contempla todas as regiões.
  - Aba **Portfolio** contempla todas as regiões, **exceto** delivery US e BR.
  - Aba de **Indicadores de PMO ainda não populada** nesta versão.
  - V2 já está em andamento.

### Prazo do Kantata e plano de contingência (04–05/08/2026)
- **Prazo dos dados de delivery no Kantata: 1º de setembro de 2026.** ([Slack](https://indiciumai.slack.com/archives/C0BJMSCD92Q/p1785844071757939))
- **Plano de contingência (novo, ainda não estava no PRD)**: até lá, dados serão extraídos do **Bitrix** para suprir o dashboard nesse intervalo.
- **Prioridades confirmadas para os dados via Bitrix**:
  1. **Portfolio** — para preencher o RAG.
  2. **Overview → Componente de Capacidade**.

### Investigação técnica do Aluizio (thread [`#C0BHJ2WF2E9`](https://indiciumai.slack.com/archives/C0BHJ2WF2E9/p1785938267446949))
- Respondendo à questão de onde/quais dados do Bitrix entrariam, o Aluizio mapeou um **modelo canônico**: uma segunda fonte (Bitrix) alimentando os mesmos `marts/core`, sem alterar o app ou os dashboards existentes.
- **Diferenças na regra de negócio de "Utilization" entre Europa (Kantata/Kimble) e Americas (Bitrix)** — não é a mesma fórmula:
  - **Kantata/Kimble**: `ResourceUtilisationIncludedUsage / ResourcePaidUsage` — horas faturáveis sobre horas **pagas** ao recurso. Por definição, a métrica **satura em 100%** (o numerador é um subconjunto do denominador).
  - **Bitrix**: hora apontada em tarefa sobre horas **contratadas** — são duas medidas independentes, sem relação de subconjunto, então a métrica **não tem teto** (pode passar de 100%).
  - **Escopo do que entra no numerador também difere**: o Bitrix, por padrão, conta qualquer hora apontada em tarefa — inclusive trabalho **interno** (RH, L&D, Financeiro, R&D etc.), não só trabalho faturável de cliente. O Kimble já isola só o que é faturável.
  - **Base de data também é diferente**: o modelo atual do Bitrix (`agg_team_utilization`) recalcula as horas pela **data de fechamento da tarefa** e descarta tarefas ainda abertas — o que pode subestimar o volume real de trabalho em andamento.
  - Consequência prática: números de "utilização" do Bitrix e do Kantata **não são diretamente comparáveis** hoje sem ajustes — é preciso alinhar regra de negócio (o que conta como faturável, qual denominador usar, qual base de data) antes de tratar os dois como equivalentes.

### ⚠️ Pendência — aguardando decisão dos stakeholders
- Está tecnicamente mapeado como usar o Bitrix como fonte provisória (enquanto o Kantata não chega, previsão 01/09), mas **ainda não há decisão dos stakeholders sobre o caminho a seguir**: se as diferenças de regra de negócio acima são aceitáveis para uso provisório no Overview/Portfolio, e em qual parte exata do app essa fonte entraria. Fica pendente com Joana Elisa Soares da Silva, Fernando de Souza e Vitor Avancini. (05/08/2026)
