# Blue Exams — Plataforma de simulados (assinatura)

## Contexto
A Blue Exams precisava de uma plataforma web de simulados em formato de assinatura, com a premissa de replicar a experiência do Executive Assessment (EA) e permitir estudo com feedback e acompanhamento.

## Meu papel
- Desenvolvimento e manutenção da plataforma web (entrega orientada a resultado e estabilidade).
- Integrações essenciais de produto (autenticação, pagamentos/assinatura e persistência em banco).
- Suporte a deploy, troubleshooting e correções em produção.

## Stack (alto nível)
- Front-end: Next.js (App Router), React
- Autenticação: NextAuth
- Pagamentos: Stripe
- Banco de dados: PostgreSQL
- ORM: Prisma

## Arquitetura (alto nível)
- Aplicação full-stack em Next.js, com rotas/handlers no próprio app.
- Persistência em PostgreSQL via Prisma.
- Billing e status de assinatura via Stripe.

## Desafios e decisões
- Modelagem de dados e controle de acesso para usuários assinantes.
- Estabilidade e correções rápidas em produção, priorizando impacto no usuário.
- Balancear velocidade de entrega com qualidade (evitando regressões e mantendo comportamento consistente).

## Resultados
- Plataforma funcional no modelo assinatura.
- Implementação de base técnica para evolução contínua (novos simulados, relatórios, melhorias de UX).

## Lições / O que eu melhoraria
- Criar suíte de testes automatizados cobrindo fluxos críticos (auth, assinatura, simulado).
- Observabilidade mais completa (dashboards e alertas) para reduzir tempo de diagnóstico.
