# LinkedIn

Esta pasta reúne os materiais prontos para atualizar o perfil público.

- Headline: `./headline.md`
- Sobre em português: `./about.pt.md`
- Sobre em inglês: `./about.en.md`
- Capa HTML: `./cover.html`
- Capa PNG pronta: `./assets/linkedin-cover.png`
- Drafts de posts: `./drafts/`

## Capa

A capa foi desenhada em HTML/CSS no tamanho base recomendado pelo LinkedIn: `1584x396`.

O PNG versionado para upload direto fica em `./assets/linkedin-cover.png` e está em 2x (`3168x792`) para melhor nitidez mantendo a mesma proporção.

### Gerar PNG pelo navegador

1. Abra `linkedin/cover.html` no navegador.
2. Use DevTools para simular uma viewport de `1584x396`.
3. Exporte ou tire screenshot em PNG.

### Gerar PNG via linha de comando

```bash
google-chrome --headless=new --disable-gpu --window-size=1584,396 --force-device-scale-factor=2 --screenshot=linkedin-cover.png linkedin/cover.html
```

## Direção de conteúdo

O posicionamento atual é:

- Desenvolvedor Full Stack Júnior.
- TypeScript, React/Next.js, Node.js, PostgreSQL e AWS.
- Produto, requisitos, documentação e backlog.
- IA aplicada como apoio supervisionado ao trabalho.
- Experiência atual na ControlLed descrita em alto nível, sem detalhes internos.
