# Pig / Lorena - PP's requests

**Data:** 10/08/2026
**Participantes:** Lorena Sales Santos, Vitor Avancini ("Pig", CDO)
**Transcrição completa:** https://docs.google.com/document/d/1gliDExpQM1-dvRqo5BEEY80rhIffxd0kcV0_ZUxz0GU/edit?tab=t.427oc1om4bnz

## Resumo do teor

1:1 de alinhamento entre Lorena e o CDO (Vitor) sobre três iniciativas trazidas pelo PP, todas ainda em fase exploratória/discovery. A conversa cobriu:

- **CRM/Salesforce** — correção do não preenchimento dos campos obrigatórios de comissão. Decisão: priorizar alinhamento/treinamento com os CDs antes de construir automação nova (condicionar o e-mail de repasse + alertas no Slack ficam como camada seguinte, só se necessário).
- **EX Account Health** — a ferramenta de acompanhamento de saúde de conta pros CDs (foco principal deste registro — ver abaixo).
- **Ferramenta de propostas comerciais** — revisar adoção de uma ferramenta já existente (de Mateus Lima) antes de considerar construir algo novo.
- Um fechamento sobre gestão do conhecimento (organizar notas/transcrições dispersas), sem decisão formal.

Nenhuma decisão formal, owner ou prazo foi atribuído ao EX Account Health nesta reunião — ainda está em estágio de escopo do ponto de vista do CDO.

## Pontos levantados — EX Account Health

- **Diagnóstico confirmado:** acompanhamento de conta hoje é manual, disperso (planilhas, Salesforce, Bitrix), no jeito de cada CD, e puramente reativo — narra o que já aconteceu, não antecipa risco/oportunidade.
- **Slack-first confirmado pelo Vitor** (não só ideia da Lorena): toda notificação/informação deve chegar primeiro no Slack, com link pro detalhe. Um app completo só se justifica quando o caso de uso realmente precisar.
- **Novo fato técnico:** o Delivery Dashboard já salva os dados no Databricks — dá pra juntar Databricks + Delivery Dashboard + Salesforce sem pipeline novo. Reduz (não elimina) a dependência do roadmap do próprio Delivery Dashboard.
- **Dúvida de escopo em aberto, levantada pelo Vitor:** essa solução deveria virar uma aba dentro do Delivery Dashboard, ou continuar separada? Lorena levantou a preocupação de o Delivery Dashboard virar uma "grande coisa" genérica, já que o que os CDs precisam aqui é nichado. **Não decidido.**
- **Decisão informal:** separar, por enquanto, o rastreamento operacional (RAG/riscos/delivery health) do comercial (meta de conta/ritmo de vendas) — não juntar tudo num único app de uma vez.
- **Fontes de dado reconfirmadas**, com uma exclusão explícita nova: Salesforce, planilha de RAG, transcrições de reunião, canal de Slack por conta, e a planilha semestral de meta de conta (mais difícil de integrar — muda de formato ano a ano e não está no Salesforce). **Excluído explicitamente pelo Vitor:** notas pessoais dos CDs (Notion etc.) — não são acessíveis de forma centralizada.
- **Próxima entrevista de discovery combinada:** falar com outro CD, deliberadamente não o Igor Benincá (ele já pensa em solução, enviesaria a coleta de dor pura). Nome cogitado, não confirmado: Ricardo Onohara.
- **Itens oficiais de próxima etapa da reunião** (ambos de titularidade da Lorena, sem prazo definido):
  1. Entrevistar Marcelo Vendas — dores comerciais e necessidade de visibilidade sobre saúde de contas do lado Comercial.
  2. Mapear ferramentas comerciais/de proposta já existentes e seu nível de adoção.

## Próximos passos de ação — EX Account Health

1. Escolher e agendar a entrevista com um segundo CD (não o Igor) para coleta pura de dor.
2. Agendar entrevista com o Marcelo Vendas.
3. Levar uma posição própria pro Vitor sobre a dúvida de escopo (aba do Delivery Dashboard vs. solução separada) — não deixar em aberto indefinidamente.
4. Confirmar com o PP se a separação operacional/comercial muda a ordem de prioridade do que ele validaria primeiro no mini protótipo.
5. Check-in com a Victória (Delivery Dashboard) sobre o bloqueio de matriz de acesso e o timeline do Kantata, agora que a integração técnica via Databricks ficou mais simples.
6. Comunicar ao PP a exclusão de notas pessoais (Notion etc.) como fonte, já validada com o Vitor.

*(Ver também `../discovery/PRD/PRD-ex-account-health-scratchpad.md`, entrada de 08/11/2026 no Judgment Calls Log, para o registro completo com citações da transcrição.)*
