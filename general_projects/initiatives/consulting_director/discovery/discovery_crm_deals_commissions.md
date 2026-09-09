# Discovery — CRM: Repasse de Novos Deals e Comissões

Objetivo: resolver as dúvidas em aberto registradas em `PRD/PRD-crm-deals-commissions-scratchpad.md`. Já sabemos que a solução não é um produto de dados — é um ajuste de processo/automação no Salesforce. São duas reuniões separadas (PP e Beatriz), organizadas aqui em duas seções — cada uma com as perguntas certas pra aquela pessoa.

---

## Reunião com o PP

Foco: a experiência de quem preenche os campos, e o segundo gap que ele trouxe (alertas de andamento perdidos do Bitrix).

### Sobre a ideia do alerta proativo no Slack
A ideia: antes do deal ser marcado como Ganho, mandar um aviso no Slack se os campos obrigatórios ainda estiverem em branco — pra pegar o problema mais cedo.
- Os campos "Consulting Director" e "Solution Architect" de um deal costumam já estar decididos bem no início dele, ou só ficam claros perto do fechamento? (Isso importa porque um alerta disparado cedo demais pode não ter nada de útil pra avisar ainda.)
- Depois de quantos dias com o campo em branco você acha que faria sentido disparar esse alerta?
- Quem deveria receber esse alerta — só o dono do deal, o gestor dele também, ou outra pessoa?
- Esse alerta deveria se repetir (ex: todo dia até ser resolvido) ou ser só um aviso único?

### Sobre uma alternativa que surgiu — não travar o deal, e sim segurar o aviso pro Financeiro
Descobrimos com a Beatriz que dá pra reabrir/editar um deal já Ganho — o problema real é que o e-mail automático de repasse pro Financeiro dispara uma única vez, no momento do fechamento, com a foto do que existia até ali.
- Se em vez de travar o fechamento do deal, a gente simplesmente **atrasasse o envio do repasse pro Financeiro** até os campos estarem preenchidos (sem impedir você ou o AE de fechar o deal normalmente), isso faria sentido pra você?
- Isso teria algum efeito colateral que você enxerga (ex: atraso na comissão de quem já preencheu certo, se o repasse for por lote)?

### Sobre o segundo gap — alertas de andamento de deal (Bitrix vs. Salesforce)
Você mencionou que perdeu, na migração pro Salesforce, os alertas automáticos que o Bitrix mandava sobre o andamento dos seus próprios deals — e por isso criou um artefato pessoal no Claude que roda toda sexta de manhã.
- Esse é um problema separado do preenchimento das comissões, ou você vê os dois como a mesma dor no fundo?
- Você sabe se os outros CDs sentem falta da mesma coisa, ou têm algum workaround parecido, ou nem notaram essa perda?
- O jeito que você organizou seu artefato pessoal (os contadores de gaps, os filtros, a visão por conta) já reflete bem o que seria ideal, ou foi só o que deu pra montar rápido?
- Faz sentido pra você que a gente pense numa solução formal/oficial pra isso, ou seu artefato pessoal já resolve suficientemente bem? (Importante: não estamos assumindo que a solução final seria necessariamente um artefato como o seu — é só uma das possibilidades, já que nem todo CD é tão técnico quanto você.)

### Pra confirmar o que já assumimos
- Só pra confirmar: é você mesmo, CD, quem entra no Salesforce e preenche "Consulting Director"/"Solution Architect", certo? Nunca é o AE preenchendo em seu nome?

---

## Reunião com a Beatriz

Foco: viabilidade técnica no Salesforce e o andamento do alinhamento com os CDs. Beatriz é do Financeiro, com forte conhecimento de Salesforce.

### Sobre a nova ideia — segurar o e-mail de repasse em vez de travar o deal
Você já confirmou que dá pra fazer isso tecnicamente, mas levantou um risco novo: o Operações depende desses e-mails pra algum processo interno de alocação.
- Você consegue detalhar melhor o que exatamente o Operações usa desses e-mails? É algo que precisa chegar exatamente no momento do "Ganho", ou eles teriam margem pra receber um pouco depois, já com as informações completas?
- Isso seria mais simples de implementar do que a trava no fechamento do deal, ou dá no mesmo trabalho?

### Sobre a sua ideia — alerta quando um deal fechado é alterado
Você sugeriu adicionar um alerta pra quando alguém altera um deal já fechado, em vez de descobrir informalmente como acontece hoje.
- Essa ideia funcionaria bem sozinha (sem a ideia de segurar o e-mail), ou você vê ela mais como um complemento?
- Quem deveria receber esse alerta — só você, o Financeiro todo, ou também quem administra os processos do Operações?

### Perguntas técnicas — trava e auto-preenchimento
- Quem, hoje, tem permissão de admin pra criar ou alterar validation rules e Flows no nosso Salesforce, além de você?
- Os campos "Consulting Director" e "Solution Architect" são preenchidos manualmente sempre, ou existe algum lugar no Salesforce (ex: um time padrão da conta, um responsável já definido em outro campo) que já sabe quem deveria estar ali antes mesmo do deal ser criado?
- O app nativo "Sales Cloud for Slack" já está instalado e conectado no nosso Salesforce?
- O PP mencionou que acha que existia uma trava de envio/fechamento do deal quando o CRM era o Bitrix. Existia mesmo?

### Sobre a responsabilidade e o alinhamento com os CDs
- Quando fica marcada a call de alinhamento síncrono com os CDs que você mencionou? Isso muda algo em como devemos seguir agora — vale esperar o resultado dela antes de avançar numa solução técnica, ou seguimos em paralelo?

### Sobre outras pessoas/iniciativas envolvidas
- Você mencionou que está resolvendo isso com outras pessoas além do Financeiro e dos CDs. Quem mais está envolvido, e alguém já tentou resolver isso antes de um jeito que não deu certo?
- Existe algum outro time (RevOps, Sales Enablement, Comercial) que já tenha tentado atacar esse mesmo problema?

---
