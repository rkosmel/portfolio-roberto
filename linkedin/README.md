# Como gerar a imagem da capa do LinkedIn em alta resolução

## Método 1: Print via navegador (recomendado)
1. Abra `linkedin/cover.html` no navegador
2. Use atalho de print:
   - **Windows/Linux**: `Ctrl + Shift + I` → DevTools → Toggle device toolbar → 1584×396 → Print → Save as PDF → Exportar como PNG
   - **Mac**: `Cmd + Shift + I` → DevTools → Toggle device toolbar → 1584×396 → Print → Save as PDF → Exportar como PNG

## Método 2: Screenshot via linha de comando (Linux)
```bash
# Instalar se necessário
sudo apt install chromium-browser

# Gerar PNG em 1584x396
chromium-browser --headless --disable-gpu --window-size=1584,396 --screenshot=linkedin-cover.png linkedin/cover.html
```

## Método 3: Ferramenta online
- Suba o HTML para um serviço como CodePen ou JSFiddle
- Use a função de exportação de imagem ou print do navegador

## Dicas de qualidade
- Use zoom 100% no navegador
- Exporte em PNG (não JPG)
- Verifique se o arquivo tem exatamente 1584×396 pixels
- Se necessário, redimensione com ferramenta como GIMP/Photoshop mantendo a proporção
