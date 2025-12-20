# MBA No Brainer — Chatwoot em AWS (EC2 + RDS + S3)

## Contexto
A MBA No Brainer precisava de uma solução de atendimento (Chatwoot) operando em cloud, com banco e storage gerenciados, e um plano seguro para migração de dados entre ambientes.

## Meu papel
- Provisionamento e operação da aplicação em AWS.
- Setup via Docker Compose (app, workers, redis), e integração com serviços gerenciados.
- Planejamento de migração de dados (Postgres e assets), com validações e estratégia de rollback.

## Stack (alto nível)
- App: Chatwoot (Rails)
- Infra/execução: AWS EC2 + Docker Compose
- Banco: PostgreSQL em AWS RDS
- Arquivos: AWS S3

## Arquitetura (alto nível)
- Workloads em containers na EC2.
- Banco e storage fora da instância (RDS/S3) para durabilidade e separação de responsabilidades.

## Desafios e decisões
- Definir processo de migração com risco controlado (janela de manutenção curta).
- Planejar rollback e validações para evitar perda de dados.
- Considerar limitações de conectividade/rede entre ambientes ao definir onde executar dump/restore.

## Resultados
- Ambiente novo preparado e operável.
- Runbook de migração com passos claros e verificações (dump/restore e sync de assets).

## Lições / O que eu melhoraria
- Automatizar runbooks com scripts idempotentes.
- Padronizar observabilidade (logs e métricas) para reduzir tempo de diagnóstico.
