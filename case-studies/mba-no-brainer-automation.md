# MBA No Brainer — Sistema de Automação de Ranking

## Contexto
Durante meu estágio na MBA No Brainer, fui responsável por desenvolver e manter um sistema completo de automação para o ranking de gamificação da plataforma. O objetivo era computar automaticamente pontos dos alunos com base em diversas atividades e desafios, criando um ambiente competitivo e engajador.

## Desafio
O sistema de ranking da MBA No Brainer precisava computar pontos de múltiplas fontes:
- Desafios diários completados
- Tarefas entregues nos prazos
- Participação em estudos em grupo
- Interações com a plataforma
- Conquistas e badges

O processo manual era demorado, propenso a erros e não escalável para o crescimento da base de alunos.

## Minha Contribuição

### Automação com Zapier
Desenvolvi múltiplas automações complexas no Zapier:

**Arquitetura de Workflows:**
- **Multi-step workflows**: Sequências de 10+ passos com lógica condicional
- **Branching logic**: Ramificações baseadas em tipo de atividade e perfil do aluno
- **AI agents**: Integração com agentes de IA para análise qualitativa de participações
- **Error handling**: Tratamento robusto de falhas e retry automático
- **Rate limiting**: Controle de volume para não sobrecarregar APIs

**Workflows Principais:**
1. **Daily Challenge Processing**: Monitoramento de conclusões de desafios diários e cálculo automático de pontos com base na dificuldade e tipo de desafio.
2. **Group Study Analytics**: Análise de participações em estudos em grupo e atribuição de pontos colaborativos baseados no tamanho do grupo e nível de engajamento.

### Automação com AWS Lambda
Para maior escalabilidade e controle, implementei um sistema complementar em AWS:

**Arquitetura Serverless:**
- **AWS SQS**: Filas para processamento assíncrono de eventos
- **AWS Lambda**: Funções serverless para computação de pontos
- **PostgreSQL RDS**: Banco de dados relacional para ranking
- **CloudWatch**: Monitoramento e logging das automações

**Processo:**
1. Eventos da plataforma são publicados em filas SQS
2. Lambda functions processam eventos em paralelo
3. Regras de negócio aplicadas para cálculo de pontos
4. Resultados persistidos em PostgreSQL RDS
5. Dashboard atualizado em tempo real

## Tecnologias Utilizadas

### Zapier
- **Advanced Workflows**: Multi-step com branching e conditional logic
- **AI Integration**: OpenAI e Claude para análise de conteúdo
- **API Integrations**: REST APIs, webhooks, database connections
- **Error Handling**: Retry mechanisms e fallback strategies

### AWS
- **AWS Lambda**: Python para funções serverless
- **AWS SQS**: Message queues para processamento assíncrono
- **PostgreSQL RDS**: Banco de dados relacional para ranking
- **AWS CloudWatch**: Monitoramento e alerting

### Monitoramento e Debugging
- **Logging**: Registro detalhado de todas as execuções
- **Alerting**: Notificações automáticas para falhas
- **Performance Tracking**: Métricas de tempo de processamento
- **Data Validation**: Verificação de consistência dos pontos

## Resultados
- Sistema de automação funcional processando múltiplos tipos de atividades e desafios dos alunos.
- Redução significativa no tempo manual de processamento do ranking.
- Integração bem-sucedida entre Zapier (workflows) e AWS (serverless).
- Ranking atualizado em tempo real com zero erros manuais.

## Lição / O que eu melhoraria
- Implementar testes automatizados para validar todas as regras de negócio do ranking.
- Criar dashboard de monitoramento específico para as automações.
- Documentar mais detalhadamente os workflows para facilitar manutenção.
