# Checklist de publicação (segurança e privacidade)

Este repositório é um portfólio em formato de **case studies**. O objetivo é demonstrar entregas e decisões técnicas **sem expor código proprietário, credenciais, dados de clientes ou PII**.

## Antes de publicar no GitHub
- Verifique se não há:
  - `.env*`, `*.pem`, `*.key`, dumps (`*.sql`, `*.dump`) ou qualquer token/credencial.
  - URLs internas, endpoints privados, nomes de buckets/hosts internos ou dados de clientes.
- Confira o `.gitignore` (ex.: `.env`, `*.pem`, `*.sql`, `*.dump`, `node_modules/`, builds).

## Ao escrever um case study
- Evite:
  - Senhas, API keys, tokens, headers/payloads reais.
  - Trechos de logs com PII (e-mails, telefones, nomes, IDs reais).
  - Código de projetos privados (prefira pseudocódigo e diagramas).
- Prefira:
  - Arquitetura em alto nível e contexto do problema.
  - Decisões técnicas e trade-offs.
  - Resultados, impactos e aprendizados (quando aplicável).

## Se algo sensível foi exposto
- Considere que apagar o arquivo depois não remove o histórico do Git.
- Rotacione/invalide credenciais imediatamente e faça limpeza do histórico quando necessário.
