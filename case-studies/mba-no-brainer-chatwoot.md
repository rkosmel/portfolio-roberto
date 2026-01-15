# MBA No Brainer — Chatwoot em AWS com Integração WhatsApp

## Contexto
A MBA No Brainer precisava implementar um sistema de atendimento ao cliente via WhatsApp para melhorar a comunicação com alunos e professores. Como a empresa já utilizava AWS, a solução deveria ser integrada à infraestrutura existente.

## Meu papel
- **Pesquisa e seleção**: Realizei análise de ferramentas open source e escolhi o Chatwoot como melhor solução
- **Arquitetura completa**: Design e implementação da infraestrutura em AWS
- **Instalação e configuração**: Setup do Chatwoot via Docker com PostgreSQL e S3
- **Integração WhatsApp**: Configuração completa com Twilio para WhatsApp Business
- **Gestão de usuários**: Setup de acessos para professores da MBA No Brainer

## Stack (completa)
- **App**: Chatwoot (Rails) - Software open source de atendimento
- **Infra**: AWS EC2 + Docker Compose
- **Banco**: PostgreSQL em AWS RDS
- **Storage**: AWS S3 para arquivos
- **WhatsApp**: Twilio API para integração Business
- **Deploy**: Docker containers em produção

## Arquitetura
- Containers Docker na EC2 (app, workers, redis)
- PostgreSQL RDS separado da instância principal
- S3 para armazenamento de arquivos e mídias
- Twilio como intermediário para WhatsApp Business
- URL padronizada para acesso dos professores

## Desafios e decisões
- **Escolha da ferramenta**: Análise comparativa entre opções open source
- **Integração WhatsApp**: Configuração complexa com Twilio API
- **Segurança**: Setup de acessos restritos para professores
- **Performance**: Otimização de containers e banco de dados

## Resultados
- **Sistema 100% funcional**: Chatwoot operando em produção
- **WhatsApp integrado**: Professores atendendo via WhatsApp Business
- **Acesso simplificado**: URL única e credenciais organizadas
- **Escalabilidade**: Infraestrutura pronta para crescimento
- **Custo-benefício**: Solução open source vs alternativas pagas

## Lições e melhorias
- **Automação**: Scripts para deploy e manutenção
- **Monitoramento**: Logs e métricas para operação
- **Backup**: Estratégia robusta de recuperação
- **Documentação**: Runbooks detalhados para equipe
