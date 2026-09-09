---
title: Manual de Bordo - C6
source: https://docs.google.com/document/d/1htSoPaX2fRno8mnCD1fcX3VgV--OtiZK89lSXuafng8/edit
fetched: 2026-09-09
---

# Manual de Bordo - C6

## Como a gente joga nesse cliente · Projeto de Transformação IA C6

**USO INTERNO INDICIUM** — Não circular fora do time do projeto sem alinhamento com o Delivery Manager.

---

### Os três não negociáveis

**1. Nada do C6 sai do ambiente do C6.**
Dado, código, print, nome de sistema, arquitetura, número. Nem para IA pública, nem para portfólio, nem para post, nem para grupo de amigo.

**2. Nenhuma IA sem autorização.**
IA não é usada em nada do projeto sem aprovação formal e documentada do cliente.

**3. Na dúvida, DM.**
Situação estranha, pressão, conflito, pergunta que você não sabe onde encaixa: fale com o Delivery Manager antes de agir. Dez escalações desnecessárias são melhores que uma tardia.

### Comunicação

| Faça | Não faça |
|---|---|
| Formalize por escrito o que foi combinado em call — thread, canal ou card, mas registre | Deixe combinado importante só na memória de quem estava na reunião |
| Ajuste a linguagem ao público: executivo quer conclusão e impacto, gestor quer decisão sustentada por dado, time operacional quer instrução prática | Use o mesmo material e o mesmo nível de detalhe para C-level e para squad |
| Diga "vou verificar e volto com uma resposta" quando não souber | Improvise resposta técnica na frente do cliente para não parecer perdido |
| Escute até o fim antes de responder — inclusive quando a crítica parece injusta | Responda no impulso, no calor da reunião |
| Avise antes quando não puder participar de uma reunião | Falte sem avisar, ou entre atrasado sem contexto |
| Contextualize quem entrou novo na thread | Presuma que a pessoa leu tudo o que veio antes |

### Compromissos e escopo

| Faça | Não faça |
|---|---|
| Alinhe internamente antes de prometer prazo, entregável, ferramenta ou integração | Assuma compromisso em nome do time para agradar na hora |
| Diga com naturalidade que algo será definido depois do Assessment — o escopo é flexível por desenho | Invente uma definição de escopo que ainda não existe |
| Levante bloqueio e risco de atraso no mesmo dia em que aparecerem | Guarde o risco esperando melhorar sozinho |
| Traga cenário e opção junto com o problema | Leve só o problema e espere que alguém resolva |
| Documente decisão e contexto no lugar acordado da sua frente | Deixe a decisão viva só no chat |

### Dados, segurança e IA

| Faça | Não faça |
|---|---|
| Use as ferramentas homologadas e o ambiente provisionado | Instale extensão, plugin ou add-on não auditado no ambiente do cliente |
| Use dado sintético, anonimizado ou mascarado quando precisar de IA para apoiar raciocínio | Cole código proprietário, credencial, token, API key ou arquitetura em IA pública |
| Avise os participantes antes de usar assistente de transcrição | Grave reunião ou suba áudio e vídeo do projeto em IA externa |
| Reporte imediatamente se enviar dado sensível por acidente — reporte de boa-fé, sem retaliação | Esconda o erro esperando que ninguém perceba |
| Acesse só o que o seu trabalho exige | Explore dado ou sistema fora do escopo por curiosidade |
| Mantenha sua credencial sua | Compartilhe acesso com outra pessoa, inclusive do time |
| Valide toda saída de IA antes de usar — você é o autor e o dono técnico | Entregue output de IA sem revisão, assumindo que está certo |

### Postura no cliente

| Faça | Não faça |
|---|---|
| Fale do C6 como banco que deu o primeiro passo e que a Indicium apoia na próxima fronteira | Fale de gap, falha, atraso ou imaturidade do banco — nem para o cliente, nem entre nós |
| Trate qualquer pessoa do C6 com o mesmo respeito, independente de nível | Ajuste o respeito ao cargo da pessoa |
| Entenda por que alguém pensa diferente antes de discordar | Critique decisão, sistema ou arquitetura do cliente |
| Leve ao DM se for puxado para "de que lado você está" | Opine sobre política ou disputa interna entre áreas do C6 |
| Respeite o canal combinado de comunicação com cada nível | Leve assunto direto a executivo do C6 sem alinhar antes |
| Alinhe com o parceiro antes de comparar plataformas na frente do cliente | Recomende trocar de plataforma ou compare stacks por conta própria |
| Comunique incidente ao cliente só depois de alinhar com o DM | Comunique problema ao cliente sem alinhamento interno |
| Fale do projeto só dentro dos canais do projeto | Fale do C6 em rede social, evento ou canal público |

---

# O resto do manual

*Contexto, técnica e detalhe. Leitura de apoio — vale voltar aqui quando a situação aparecer.*

## 1. Por que este manual existe

Isso não é código de conduta corporativo. É a lista de combinados que evita a maior parte dos ruídos que aparecem em um grande projeto de cliente enterprise.

Todo mundo aqui é tecnicamente muito bom — foi por isso que entrou. O que decide se o projeto vai bem é outra coisa: como o time se comunica, como reage quando algo dá errado, e o cuidado que tem com o que é do cliente.

## 2. O contexto em um minuto

- O C6 tem cerca de 42 milhões de clientes. Qualquer ganho de eficiência se multiplica nessa escala — e qualquer erro também.
- O banco já investiu em licenças de IA e tem mandato do CEO para escalar. A Indicium não está consertando nada: está construindo junto o motor que multiplica esse investimento.
- O projeto roda em ciclos de 3 meses.
- O AITO é a camada transversal que governa o programa: estratégia, governança, medição, padrões e cultura.
- Escopo é flexível por desenho. Métricas e casos de uso definitivos saem do Assessment. "Ainda não está definido" é resposta legítima e pode ser dita ao cliente sem constrangimento.

## 3. Os oito combinados

1. **O óbvio não é óbvio, e deve ser dito.** Se combinou em call, formaliza por escrito. Comunicou? Formalizou.
2. **Fale com o público que está na sala.** Mesmo conteúdo, três traduções: executivo, gestor, operacional.
3. **Compromisso só se for compromisso.** Nada de prazo, escopo ou ferramenta prometidos sem alinhamento interno.
4. **Perspectiva antes de resposta.** Percepção é como você interpreta a foto; perspectiva é onde você põe a câmera. Entender por que alguém pensa diferente não é concordar — é ganhar informação para conduzir melhor.
5. **Não entre em disputa interna do cliente.** Áreas diferentes do banco têm prioridades diferentes, e isso é normal numa organização desse tamanho. O papel da Indicium é técnico e de entrega, não de árbitro.
6. **Levante a mão cedo.** Surpresa executiva destrói credibilidade muito mais rápido que atraso avisado.
7. **Nada do cliente sai do ambiente do cliente.**
8. **Na dúvida, DM.**

## 4. Como nos comunicamos

**Assíncrono** — o receptor lê quando puder. Exige objetividade, porque talvez não dê para tirar dúvida na hora. Antes de mandar, checar: o objetivo está claro? o contexto está completo? tem ação e prazo, se necessário? dá para ler e entender em 1–2 minutos?

**Síncrono** — tempo real. Preparação antes: o que preciso comunicar, para quem, qual o arco (abertura → conflito → resolução), como fecho.

**Por e-mail:** manter a thread, separar em tópicos, usar imagem quando ajudar, e contextualizar quem entrou novo na conversa.

**Conflito: use CNV.** Os quatro pilares, na ordem:

| Pilar | O que fazer |
|---|---|
| Observação | Descrever os fatos, sem julgamento ou interpretação |
| Sentimento / Impacto | Qual o impacto real daquilo |
| Necessidade | O que precisa acontecer, e por quê |
| Pedido / Indicação | Pedido claro, possível e positivo — com prazo |

**Exemplo aplicado ao contexto do projeto:** *"Nas conversas desta semana surgiu a possibilidade de alterar [X]. Isso impacta [Y] porque muda [Z]. Entendemos a necessidade de negócio; para não impactar o cronograma, precisamos de uma definição até o dia [data]. Podemos apoiar essa decisão trazendo os cenários com pontos positivos e de atenção."*

Fechar sempre com apoio e follow-up: "vamos acompanhar isso na próxima reunião, tudo bem?"

## 5. Quando algo sai do controle

**Nem todo problema é crise.** Crise é quando tempo + impacto + visibilidade se combinam.

**Sinais de que virou crise:**
1. A decisão não pode esperar
2. A situação escapa do controle local
3. Há impacto em múltiplas áreas
4. A liderança é acionada fora do fluxo normal
5. O risco reputacional cresce rápido

**Regra prática: se virou assunto de diretoria, já é crise.** Num cliente do porte do C6, isso acontece rápido.

**O que NÃO fazer, nunca:**
- Negar, minimizar ou empurrar para frente
- Comunicar ao cliente sem alinhamento interno
- Procurar culpado durante a crise
- Responder no impulso

**O que fazer:**
1. Pausar. Silêncio em momento tenso não é fraqueza — é o que permite gerar uma hipótese melhor do que a resposta reativa.
2. Acionar o DM imediatamente, antes de responder ao cliente.
3. Estruturar a comunicação em cinco blocos: o que aconteceu (fatos) · impacto para o cliente · o que está sendo feito · próximos passos e prazos · canal de contato.
4. Cadência apertada enquanto durar: check-in curto no início e no fim do dia, board granular, visibilidade total.
5. Quick win. Entrega de alto impacto e baixo esforço para mostrar movimento. O objetivo é mostrar continuidade, não perfeição.
6. Post mortem depois de estabilizar: causa raiz, avaliação da resposta, ajuste de processo, aprendizado registrado.

**Sobre pressão pessoal:** cobrança do cliente é reflexo do contexto profissional, não julgamento sobre a pessoa. Entender a dor do cliente sem ser sugado por ela. Se estiver pesando, isso também é assunto do DM.

## 6. Segurança e uso de IA no cliente

**O treinamento AI Security é obrigatório para todo mundo da Indicium** e é especialmente relevante aqui: este projeto *é* de IA, dentro de um banco. Quem ainda não fez, faz antes de tocar em qualquer ambiente do C6.

**Information Security Training > 5. AI Security > Lesson 5**
https://training.hub.indicium.ai/mod/page/view.php?id=17628

**Resumo do treinamento:**

A IA muda a dinâmica de ataque e defesa por causa da escala e do poder de processamento. A proteção corporativa atua em duas frentes: o uso interno pelos colaboradores (riscos do dia a dia) e o uso externo pelos desenvolvedores (auditoria de prompt, mitigação de prompt injection, proteção das camadas de dado expostas).

**Shadow AI** é o desafio central no dia a dia: uso de ferramenta, extensão ou API não aprovada, que remove a visibilidade de TI sobre o dado corporativo. Compartilhar código proprietário, credencial ou informação sensível de cliente em instância pública treina modelos comerciais externos — isso é vazamento de dado. Instalar add-on de marketplace sem auditoria expõe o sistema local a prompt injection.

Vale **Least Privilege (need-to-know)** e confidencialidade integral em toda interação com IA. Dado sensível (PII, segredo comercial, código-fonte, dado financeiro) só entra em instância corporativa com garantia de não-treinamento. Em ferramenta pública ou gratuita, é proibido enviar dado corporativo — as versões gratuitas usam os prompts para treinar novos modelos comerciais. Prefira dado sintético, anonimização ou masking.

**Na prática:**

| Uso | Pode | Não pode |
|---|---|---|
| Texto | Estruturar ideia, melhorar gramática, traduzir informação pública | PII, dado financeiro, estratégia de preço, dado sensível de cliente |
| Código | Explicar lógica, otimizar SQL genérico, gerar snippet com mock | Lógica proprietária, API key, token, senha, arquitetura completa de sistema |
| Transcrição e resumo | Assistente aprovado, avisando os participantes antes | Áudio, vídeo e transcrição de projeto em IA pública |

**Human-in-the-loop.** A IA é acelerador, não decisor final. Quem gera é autor legal e dono técnico da saída — código, e-mail ou relatório. Toda saída passa por validação de rigor, ausência de alucinação e qualidade antes de qualquer uso em produção. Desconfiança alta com engenharia social gerada por IA (phishing, clonagem de voz): pedido urgente de dado ou dinheiro se valida por canal interno, sempre.

**Regra de ouro em projeto de cliente: nenhuma IA sem autorização.** IA não é usada sem conhecimento prévio e aprovação formal e documentada do cliente. O cliente precisa saber quais modelos serão usados e o impacto nos entregáveis. Isso não é burocracia interna — é o que sustenta a confiança do banco no projeto.

**Se dado sensível for enviado a uma IA pública por acidente:** avisar imediatamente. Existe reporte de boa-fé e não há retaliação. Transparência é o que permite conter o vazamento rápido; esconder é infinitamente pior que errar. Em caso de incidente, levar ao DM, que aciona os canais internos de segurança e define a comunicação com o cliente.

## 7. Trabalhando com os parceiros

O C6 não é um projeto só Indicium + cliente. Tem parceiro de tecnologia dentro da conta, com time próprio, metas próprias e presença nas mesmas reuniões. Na prática isso significa que existe uma terceira leitura da situação em qualquer sala — e ignorar isso gera atrito rápido. A composição atualizada do time do parceiro está na página de stakeholders do projeto.

**Entenda como o parceiro opera.** Saiba quem é o AE (Account Manager) e quem é o SA (Arquiteto de Soluções) na conta, qual a cobertura e quais as metas de cada um. AE é medido por crescimento de conta e consumo; SA é medido por deploy bem-sucedido e adoção. Alinhar a comunicação ao que move cada um não é politicagem — é o que faz a conversa render.

**Chegue com contexto.** Em reunião com parceiro, traga o estágio da iniciativa, a dor do cliente e o próximo passo proposto. Chegar informado e organizado constrói confiança; chegar cru queima duas vezes, com o parceiro e com o cliente.

**Alinhe a narrativa antes de falar com o cliente.** Orientação de arquitetura, mensagem de valor e pitch conjunto se combinam antes da reunião com o C6, não durante. Contradição entre Indicium e parceiro na frente do cliente custa credibilidade dos dois lados.

**Avise antes de acionar.** Nada de contato com o cliente sobre tema do parceiro sem o parceiro saber. Comunique muito, compartilhe atualização com frequência, registre decisão.

**Sobre plataforma e comparação.** Este é o ponto mais sensível do dia a dia:
- Não critique a plataforma do parceiro na frente do cliente. Se houver limitação técnica real, ela é levada ao parceiro e ao DM — não vira reclamação em reunião com o C6.
- Não recomende trocar de plataforma, nem sugira alternativa de outro fornecedor, por conta própria.
- O stack de ativação do projeto é multi-modelo por desenho. O que não é esperado é fazer comparação de produto, benchmark ou recomendação de preferência sem alinhamento prévio.
- Se o cliente pedir comparação de componentes entre plataformas, traga o parceiro para dentro da conversa e construa a conclusão em conjunto. Comparação feita pela Indicium sozinha, mesmo bem-intencionada, queima a relação.
- Pergunta de custo, dimensionamento ou otimização de plataforma não se responde sozinho. Vai para o DM, que aciona o parceiro. Otimização sem alinhamento prévio é o jeito clássico de perder um parceiro.

**Cenário win-win.** O objetivo é o cliente crescer com os dois. Achou uma oportunidade de valor para o C6 que passa pelo parceiro? Leve ao DM em vez de deixar morrer.

## 8. Antes de entrar em qualquer reunião com o C6

- Sei qual é o objetivo e quem vai estar na sala
- Sei qual é o público e adaptei a linguagem
- Sei o que posso e o que não posso comprometer
- Se vou trazer problema, trago também cenário e opção
- Se o tema toca parceiro, a narrativa está alinhada com ele
- Sei quem registra o combinado depois

**Depois:** formalizou? Se não, ainda não terminou.

## Materiais que originaram este manual

Conteúdos da Indicium AI Academy, somados ao material de kick-off e planejamento do projeto:

- Comunicação Eficaz e o Relacionamento com Clientes Externos — Cursos de Soft Skills, Times Técnicos (2025)
- Liderança Ágil em Situações Difíceis com Clientes — Plano de Soft Skills, Lideranças Técnicas · Gestão de Crise (2026)
- Communicating with Partners: How we co-deliver with partners — Soft Skills for Leadership (2025)
- Information Security Training > 5. AI Security > Lesson 5 — treinamento obrigatório
