# Lorena / PP - EX Account Health

**Data:** 11/08/2026
**Participantes:** Lorena Sales Santos, Pedro Portela ("PP")
**Transcrição completa:** https://docs.google.com/document/d/1T4VRS5sA2jfbaFmjqR50spXmTZ5gEcv1IbqVzZBuoiw/edit?tab=t.efntmftbq4jb

## Resumo do teor

Reunião de discovery com o PP, rodada contra o roteiro `discovery/discovery_ex_account_health_v2.md` (foco em validar requisitos, não solução). Na prática, boa parte da conversa (~25 dos ~38 minutos) foi sobre o **Delivery Dashboard** — iniciativa paralela e agora formalizada por Fernando, com 4 pilares (rentabilidade, delivery health, crescimento/pipeline via Salesforce, riscos qualitativos), todos os 8 CDs reportando mensalmente, com write-back direto no banco. A validação de requisitos específica do EX Account Health ficou concentrada nos últimos ~9 minutos.

As Seções 1 e 2 do roteiro (mapeamento do processo do dia a dia, onde está a maior dificuldade) **não foram cobertas** nesta reunião — o PP referenciou uma conversa anterior, mais pontual, como já tendo coberto esse terreno. Vale confirmar se essa cobertura anterior foi de fato suficiente.

Nenhuma decisão de owner/sponsor foi fechada — o PP recusou explicitamente esse papel pra si mesmo.

## Pontos levantados — EX Account Health

- **Owner/sponsor ainda indefinido:** o PP recusou ser o dono da iniciativa ("não sei se eu sou a pessoa correta") e recomendou o VP de Consultoria (Quadros) ou Operações (Fernando) como possíveis sponsors. **Não decidido.**
- **Confirmado, sem ressalva:** solução atende os 8 CDs, cada um só com acesso ao próprio portfólio; quer insights de risco/oportunidade; quer indicadores estáticos por conta (deals abertos/fechados, saúde da conta); quer espaço pra incluir comentários/insights próprios, persistidos.
- **Definição de sucesso, nas próprias palavras do PP:** centralizar a informação dispersa em um lugar só, pra apoiar decisões de alocação, novas propostas e ações com o cliente — não é sobre gerar retorno financeiro direto, é "bem intangível", sobre visibilidade e melhor decisão.
- **Canal de entrega:** alerta no Slack é aceitável, mas o PP revelou preferência pessoal por um **artefato vivo no Claude** em vez de Slack.
- **Rebaixado a nice-to-have:** aderência ao plano de conta (o PP questionou se isso é papel do CD ou do Comercial — "não temos meta de vendas"); apoio a ação/follow-up (ele já usa lembrete de calendário próprio); histórico/cadência da saúde da conta (adiado pra feature futura, dado o momento de reestruturação).
- **Confirmado como fora de escopo:** revisão/criação de propostas é um processo totalmente separado (o próprio fluxo "Play" do PP) — ele foi categórico que não deve ser misturado aqui.
- **IA para insight — direção corrigida:** o PP é cético sobre IA gerar recomendação a partir de transcrição de reunião (prefere comentário manual, assinado por pessoa), mas se empolgou com uma ideia diferente — IA cruzando contexto da conta com dado *externo* (concorrência, tendências de mercado) pra sugerir oportunidade real.
- **CRM/Comissões confirmado como problema diferente:** o PP foi categórico que esse gap não deve compartilhar solução/artefato com o EX Account Health — é uma questão operacional do Financeiro, misturar desvia o foco.
- **Novo risco:** reestruturação em andamento na área de Consultoria/CDs, com impacto ainda incerto nos processos e relatórios.
- **Novo achado de qualidade de dado:** o artefato pessoal do PP tinha uma contagem desatualizada (de antes da migração pro Salesforce) e um erro de mapeamento de conta (Itaú vs. Fundação Itaú) — o próprio PP não tinha notado antes da IA apontar.
- **Contexto organizacional:** clima de corte de custo/eficiência está moldando a preferência do PP por iterar rápido em vez de buscar a solução perfeita.

## Próximos passos de ação — EX Account Health

1. Re-perguntar diretamente ao PP os dois objetivos originais (oportunidades/velocidade comercial vs. risco antecipado) nessas palavras exatas, já que a resposta dele nesta reunião foi mais ampla ("melhor tomada de decisão") e não fechou uma priorização entre os dois.
2. Confirmar se o Comercial deveria ter acesso a alguma parte dessa solução, já que o próprio PP sugeriu que aderência ao plano de conta é "mais de interesse do Comercial do que do CD".
3. Validar com outro(s) CD(s) se a dificuldade e as preferências mapeadas até aqui (muito baseadas no PP) realmente generalizam — o "sim" do PP sobre isso na reunião foi cordial, não uma validação real.
4. Decidir se a ideia de IA cruzando contexto externo (concorrência/tendências) pra sugerir oportunidades entra como item formal do report, e revisar/retirar a expectativa de blind-spot detection a partir de transcrições internas.
5. PP vai enviar o link da planilha do projeto de Delivery Dashboard por e-mail.
6. Lorena vai levantar exemplos concretos de risco de rentabilidade/pessoas, pra refinar o filtro de "risco relevante" que o PP pediu.
7. PP vai liberar acesso ao documento "Play" (preparação/validação de proposta), caso valha explorar esse processo separadamente no futuro.
8. Sem responsável definido ainda: decidir quem será o sponsor final (VP Consultoria/Quadros ou Operações/Fernando).

*(Ver também `../discovery/PRD/PRD-ex-account-health-scratchpad.md`, seção "Discovery Meeting with PP — Requirements Validation (08/11/2026)" e a entrada correspondente no Judgment Calls Log, para o registro completo com citações da transcrição. Ver também `../discovery/PRD/PRD-crm-deals-commissions-scratchpad.md` para a resolução da dúvida em aberto 13, decidida nesta mesma reunião.)*
