# Discovery — EX Account Health — Reunião com o PP (v2)

**Objetivo desta reunião:** validar requisitos, não solução. Independente de qual vai ser o formato final (report, dashboard, alerta no Slack, etc.), essa conversa é sobre confirmar três coisas com o PP: (1) o que ele de fato precisa que esse trabalho resolva, na visão dele mesmo; (2) qual o resultado final que ele espera atingir, se o problema fosse resolvido; e (3) onde exatamente, dentro do processo real do dia a dia dele, está a maior dificuldade.

**O que este roteiro deliberadamente NÃO cobre (fica pra uma etapa posterior, só depois dos requisitos estarem confirmados):** validação do mini protótipo, BigNumbers, lista de conteúdo do report, estética, ou qualquer outra decisão de solução. Tudo isso que já rascunhamos (ver `PRD/PRD-ex-account-health-scratchpad.md`) segue sendo hipótese nossa até agora, não requisito confirmado por ele — misturar essa validação com a de solução arrisca fazer o PP reagir a uma ideia pronta em vez de descrever o problema com as próprias palavras.

## Perguntas

### 4. Validação dos requisitos que já entendemos — um por um
Ao longo do processo, fomos sintetizando várias coisas como se fossem requisitos — mas isso ainda é a nossa interpretação, e pode estar errada, incompleta ou desatualizada. Quero confirmar cada uma diretamente com você, sem pular nenhuma:

**Titularidade e escopo**
- Entendemos que você é o **owner** dessa iniciativa do lado dos CDs — ou seja, as decisões de requisito passam por você, não é só mais um usuário entre outros. Isso está certo? Tem alguém mais que deveria ter esse papel junto com você?
- Entendemos que a solução precisa **atender todos os 8 CDs**, não só você. Isso ainda é verdade do jeito que você imaginou desde o início, ou mudou algo?
- Essa solução deve atender a todos os CDs
- Entendemos que, apesar de servir todos os CDs, **cada um só teria acesso ao próprio portfólio** — ninguém vendo a carteira de outro CD por padrão. Isso é uma exigência sua, ou apenas uma suposição nossa de bom senso?

**O que a solução precisa entregar**
- Entendemos que você quer uma solução que te dê **insights sobre riscos e oportunidades** — não só te mostrar dados brutos, mas te apontar algo que talvez você não tivesse notado sozinho. Isso está certo?
    - Entendemos que essa solução precisa apoiar **ação** (ex: lembrar de dar follow-up, revisar proposta) e não só mostrar informação passivamente. Isso é fiel ao que você quer, ou "apoiar ação" significa outra coisa na sua cabeça?

- Entendemos que a solução também precisa mostrar **indicadores "estáticos"** sobre cada conta — por exemplo, número de deals em aberto, status de saúde da conta, deals já fechados. Esses são os indicadores certos, ou tem outros que pesam mais pra você no dia a dia?
- Entendemos que você quer ver a **cadência/histórico da saúde da conta** — não só a foto de agora, mas como isso vem evoluindo com o tempo. Isso é sobre pegar uma piora antes que ela vire um problema grande, ou tem outro motivo pra isso importar pra você?
- Entendemos que a solução precisa ser capaz de **analisar a aderência ao plano de conta** — e que isso, na prática, significa responder três perguntas: temos oportunidade suficiente pra bater a meta? estamos no ritmo certo (nem adiantado, nem atrasado)? tem algo do lado de delivery ameaçando isso? Falta alguma quarta pergunta que a gente não capturou?
- Entendemos que você quer ter **espaço pra incluir seus próprios insights ou comentários sobre cada conta** — algo que fique registrado ali, não só o que é gerado automaticamente. Isso é sobre substituir onde você já anota isso hoje, ou seria um lugar novo, complementar ao que já existe?
- Revisão e elaboração de propostas é uma solução e visibilidade e proatividade em relação as contas é outra

**Como a informação chega até você**
- Entendemos que a solução precisa **chegar até você de forma ativa** — por exemplo, um alerta no Slack — em vez de depender de você lembrar de abrir algum lugar pra checar. Isso está certo? Só o Slack resolveria, ou tem outro canal que faria mais sentido pro seu dia a dia?
- Entendemos que hoje a informação está espalhada em fontes diferentes (Salesforce, Bitrix, planilhas, reuniões, Slack), e que um requisito real é **centralizar tudo isso num lugar só**. Confirma esse ponto — e, se sim, "um lugar só" significa uma única tela/mensagem, ou só significa não precisar mais abrir 5 lugares diferentes, podendo ainda ser mais de uma visão?

**Fronteira com outras fontes/iniciativas**
- Entendemos que a planilha de account planning não vai ser substituída por essa solução — ela seria uma fonte de dado, não um substituto. Isso ainda faz sentido pra você?
- **Aviso, não pergunta:** um ponto que apareceu na nossa lista de requisitos foi "substituir os reports pro Quadros e pro Fernando" — mas isso já não é mais escopo desta iniciativa. Esses reports passaram a ser responsabilidade de uma iniciativa separada, o Delivery Dashboard, que já está assumindo esse papel. Só deixando registrado pra você não esperar isso daqui.

### 3. O resultado final que você espera atingir
- Independente de como isso vai ser resolvido: se, em 3 meses, esse problema estivesse resolvido, o que estaria diferente no seu dia a dia? O que você conseguiria fazer que hoje não consegue?
(a) identificar oportunidades e manter a velocidade comercial, e (b) identificar risco antes que ele "pegue alguém de surpresa".
- Existe algum sinal que você já usa, na prática, pra saber que uma conta "está bem" ou "está mal"?

### 1. Mapeamento do processo real (o "como", passo a passo)
- Me guia pelo seu processo real de acompanhamento de contas, do começo ao fim, como se eu fosse fazer isso por você pela primeira vez. Quais são as etapas, em que ordem, com que frequência cada uma acontece?
- Em quais desses passos você já usa alguma automação ou IA hoje (Claude, etc.)? O que exatamente ela faz por você, e o que ainda sobra pra você fazer manualmente mesmo com essa ajuda?
- Tem alguma etapa que você faz só porque "sempre foi assim", e que hoje talvez nem sirva mais pra nada?

### 2. Onde está a maior dificuldade, de fato
- De todas as etapas que você descreveu, qual é a que mais consome seu tempo ou energia hoje?
- Essa dificuldade é sobre **ter o dado** (não saber onde/como buscar a informação), sobre **julgamento** (você tem o dado mas decidir o que fazer com ele é difícil), ou sobre **não deixar passar** (esquecer de agir a tempo, mesmo sabendo o que fazer)?
- Se a gente resolvesse só essa etapa, e nada mais, isso já resolveria a maior parte da sua dor? Ou a dificuldade está espalhada em várias etapas pequenas, nenhuma delas dominante?

### 5. Fronteiras — o que é desse problema, e o que é de outro problema
- O Comercial vai ter acesso a essas informações?

### 6. Generalização — isso é só seu, ou é de todos os CDs?
- Você acha que os outros 7 CDs sentem essa mesma dificuldade, do mesmo jeito que você, ou isso varia bastante de pessoa pra pessoa?
- Até onde você sabe, alguém mais já tentou resolver isso com um workaround próprio, do jeito que você fez?
