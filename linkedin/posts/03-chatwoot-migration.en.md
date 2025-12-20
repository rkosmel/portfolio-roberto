Not every project is about new features — some of the most valuable learning comes from infrastructure and operations.

In one of my recent projects, I supported a **Chatwoot** setup on AWS and helped plan a low-risk data migration.

High-level highlights:
- Workloads running on **Docker Compose** on an **EC2** instance
- Database on **AWS RDS (PostgreSQL)** and assets on **S3**
- Migration plan with clear steps:
  - `pg_dump` / `pg_restore` with a short maintenance window
  - post-restore validation
  - S3 assets sync
  - rollback strategy

Stack:
- AWS (EC2, RDS, S3)
- Docker / Linux
- PostgreSQL

For confidentiality, I don’t share endpoints/credentials or internal details — but I’m happy to discuss the approach.

#aws #docker #postgresql #devops #cloud
