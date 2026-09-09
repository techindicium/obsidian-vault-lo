# Core Problems — Diretoria de Consultoria (CD)

Documento de descoberta de problemas para a iniciativa de melhoria de processos da Diretoria de Consultoria. Consolida os problemas coletados até agora, o contexto levantado com os stakeholders e as decisões de escopo já alinhadas. Última atualização: 2026-07-30.

---

## Issue 1 — CRM: Repasse de Novos Deals e Comissões

**Impacto:** atraso no pagamento de comissões e retrabalho para o Financeiro.

### Descrição do problema

Problema no preenchimento no Salesforce: campos imprescindíveis ficam em branco, o que prejudica o Financeiro e atrasa o pagamento das comissões dos envolvidos.

Como alguns campos foram adicionados recentemente ao CRM para facilitar este processo, é preciso reforçar como preenchê-los corretamente.

### Processo correto de preenchimento

1. Abra a oportunidade no Salesforce.
2. Clique na aba "Sales Architect".
3. Localize a seção "Opportunity Team (Commissioned)".
4. Preencha o nome completo de todas as pessoas envolvidas na venda que devem receber comissão, nas posições corretas (SA, CD, Expert).

Esse preenchimento precisa ser feito **antes** que a oportunidade seja marcada como Ganha, já que o repasse para o Financeiro é gerado automaticamente neste momento.

### Como validar se os deals estão com as informações preenchidas

1. Filtre suas oportunidades: crie uma visualização de lista no Salesforce com as oportunidades em que você já está incluído no time.

**Caminho:** Salesforce > Opportunities > Ícone de Configuração > New > Save > Ícone de Filtro > Filter by My Opportunity Teams > Save

---

## Issue 2 — Acompanhamento de Delivery Health por Cliente

> **Nota de escopo (2026-09-03):** os dois reports manuais e as duas planilhas descritos na seção "Reports existentes hoje" abaixo **não fazem mais parte do escopo desta iniciativa** — o Delivery Dashboard (iniciativa separada) já assumiu esse reporting, confirmando a Open Question #11 do scratchpad (`PRD/PRD-ex-account-health-scratchpad.md`). Já refletido em `PRD/PRD-ex-account-health.md` (Seção 1 e Seção 4 — Out of Scope). Mantido abaixo apenas como registro histórico do contexto que originou a iniciativa.

### Descrição do problema

Os diretores de consultoria (CDs) reportam mensalmente informações para o time de Operações, dependendo de dados dispersos:
- Rentabilidade (Salesforce + Bitrix)
- Oportunidades comerciais (Salesforce)
- Contexto dos projetos (anotações Gemini, canais do Slack, docs no Drive...)
- Planejamento de conta

O acompanhamento atual é feito nesta planilha: [\[EX\] Monitoring](https://docs.google.com/spreadsheets/d/1J1BnWQrpf5nXUlGH0Tqg_J4AwFFvkNm_o8egBxIWL00/edit?gid=247561991#gid=247561991&fvid=105490373) e [Delivery Health - Scorecard Mensal](https://docs.google.com/spreadsheets/d/122LZcjZh1RHQo0F8WkmytS2JkSvpn9PufT2G33If0mA/edit?gid=522186944#gid=522186944)

Rascunho que o stakeholder montou para exemplificar o que ele quer: [protótipo EX Account Health](claude://cowork/shared-artifact?uuid=019faee2-3a17-7421-8554-4007b24fac22)

### Reports existentes hoje

Ambos alimentados pelas mesmas fontes dispersas listadas acima:

| Report | Cadência | Destinatário | Conteúdo |
| --- | --- | --- | --- |
| Semanal | Toda semana | Quadros | Apenas saúde da conta (delivery health) |
| Mensal | Todo mês | Fernando | Análise completa: rentabilidade, funil de vendas (pipeline comercial) e riscos |

O rascunho do stakeholder (link acima) é a representação de como seria o report completo que o Fernando precisa (o mensal), com todas as informações consolidadas por conta.

### Framework RAG usado na consolidação mensal

A aba `Delivery Health - Scorecard Mensal` da planilha já define um framework RAG (Red/Amber/Green), com 4 blocos + 1 status geral, cada um com critério objetivo de classificação:

| Bloco | Green | Amber | Red |
| --- | --- | --- | --- |
| RAG Geral | Conta saudável no geral, sem problemas materiais. Coerente com os blocos. | Algo exige atenção ou acompanhamento; um bloco fora do trilho, mas gerenciável. | Conta em risco material; algo falhando que precisa de Operations agora. |
| Profitability | GM% no target ou acima (ou dentro de pequena tolerância). Economia saudável. | GM% abaixo do target, mas recuperável ou temporário. Pressão sendo gerenciada. | GM% bem abaixo do target sem caminho claro de volta, ou conta deficitária. |
| Delivery Health | Entrega no trilho, cliente satisfeito. Pulse 4-5, sem problemas de prazo ou qualidade. | Atritos pontuais: atrasos, qualidade ou sinais mistos do cliente. Pulse 3, recuperável. | Entrega comprometida, cliente insatisfeito, escalações ou compromissos perdidos. Pulse 1-2. |
| Growth | Conta crescendo, ou estável de forma saudável, com plano de conta no trilho. | Estagnada ou atrás do plano, pipeline limitado. Precisa de um movimento de crescimento. | Conta encolhendo, risco de redução de escopo ou churn. Tendência de redução. |
| Risks | Sem riscos ou bloqueios materiais. Nada a escalar. | Riscos ou bloqueios conhecidos sendo gerenciados. Algo a monitorar, pode precisar de apoio. | Bloqueio ativo ou risco de alto impacto que exige intervenção de Operations agora. |

**Princípio da planilha:** classificar a realidade do mês, não a expectativa; na dúvida entre dois níveis, escolher o mais cauteloso; todo Amber e Red vem com comentário explicando o porquê e o que está sendo feito para voltar a Green/Amber.

### Mecanismo de sugestão automática + override do CD

Visto no rascunho do stakeholder: para cada conta, o painel cruza as fontes disponíveis (nota consolidada da reunião semanal EX, anotação automática do Gemini, mensagens do Slack, pipeline do Salesforce, histórico de pulso semanal 1-5) e propõe um status Verde/Amarelo/Vermelho segundo as regras da tabela acima.

Essa sugestão não é definitiva: o CD pode sobrescrevê-la manualmente (clicando em Verde/Amarelo/Vermelho no painel), e é essa escolha manual que fica salva como status final da conta. **A automação propõe, o julgamento final é do CD.**

### Gap identificado

O bloco de Profitability (GM%) fica em branco na maioria dos meses na planilha atual, porque esse dado hoje só está acessível ao time de Operações/Financeiro, não aos CDs.

### Alinhamentos confirmados com o stakeholder (Pedro Portela)

- **Abrangência:** a solução deve atender a todos os CDs da consultoria (hoje: Igor Medeiros Benincá, David Teles Eller, Daniel Padula de Quadros, Douglas Morales Monteiro, Pedro Portela, Joshua Goldner, Márcio Sumariva Nandi, Ricardo Pacheco Onohara), não só a carteira do stakeholder que desenhou o rascunho.
- **Reports:** a solução deve atender aos dois reports (semanal de Quadros e mensal de Fernando) de forma integrada, não apenas um dos dois. O rascunho compartilhado representa o report mensal completo, destinado ao Fernando.
- **Regra de status:** o status sugerido deve seguir as regras determinísticas já definidas na planilha `Delivery Health - Scorecard Mensal` (tabela RAG acima), não uma classificação livre por LLM, com possibilidade de override manual do CD.
- Cópia exemplo da planilha utilizada pelos CDs e Account Executive para acompanhamento do planejamento da conta. [Account Planning 2026](https://docs.google.com/spreadsheets/d/1CgMowcPMmobIMNAv2znyppqpPmcW6aJE-tBEECqEpNY/edit?gid=1343155362#gid=1343155362)

---

## Dúvidas, Pendências e Alinhamentos

### Dúvidas em aberto (levar ao stakeholder)

- Issue 1: Por enquanto sem

- Issue 2: qual o formato/nível de detalhe exato que Quadros e Fernando esperam receber de cada report (semanal x mensal), para validar se a estrutura do rascunho atende aos dois?
- Issue 2: como é, na prática, o fluxo manual que o CD segue hoje para gerar cada report — passo a passo de onde ele busca cada informação, em que momento, e como consolida tudo antes de enviar? Ainda não está mapeado; só sabemos quais são as fontes (Salesforce, Bitrix, Gemini, Slack, Drive), não a sequência real de trabalho.

### Pendências a correr atrás

- Issue 1: Por enquanto sem

- Issue 2:
    - Verificar com o time de Operações e Financeiro se é possível liberar acesso aos dados de rentabilidade (GM%) hoje restritos a eles, para preencher o bloco de Profitability sem depender de repasse manual.
    - Confirmar diretamente com Quadros e com Fernando os requisitos de cada um dos dois reports antes de avançar no desenho da solução.
