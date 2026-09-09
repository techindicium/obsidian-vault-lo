# EX Account Health — Respostas ao Roteiro de Discovery (Passos 1, 2, 4, 7, 8)

> Consolidado a partir de `initial_context/core_problems.md`, `PRD/PRD-ex-account-health-scratchpad.md`, `PRD/PRD-ex-account-health.md` e os registros em `meetings/`. Foco objetivo: só o que importa para elaboração do design.

## Objetivo principal da iniciativa

Dar a cada Diretor de Consultoria (CD) uma ferramenta pessoal que centraliza, num lugar só, a informação hoje dispersa sobre suas contas — status RAG, pipeline comercial, contexto narrativo (reuniões, Slack), financeiro — para que ele veja sinais de risco e oportunidade **antes** que aconteçam, em vez de reconstruir esse quadro manualmente a cada ciclo. Nas palavras do próprio PP (11/08/2026), sucesso é *"a centralização da informação... pra melhor tomada de decisão"* — decisões de alocação, novas propostas, ações com cliente. Escopo: os 8 CDs da consultoria, cada um só com acesso ao próprio portfólio.

---

## Passo 1 — Síntese Pré-Discovery

- Acompanhamento de conta hoje é manual e disperso entre Salesforce, planilhas de rentabilidade (Bitrix/Operações), transcrições de reunião (Gemini), Slack, Drive e a planilha de account planning — e é **puramente reativo**, não antecipa risco/oportunidade (confirmado por Vitor Avancini, CDO, 10/08/2026).
- Já existe uma rubrica RAG determinística (Overall + 4 blocos: Profitability, Delivery Health & Pulse, Growth, Risks) na planilha `Delivery Health - Scorecard Mensal`. Este produto vai **consumir** esse RAG, não recalculá-lo.
- O bloco de Profitability (GM%) fica em branco na maioria dos meses porque o dado só é acessível a Operações/Financeiro hoje.
- Solução deve servir a todos os CDs (aproximadamente 8), cada um só com acesso ao próprio portfólio.
- JTBD validado: identificar oportunidades/manter velocidade comercial, e identificar risco precocemente — que PP depois reenquadrou de forma mais ampla como "melhor tomada de decisão" (alocação, rentabilidade, risco de pessoas).
- Meta de conta ("account planning") não é um número simples puxado de sistema — é definida em conjunto por CD e Account Executive, mas a titularidade do número é do Comercial; mistura cálculo, especulação e algo conhecido do cliente (ex: orçamento anual de IA do cliente).

---

## Passo 2 — Mapeamento de Fontes de Dados e Arquitetura (Stack)

| Sistema/Fonte | O que guarda | Dono/admin | Como se conecta hoje |
|---|---|---|---|
| CRM (Salesforce) | Pipeline, dados de contrato, estágio de proposta, consumo de contrato (faturado vs. total) | Financeiro | Acesso via integração Salesforce MCP que o time da Lorena já construiu — reaproveitável |
| Delivery Scorecard (planilha mensal, alimenta o Delivery Dashboard) | RAG Overall + 4 blocos | Operações | Confirmado como fonte do RAG; exposição de histórico ao longo do tempo ainda em aberto |
| Rentabilidade/margem (GM%) especificamente | Realizado vs. meta, base do bloco Profitability | Operações hoje (em planilhas); Salesforce cogitado como fonte futura, sem prazo | Acesso restrito aos CDs hoje — bloqueio técnico e de governança |
| Planilha de account planning | Visão de portfólio (uma linha por conta: cliente, CD, Account Executive, status, tier A/B/C, indústria, potencial de receita do ano); bloco detalhado por conta (meta mensal, campo "weighted revenue", stack do cliente); tabela por engagement (solução, probabilidade, modelo de billing, taxa horária, horas mês a mês, total anual) | Comercial | Confirmada estruturada e extraível; os 8 CDs usam a mesma planilha |
| Transcrições de reunião (Gemini) | Matéria-prima pra síntese narrativa, sinal de risco/oportunidade | Cada CD, individualmente | Acesso via SSO pelo MCP de Google Drive/Slack, com a credencial do próprio CD — sem convite manual de usuário de serviço. Depende do CD estar convidado (ao menos como opcional) na reunião |
| Slack (canais por conta) | Sinal adicional de risco/oportunidade, chatter do dia a dia | Cada CD, individualmente | Mesmo mecanismo SSO acima, via MCP de Slack |
| Planilha de alocação (Operações) | Alocação de squad — quem está staffado em qual conta | Operações | Fonte atual confirmada; sendo substituída pelo Kantata, sem prazo |
| Contatos-chave do lado do cliente | Stakeholders do cliente por conta/proposta | Não confirmado | Nenhuma fonte identificada ainda |
| Delivery Dashboard (tela de Portfolio) | Ponto de acesso pro dado do Delivery Scorecard acima — não é fonte em si | Iniciativa paralela (Fernando/Victória) | Dependência de coordenação, não questão de dado |

**Quem administra varia por sistema** — não é uma pessoa/time único: Financeiro (Salesforce), Operações (Scorecard, margem, alocação), Comercial (account planning), cada CD individualmente (transcrições, Slack), e a equipe do Delivery Dashboard (Victória) pra tudo que passa por ali.

**Fato técnico (Vitor Avancini, 10/08/2026):** o Delivery Dashboard já grava seus dados no Databricks — dá pra juntar Databricks + Delivery Dashboard + Salesforce sem construir um pipeline novo.

**Reuso identificado:** integração Salesforce MCP já existente (time da Lorena) e o padrão de acesso via MCP (Drive/Slack), já usado em outro projeto interno (`ai_databricks_daily_intelligence`).

---

## Passo 4 — Mapa de Stakeholders

| Papel | Pessoa/time |
|---|---|
| Sofre a dor hoje | Os 8 CDs — PP é o mais vocal e o mais processual; Onohara tem processo bem menos estruturado ("guarda tudo na cabeça") |
| Executa o processo hoje | Cada CD, individualmente, sem padronização entre eles |
| Dono técnico — CRM/pipeline | Financeiro (Salesforce) |
| Dono técnico — Scorecard/margem/alocação | Operações |
| Dono técnico — account planning | Comercial |
| Dono técnico — camada Delivery Dashboard/Databricks | Victória (iniciativa paralela Delivery Dashboard) |
| Valida direção/escopo | Vitor Avancini ("Pig"), CDO |
| Sponsor/owner formal | **Indefinido** — candidatos sugeridos por PP: Quadros (VP de Consultoria) ou Fernando (Operações) |
| Segundo CD entrevistado (checagem de generalização) | Ricardo Onohara (13/08/2026) |
| Stakeholder comercial ainda não entrevistado | Marcelo Vendas — dor comercial e necessidade de visibilidade de saúde de conta do lado Comercial |

---

## Passo 7 — Artefatos que o stakeholder já construiu

*(Revisão só de estrutura — nenhum nome real de cliente/funcionário ou valor real de receita foi copiado pra qualquer documento do projeto.)*

- **`initial_context/ex-account-health-prototype.pdf`** — rascunho/protótipo do próprio PP, exemplificando como seria o report mensal completo. Fonte de sinal mais rica do discovery até agora — mostra exatamente o que PP já sentiu necessidade de resolver por conta própria.
- **Automação pessoal informal (Claude + planilha)** — já usada por PP pra filtrar a planilha `[EX] Monitoring` só pras contas dele, pra montar seu rascunho pessoal — evidência de que uma abordagem LLM + planilha já funciona informalmente.
- **Mapa de stakeholders pessoal do PP** — identificado como desatualizado (~1 ano) e incompleto — sinal de adoção fraco pra ferramentas de centralização em geral, relevante pro risco de generalização.

---

## Passo 8 — Varredura de iniciativas adjacentes

- **Delivery Dashboard** (Fernando/Victória) — iniciativa paralela e formal que já assumiu os 4 pilares (rentabilidade, delivery health, growth/pipeline via Salesforce, riscos qualitativos), reportados mensalmente pelos 8 CDs com write-back direto no banco. Dependência de coordenação ainda em aberto do lado deles (bloqueio de matriz de acesso, timeline do Kantata), mas a integração técnica ficou mais simples porque o Delivery Dashboard já grava no Databricks.
