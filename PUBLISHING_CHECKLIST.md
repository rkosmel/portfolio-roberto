# Checklist de publicação (modo seguro)

Este repositório é um portfólio em formato de **case studies**. A ideia é mostrar resultados e capacidade técnica **sem publicar código proprietário, credenciais ou dados sensíveis**.

## Antes de publicar no GitHub
- Verifique se não há:
  - `.env`, `.pem`, dumps (`*.sql`, `*.dump`), credenciais, tokens.
  - URLs internas, endpoints privados ou dados de clientes.
- Confira o `.gitignore` (já inclui `.env`, `*.pem`, `*.sql`, `*.dump`).

## Ao escrever um case study
- Evite:
  - Senhas, API keys, nomes de secrets.
  - Trechos de logs com PII.
  - Identificadores internos (ex.: IDs reais de usuários/clientes).
- Prefira:
  - Arquitetura em alto nível.
  - Decisões técnicas e trade-offs.
  - Resultados e aprendizados.

## Se você ainda tem arquivos antigos localmente
- Mantenha fora do portfólio e fora de qualquer repo público.
- Se houver qualquer suspeita de credenciais expostas, rotacione/invalidade (quando aplicável).
