# GitHub — passos para publicar o portfólio

## 1) Decisão rápida (privacidade)
Se este repositório for **público**, seu e-mail (e possivelmente telefone, se você mantiver no JSON) ficam expostos.

Sugestão:
- Manter **e-mail** público.
- Avaliar se quer manter **telefone** público (opcional).

## 2) Criar repositório no GitHub
1) Acesse: https://github.com/new
2) Owner: `rkosmel`
3) Repository name: `portfolio-roberto`
4) Visibility: `Public`
5) **Não** marque para criar README (já existe localmente)
6) Create repository

## 3) Publicar (push) a pasta local
Abra um terminal e rode estes comandos dentro de `Documentos/portfolio-roberto`:

```bash
git init
git add .
git commit -m "chore(portfolio): initial case studies and resume"
git branch -M main
git remote add origin https://github.com/rkosmel/portfolio-roberto.git
git push -u origin main
```

## 4) Fixar (pin) no perfil
No GitHub:
- Vá em seu perfil → "Customize your pins" → fixe `portfolio-roberto`.

## 5) (Opcional) Criar README de perfil
O GitHub mostra um README especial quando você cria um repo com o **mesmo nome do seu usuário**.

- Crie um repo chamado `rkosmel`.
- Adicione um `README.md` nele.
- Você pode usar o template em `./github/profile-README.md`.
