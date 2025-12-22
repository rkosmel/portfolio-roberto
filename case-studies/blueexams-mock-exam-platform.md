# Blue Exams — Plataforma de simulados (assinatura)

## Contexto
A Blue Exams precisava de uma plataforma web de simulados em formato de assinatura, com a premissa de replicar a experiência do Executive Assessment (EA) e permitir estudo com feedback e acompanhamento.

## Meu papel
- Construção end-to-end (0→1) da plataforma web (modelagem do domínio e do banco, estrutura de questões, páginas/telas e fluxos principais).
- Implementação de autenticação (NextAuth) e cobrança por assinatura (Stripe).
- Criação e manutenção do conteúdo/banco de questões (11 simulados), com rotinas de inserção e atualização.
- Deploy e operação em produção na AWS (EC2/RDS/S3), além de troubleshooting e correções com foco em estabilidade.

## Stack (alto nível)
- Full-stack: Next.js (App Router), React, TypeScript
- Autenticação: NextAuth
- Pagamentos: Stripe
- Banco de dados: PostgreSQL
- ORM: Prisma
- Infra/Cloud: AWS (EC2, RDS, S3), Nginx

## Arquitetura (alto nível)
- Aplicação full-stack em Next.js, com rotas/handlers no próprio app.
- Persistência em PostgreSQL (RDS) via Prisma.
- Billing e status de assinatura via Stripe.
- Assets (ex.: imagens) em S3 e aplicação servida via Nginx em EC2.

## Principais features
- Banco de questões com 11 simulados completos (IR, Verbal, Quant).
- Experiência “tipo prova”: timer, pausa/retomar, calculadora e navegação consistente.
- Salvamento automático de respostas/progresso (com rastreio de tempo) e retomada de sessão.
- Question Review: comparação de respostas, tempo por questão, filtros e marcação para revisar depois.
- Analytics: percentil, breakdown por seção, comparação com tentativas anteriores e análise de tempo por questão (ex.: Bubble Chart).

## Desafios e decisões
- Construir o produto 0→1, mantendo entregas rápidas sem abrir mão de estabilidade.
- Modelagem de dados e controle de acesso para usuários assinantes.
- UX “tipo prova”: timer, pausa/retomar e salvamento automático para reduzir risco de perda de progresso.
- Correções rápidas em produção e troubleshooting, priorizando impacto no usuário.

## Resultados
- Plataforma funcional no modelo assinatura, com base técnica para evolução contínua (novos simulados, relatórios, melhorias de UX).
- Banco com 11 simulados completos e conteúdos estruturados.
- Recursos de prova: timer, pausa/retomar, calculadora, salvamento automático de respostas e revisão detalhada de questões.
- Dashboard de resultados com percentil, breakdown por seção, comparação com tentativas anteriores e análise de tempo por questão (ex.: Bubble Chart).

## Lições / O que eu melhoraria
- Criar suíte de testes automatizados cobrindo fluxos críticos (auth, assinatura, simulado).
- Observabilidade mais completa (dashboards e alertas) para reduzir tempo de diagnóstico.
