Nem todo projeto é "só feature" — algumas das experiências mais valiosas que tive foram de infra/ops.

Em um dos trabalhos, participei do setup e operação do **Chatwoot** em AWS e do planejamento de migração de dados, com foco em risco baixo.

Pontos principais (alto nível):
- Workloads rodando em **Docker Compose** numa **EC2**
- Banco em **AWS RDS (PostgreSQL)** e arquivos em **S3**
- Planejamento de migração com passos claros:
  - `pg_dump` / `pg_restore` com janela de manutenção
  - validações pós-restore
  - sync de assets no S3
  - estratégia de rollback

Stack:
- AWS (EC2, RDS, S3)
- Docker / Linux
- PostgreSQL

Por confidencialidade, não compartilho endpoints/credenciais nem detalhes internos, mas esse tipo de runbook me deu muita base pra Cloud/DevOps.
