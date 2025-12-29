# The Mindville — Plataforma de engajamento (B2B)

## Contexto
A The Mindville desenvolve uma plataforma B2B para empresas acompanharem engajamento de usuários/alunos, com dashboard e backend orientado a métricas.

## Meu papel
- Contribuições full-stack no produto existente.
- Participação em features e manutenção envolvendo autenticação/login e integrações com backend.
- Apoio em banco de dados e rotinas de debug (PostgreSQL).

## Stack (alto nível)
- Front-end: Next.js (monorepo com npm workspaces)
- Back-end: Node.js
- Banco de dados: PostgreSQL
- ORM: Prisma

## Arquitetura (alto nível)
- Front-end em monorepo com dois apps (produção e demo), compartilhando pacotes de core e UI.
- API REST em Node.js com documentação via Swagger.
- Camadas de dados (Bronze/Silver/Gold) para pipeline de métricas e snapshots.

## Desafios e decisões
- Evoluir um produto já existente sem quebrar fluxos críticos.
- Trabalhar com multi-tenancy e segurança de endpoints (ex.: chaves por tenant / JWT).

## Resultados
- Entregas incrementais e manutenção de estabilidade.
- Apoio em troubleshooting e evolução de funcionalidades no backend e no dashboard.

## Lições / O que eu melhoraria
- Criar mais documentação de arquitetura para onboarding.
- Aumentar cobertura de testes nos fluxos mais sensíveis (auth e regras de acesso).
