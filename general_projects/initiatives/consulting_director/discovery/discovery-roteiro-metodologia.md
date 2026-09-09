# Roteiro de Discovery de Produto

Guia de referência com os passos importantes a percorrer antes/durante um discovery de produto, o que registrar no scratchpad em cada passo, e um banco de perguntas de apoio para preencher as lacunas que normalmente ficam vazias.

**As "Perguntas de apoio"/"Banco de perguntas" de cada passo abaixo são um template genérico, não um roteiro pronto para levar à conversa.** O `discovery_[iniciativa].md` de cada iniciativa (Passo 6) nunca copia essas perguntas como estão — ele é gerado cruzando esse template com o que o Passo 1 (Síntese Pré-Discovery) já levantou do `initial_context/` daquela iniciativa: ponto já respondido no material bruto não vira pergunta (entra como fato conhecido, com fonte, para eventual confirmação leve); ponto parcialmente respondido vira pergunta específica formulada em cima do que já se sabe; só ponto sem nenhuma pista no material bruto herda a pergunta-molde do template quase como está. O roteiro final de uma iniciativa é sempre mais curto e mais direcionado que este template — nunca o template aplicado igual em toda iniciativa.

**Como isso se encaixa com a skill `prd-workflow`:** a skill já cobre um Discovery (Steps 2–7: Pre-Discovery Synthesis, Context and Motivation, Objective and JTBD, CSD Matrix, Out of Scope, Risk & Dependency Synthesis) numa passada só, pergunta-conjunto-por-step. Esse roteiro aqui **não substitui** a skill — é a camada de preparação que roda antes/durante, pra que quando os Steps 2–7 forem preenchidos, as respostas já estejam validadas em vez de serem só suposições de primeira passada. No final deste documento tem a tabela de encaixe, passo a passo, com os Steps da skill.

**Convenção de arquivos:** duas peças por iniciativa —
- `[iniciativa]-scratchpad.md`: notas de trabalho, onde a análise evolui (achados, dúvidas, riscos, log de decisões).
- `discovery_[iniciativa].md`: o roteiro de perguntas que efetivamente se leva pra conversa com o stakeholder.

**Regra fixa, sempre, em qualquer passo:** nunca registrar nomes reais de clientes/funcionários ou valores reais de receita no scratchpad — só a estrutura (nomes de campos, formato, lógica). Mesmo quando a fonte (planilha, print, prototipo) contém dados reais.

---

## Passo 0 — Intake

**O quê:** registrar o que disparou esse discovery e de quem veio — uma reclamação, um pedido direto, um print, uma mensagem no Slack.

**No scratchpad:** uma seção curta no topo, com a fonte e a data.

**Perguntas de apoio (quando a origem é vaga):**
- Quem trouxe isso, e em que contexto?
- Isso já foi levantado antes? Existe algo formalmente registrado (ticket, doc, e-mail, mensagem)?

---

## Passo 1 — Síntese Pré-Discovery

**O quê:** minerar documentos e sistemas existentes **antes** de perguntar qualquer coisa nova ao stakeholder — separar "já sabido" de "gap real", pra não reperguntar o que já está documentado.

**No scratchpad:** seção "Pre-Discovery Synthesis", com uma lista do que já se sabe (com a fonte) e do que continua sendo gap.

**Perguntas de apoio:**
- Existe algum documento, ticket, dashboard, planilha ou conversa anterior sobre isso?
- O que já foi tentado antes? Por que não resolveu?

---

## Passo 2 — Mapeamento de Fontes de Dados e Arquitetura (Stack)

**O quê:** mapear, ainda na fase de discovery, quais sistemas/ferramentas guardam ou processam hoje os dados relevantes pro problema (ex: Salesforce, Bitrix, Snowflake, Databricks, Google Sheets, Slack, Drive), como esses dados fluem entre eles atualmente (mesmo que manualmente, copia-cola, ou "na cabeça de alguém"), e quais acessos/integrações já existem vs. precisariam ser criados. Isso é diferente de uma arquitetura de solução (que vem depois, na fase de Design) — aqui o objetivo é só entender o terreno **como ele é hoje**.

**No scratchpad:** uma seção "Data Sources & Current Stack" — lista por sistema: o que ele guarda, quem tem acesso, como se conecta hoje (API pronta? export manual? nada, é só uma planilha pessoal?).

**Perguntas de apoio:**
- Quais sistemas guardam hoje os dados relevantes pra esse problema?
- Como esses dados se conectam hoje — é automático (API/integração já existente), ou é tudo manual (copia-cola, planilha, export)?
- Existe algum acesso ou integração já pronta em outro projeto que a gente poderia reaproveitar aqui?
- Tem algum dado relevante que só existe "na cabeça de alguém" ou numa planilha/automação pessoal, sem estar em nenhum sistema formal?
- Quem administra cada um desses sistemas — é a mesma pessoa em todos, ou varia?

---

## Passo 3 — Portão: é produto, ou é processo/config?

**O quê:** decisão explícita, o mais cedo possível, sobre se isso é de fato um produto de dados a construir, ou um ajuste de processo/configuração num sistema existente (ex: uma validation rule, um alinhamento de time, uma automação simples). Essa decisão muda se vale a pena seguir pra `prd-workflow` ou não.

**No scratchpad:** registrar a decisão e a justificativa, mesmo que provisória — pode ser revisitada se surgir informação nova.

**Perguntas de apoio:**
- Se a gente resolvesse isso sem construir nada novo, o problema já estaria resolvido?
- Existe alguma trava, regra ou automação simples num sistema que já existe que resolveria a maior parte disso?

---

## Passo 4 — Mapa de Stakeholders

**O quê:** mapear os papéis, que quase nunca são a mesma pessoa — quem sente a dor, quem executa o processo hoje, quem administra o sistema que seria afetado, quem precisa validar a solução final antes de seguir.

**No scratchpad:** uma lista ou tabela papel → pessoa/time.

**Perguntas de apoio:**
- Quem sofre com esse problema hoje, na prática?
- Quem realmente executa esse processo no dia a dia?
- Quem é o dono técnico do sistema que seria afetado por uma solução aqui?
- Quem precisa validar ou aprovar antes da gente seguir adiante?

---

## Passo 5 — Perguntas assíncronas leves (Slack ou similar)

**O quê:** antes de qualquer reunião formal, perguntas pontuais e diretas pra destravar o objetivo/JTBD — principalmente quando marcar uma reunião é difícil ou lento.

**No scratchpad:** seção "Discovery Answers", datada, com a pergunta feita e a resposta recebida.

**Banco de perguntas:**
- O objetivo disso é só [X], ou também [Y]/[Z]?
- Por que isso está sendo levantado agora — rolou algo recente, ou é uma dor antiga?
- O que aconteceria se a gente não fizesse nada?
- Quem mais precisaria estar de acordo com a solução final?

---

## Passo 6 (opcional) — Ferramenta de entrevista estruturada

**Quando usar:** quando o roteiro de perguntas é grande demais pra uma única conversa, ou o stakeholder prefere responder no próprio ritmo (assíncrono).

**O quê:** um roteiro de perguntas organizado por bloco temático (o arquivo `discovery_[iniciativa].md`) — gerado a partir do cruzamento descrito no topo deste documento (template destes passos × Síntese Pré-Discovery do Passo 1), nunca copiado direto do banco de perguntas genérico; se o volume justificar, uma ferramenta própria para responder fora de uma reunião síncrona.

---

## Passo 7 — Minerar artefatos/protótipos que o stakeholder já construiu

**O quê:** sempre perguntar se o stakeholder já tem alguma solução informal própria — planilha, automação pessoal, rascunho, print. Isso costuma ser a fonte de sinal mais rica de todo o discovery, porque mostra exatamente o que a pessoa já sentiu necessidade de resolver por conta própria.

**Regra fixa:** revisar só a **estrutura** desses artefatos — nunca copiar nomes reais ou valores reais pro scratchpad.

**Perguntas de apoio:**
- Você já tem algum jeito próprio de acompanhar isso hoje, mesmo que informal ou incompleto?
- Existe algum rascunho, planilha ou automação pessoal que você já usa pra isso?

---

## Passo 8 — Varredura de iniciativas adjacentes

**O quê:** checar, dentro da empresa, se já existe algo (outro time, outro produto, outra automação) que resolve total ou parcialmente esse mesmo problema — antes de propor qualquer coisa nova.

**Perguntas de apoio:**
- Existe algum outro time ou projeto trabalhando em algo parecido com isso?
- Esse dado ou processo já é tocado por algum outro sistema ou iniciativa que eu deveria conhecer?

---

## Passo 9 — Espaço de possibilidades, sem compromisso prematuro

**O quê:** listar os candidatos de solução que forem surgindo, mantendo linguagem de "possibilidade sendo explorada", não de "decisão", até que o stakeholder valide.

**No scratchpad:** seção "Possible Products/Solutions", atualizada conforme cada possibilidade é explorada ou descartada.

---

## Passo 10 (quando aplicável) — Exploração técnica dirigida

**Quando usar:** quando a solução depende do funcionamento específico de uma plataforma (Salesforce, Databricks, etc.), não só de uma decisão de produto.

**O quê:** pesquisa direcionada na documentação da plataforma, sempre citando fontes, terminando com um "Working read" — um veredito curto resumindo o que aquilo significa pra ideia sendo avaliada.

---

## Passo 11 (quando aplicável) — Validação cruzada com o dono técnico do sistema

**Quando usar:** quando a solução toca um sistema que você não administra diretamente.

**O quê:** ir direto à pessoa que administra esse sistema pra pressionar a ideia antes de assumir que ela é viável — quem só pediu a solução (o stakeholder original) muitas vezes não vê as mesmas restrições que quem opera o sistema por dentro vê.

**Perguntas de apoio:**
- Isso é tecnicamente possível?
- Existe algum efeito colateral que a gente não estaria vendo?
- Quem, na prática, seria afetado por essa mudança — é mesmo quem a gente está pensando?

---

## Passo 12 — Dúvidas em aberto consolidadas

**O quê:** uma lista única e viva de tudo que ainda está em aberto, sempre com um resumo de **por que aquilo importa**. Conforme cada dúvida se resolve, marcar como resolvida (não apagar sem deixar rastro) — e novas dúvidas que forem surgindo entram na mesma lista, nunca espalhadas em outro lugar.

---

## Passo 13 — Riscos e dependências

**O quê:** uma tabela com risco/dependência, evidência (de onde veio esse risco), impacto sugerido, e plano de mitigação — o plano de mitigação só se preenche depois que o stakeholder confirmar o risco, nunca inferido.

---

## Passo 14 — Log de decisões (Judgment Calls Log)

**O quê:** toda virada de entendimento — inclusive correções feitas pelo próprio stakeholder ou por você — registrada com **data** e o motivo da mudança. É o que permite corrigir o rumo sem perder o raciocínio anterior.

---

## Tabela de encaixe com a skill `prd-workflow`

| Passo deste roteiro | Alimenta qual Step da skill |
|---|---|
| 0 — Intake | Contexto geral antes do Step 1 |
| 1 — Síntese Pré-Discovery | Step 2 (Pre-Discovery Synthesis) |
| 2 — Fontes de Dados e Stack | Step 3 (Context and Motivation → As-Is Process/sources) e Step 9 (High-Level Architecture, na fase de Design) |
| 3 — Portão produto/processo | Decide **se** vale a pena seguir pra Step 1 em diante |
| 4 — Mapa de Stakeholders | Step 3 (Context and Motivation → Key Stakeholders) |
| 5 — Perguntas assíncronas | Step 4 (Objective and JTBD) |
| 6 — Ferramenta estruturada | Suporte prático pros Steps 3–7, quando o volume exige |
| 7 — Artefatos do stakeholder | Step 5 (CSD Matrix → Certainties/Assumptions) |
| 8 — Iniciativas adjacentes | Step 5 (CSD) e Step 6 (Out of Scope) |
| 9 — Espaço de possibilidades | Step 5 (CSD → Assumptions) e prepara o Step 8 (Design) |
| 10 — Exploração técnica | Step 5 (CSD) e Step 7 (Risk Synthesis) |
| 11 — Validação com dono técnico | Step 7 (Risk & Dependency Synthesis) |
| 12 — Dúvidas consolidadas | Step 5 (CSD Matrix → Doubts), enriquecido com "por que importa" |
| 13 — Riscos e dependências | Step 7 (Risk & Dependency Synthesis) |
| 14 — Log de decisões | Alimenta o scratchpad que a própria skill já usa |
