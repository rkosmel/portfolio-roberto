# Exportar currículo a partir do JSON Resume

Este diretório contém o currículo no padrão **JSON Resume**.

Arquivos:
- `resume.pt.json`
- `resume.en.json`

## Opção 1 — Gerar HTML com jsonresume (CLI)
1) Instale o CLI (requer Node.js):
```bash
npm i -g resume-cli
```

2) Valide o arquivo:
```bash
resume validate resume.pt.json
resume validate resume.en.json
```

3) Exporte para HTML (exemplo com tema "elegant"):
```bash
resume export resume-pt.html --resume resume.pt.json --theme elegant
resume export resume-en.html --resume resume.en.json --theme elegant
```

4) Abra o HTML no navegador e use "Imprimir" → "Salvar como PDF".

## Opção 2 — Manter também uma versão em LaTeX
Se você já tem um template LaTeX bom, dá para manter os dois:
- JSON Resume para versionar e atualizar rápido
- LaTeX para gerar PDF com layout perfeito
