# Blue Exams — Landing page (site institucional)

## Contexto
A Blue Exams precisava de uma landing page profissional para apresentar o produto, comunicar proposta de valor e capturar interesse (SEO básico e navegação rápida).

## Meu papel
- Concepção e implementação da landing page.
- Ajustes de UX/UI, performance e SEO básico.
- Deploy e operação do site em produção.

## Stack
- Front-end: HTML, CSS, JavaScript (vanilla)
- Infra/Cloud: AWS EC2, Nginx, TLS/SSL (Let's Encrypt)

## Arquitetura (alto nível)
- Site estático servido via Nginx.
- Certificados TLS via Let's Encrypt.

## Desafios e decisões
- Manter o site leve e rápido (sem framework) para reduzir complexidade e facilitar deploy.
- Estruturação de arquivos (assets, favicons, sitemap, robots) para compatibilidade e SEO básico.

## Resultados
- Site publicado em produção e mantido com deploy simples.
- Base sólida para evoluir conteúdo e campanhas sem depender de backend.

## Lições / O que eu melhoraria
- Automatizar deploy (CI/CD) com validações e rollback.
- Medir melhor métricas (Core Web Vitals) e funil (analytics) com rastreamento padronizado.
