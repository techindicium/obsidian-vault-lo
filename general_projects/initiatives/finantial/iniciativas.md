# Integração com Área Financeira Global (Ana RER) — Papel FDE

Fonte: transcrição da reunião Pig / Lorena (Vitor Avancini x Lorena Sales Santos)
Link da transcrição: https://docs.google.com/document/d/1DOFG1hOgZs7bFipvuTMFUUecetao_7s_aZNlzrCEep4/edit?tab=t.nseg1fjuv8p8

## Projeto guarda-chuva

**Papel de FDE / Integração com a área financeira global (Ana RER) via plataforma Databricks**

## Frentes de trabalho e itens de ação

### 1. Discovery com a área de negócio (entrevistas)

- [ ] Compartilhar materiais e diagramas de processos do time da Ana (Vitor)
- [ ] Estudar os materiais/diagramas recebidos e pesquisar contexto financeiro para alinhar vocabulário (Lorena)
- [ ] Falar com o par de Global Tech, Nathan, sobre a iniciativa antes de agendar com Ana — Nathan estava de férias; conversa prevista para a semana seguinte (grupo)
- [ ] Definir formato estruturado de entrevista, revisando metodologias já usadas (ex: "4D", skill de PRD) e pesquisando como o formato é feito hoje em dia (grupo)
- [ ] Testar o formato de entrevista com um colega próximo (ex: Jaime) antes de aplicar com a Ana
- [ ] Identificar e conversar com alguém do financeiro interno (Brasil) para ter contexto/vocabulário antes da entrevista com a Ana
- [ ] Identificar o contato ideal no Brasil para tratar do assunto (Vitor descobre e envia o nome)
- [ ] Realizar a entrevista de discovery com a Ana RER (entender gargalos, sem presumir que a solução é um dashboard)

### 2. Prototipagem de soluções

- [ ] Criar protótipos realistas (fake/HTML estático, dashboards com dados fake) com base no que for descoberto na entrevista, para validar com stakeholders antes de avançar para infraestrutura

### 3. Arquitetura e governança da plataforma Databricks

- [ ] Estruturar diagrama de arquitetura/fluxo de dados (unity catalog, separação de catálogos por área)
- [ ] Revisar/organizar roles e grupos de acesso, usando como base o material de governança feito para o Snowflake (~15 páginas — Robson sabe localizar)
- [ ] Ser mais estratégico/intencional na definição de roles e permissões (hoje o sandbox é permissivo demais)
- [ ] Propor framework de governança de uso de IA (guard rails para usuários sem conhecimento técnico)

### 4. Observabilidade / Command Center

- [ ] Avaliar o deploy do "Command Center" (ferramenta do Li) para visibilidade de uso da plataforma
- [ ] Entender quais métricas são úteis e quais descartar, comparando com os dados brutos para checar confiabilidade
- [ ] Conectar esse trabalho com as iniciativas do Daniel (AI Transformation Office)

### 5. Pesquisa sobre skills financeiras da Anthropic

- [ ] Pesquisar o repositório open source da Anthropic com skills sobre mercado/operação financeira
- [ ] Avaliar se o conteúdo se aplica ao contexto de operação financeira interna (não necessariamente mercado financeiro)

### 6. Desenvolvimento pessoal

- [ ] Lorena cursando a certificação Cloud Code Architecture, considerada relevante para o desenvolvimento da plataforma

## Sequência definida ao final da call (iniciar de imediato)

Ordem combinada explicitamente por Vitor e Lorena (~00:35–00:38):

1. Consolidar/definir o formato de entrevista de discovery (base: metodologia "4D", skill de PRD)
2. Testar esse formato com alguém do financeiro interno / colega próximo
3. Realizar a entrevista de discovery com a Ana RER
4. Prototipar soluções fake com base no que for descoberto, para validar com os stakeholders
5. **Só depois disso**: avançar para a frente de arquitetura/governança/roles do Databricks — os dois concordaram em colocar essa frente "em hold" e cogitaram paralelizá-la com outra pessoa enquanto o discovery/prototipagem acontece

Em paralelo:
- [ ] Certificação Cloud Code Architecture (estudo pessoal da Lorena)
- [ ] Pesquisa do repositório open source de skills financeiras da Anthropic

## Itens sem sequência definida (decidir quando/quem)

- [ ] Avaliação do Command Center / observabilidade (deploy, análise de métricas)
- [ ] Conexão com as iniciativas do Daniel (AI Transformation Office)
- [ ] Identificação do contato ideal no Brasil para o assunto financeiro
