# Discovery — EX Account Health — Reunião com o PP

Objetivo: validar, com o PP, o desenho da solução que estamos explorando pra apoiar os CDs no acompanhamento de contas — ainda não é 100% definido que será um "report" no formato tradicional, é uma ideia de solução em construção, então o roteiro evita se comprometer com esse formato. Boa parte do que era Steps 3–7 do Discovery já foi respondido via Slack e pela análise do protótipo/planilhas do próprio PP (ver `PRD/PRD-ex-account-health-scratchpad.md`); este roteiro cobre só o que ainda falta, incluindo a validação de um mini protótipo (duas abas, BigNumbers, estética) que vai ser mostrado a ele diretamente em vez de descrito em texto.

## Perguntas

### Sobre o seu dia a dia hoje
- Quais são os principais processos que você faz no seu dia a dia, relacionados ao acompanhamento das suas contas?
- Quais desses processos te tomam mais tempo?
- Em quais momentos você usa alguma IA pra te ajudar nesse trabalho, e como exatamente você usa? (além da automação pessoal no Claude que você já mencionou)

### Sobre a dor e o motivo de fazer isso agora
- De tudo que a gente já mapeou (dados espalhados, planilha manual, Profitability sempre em branco...), qual desses pontos é o que mais te incomoda de verdade? Se a gente resolvesse só esse, já valeria o esforço?
- **Contexto:** com a mudança pro Delivery Dashboard, entendemos que os CDs vão passar a preencher diretamente lá as informações que hoje alimentam os reports do Quadros e do Fernando — não é só a parte de override do RAG, é a própria fonte desses reports daqui pra frente. Diante disso, quem você acha que precisa estar de acordo com essa solução mais pessoal que estamos construindo — só você, ou o Comercial também entra por causa do acesso à planilha de account planning?

### Validação do conceito — via mini protótipo
Em vez de descrever item por item em texto, vamos mostrar direto um mini protótipo (com as duas abas, alguns BigNumbers, e a estética proposta) e validar ao vivo com ele:
- Isso bate com o que você tinha em mente quando montou seu próprio protótipo?
- Tem algo que parece faltar, ou algo que está ali mas que na prática você não usaria?
- A ordem como as informações aparecem faz sentido pro seu fluxo de leitura, ou você mudaria alguma coisa?

### Testando algumas suposições que a gente já fez
- Os outros CDs usam Slack e Claude do mesmo jeito que você, ou você imagina que isso varia bastante de pessoa pra pessoa? Você acha que todos sentiriam a mesma dor, ou tem gente que já tem um jeito próprio de lidar com isso?

### Dúvidas específicas sobre o desenho da solução
- Sobre o bloco de "recomendação/override do CD": isso deveria ser um texto que você mesmo escreve (de algum lugar que você já registra isso hoje, como o formulário de override do Delivery Dashboard)? Ou, se envolver IA, a ideia não seria substituir o que você já tem em mente — seria a IA sugerir recomendações com base no contexto, podendo te mostrar algo que talvez você não esteja vendo (o mesmo tratamento que já pensamos pra Oportunidades e Riscos). Isso faz sentido pra você?
- Sobre a narrativa que alimenta esse bloco e a síntese do período: hoje ela viria das reuniões/transcrições e do Slack — você também guarda notas pessoais em algum outro lugar (Notion, Evernote, etc.) que devêssemos considerar como fonte?
- Sobre o Proposal Builder (do Indicium.AI): pra fechar o gap de "construir/revisar propostas", ele precisaria de uma conversa ativa com você — nem que seja só pra confirmar o entendimento da proposta, validar a estrutura montada, ou ajustar algo antes de gerar de fato. Esse tipo de interação é um custo aceitável pra você, ou prefere que a gente pense em outro jeito, mais leve, de resolver isso?
- **Aviso, não pergunta:** sobre o Profitability/GM%, mesmo que a gente resolva o acesso técnico ao dado, pode ser que a governança da empresa não deixe esse número aparecer pro CD — isso não é uma decisão sua nem nossa, é algo que vamos sondar direto com a Victória (Delivery Dashboard/VicOps). Só avisando pra você não estranhar se esse número não aparecer na versão final.

### Sobre a conexão com a outra iniciativa (CRM/Comissões)
Contexto rápido pra você entender de onde vem essa pergunta: em paralelo, estamos explorando um problema separado — deals fechando no Salesforce sem os campos de comissão (Consulting Director/Solution Architect) preenchidos. Você mesmo já tem um artefato pessoal que flagra exatamente esse tipo de gap por oportunidade. Isso nos fez pensar: será que faz sentido trazer esse mesmo tipo de sinal (campos de comissão faltando) pra dentro dessa solução que estamos montando pra você, já que ela também olha o detalhe do pipeline comercial (item que já estava no nosso rascunho)?
- Unificar essas duas informações em um lugar só faria sentido pra você, ou prefere que fiquem completamente separadas?
- Isso mudaria a forma como você usaria essa solução no dia a dia?

### O que fica de fora, pelo menos por agora
- Pensando numa primeira versão bem simples: o que você tiraria de escopo sem pena, pra não travar o começo? (ex.: quais informações desse conceito são realmente imprescindíveis já nessa primeira versão, e quais poderiam esperar?)
- As planilhas `[EX] Monitoring` e `Delivery Health - Scorecard Mensal` são usadas só pra alimentar os reports do Quadros/Fernando, ou têm algum outro uso que a gente devia saber?

### Riscos que a gente já enxerga — quer validar contigo
Vou levar a lista de riscos que já identificamos, pra você me dizer se bate ou se eu tô enxergando errado. Você não precisa saber como mitigar cada um — mas se já tiver alguma ideia de como resolver, com um contexto que a gente ainda não tem, é ótimo saber:
- Os dados de origem (Slack, notas do Gemini, planejamento de conta em texto livre) serem bem menos estruturados do que uma planilha — o que dificulta automatizar de verdade.
- A régua de Green/Amber/Red ter espaço pra interpretação (ex: decidir se algo é "recuperável" ou "temporário" depende do seu julgamento), o que pode fazer a sugestão automática discordar de você com frequência e te levar a sempre sobrescrever manualmente.
- A gente ter desenhado tudo pensando só na sua rotina, e isso não bater com o jeito dos outros 7 CDs trabalharem.
- Dependermos do próprio Delivery Dashboard pra ter o histórico de RAG ao longo do tempo (não só o status atual) — sem isso, o indicador de tendência/deterioração não funciona como planejado. Isso é algo que só a Victória e o time dela podem confirmar, mas queria já deixar registrado como uma dependência.
- O jeito como vamos publicar essa solução no Slack (reaproveitando um bot já existente da nossa área) já carrega um risco operacional conhecido — não depende de você, é uma decisão nossa de engenharia, só deixando registrado pra transparência.

Sinta-se livre pra comentar qualquer um dos riscos acima, e também trazer outros riscos ou dependências que a gente ainda não esteja vendo.

---
