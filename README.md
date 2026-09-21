# Estúdio Aspas SIC TV Record

Monta o card de citação do debate da SIC TV | Record sobre foto: cole o
texto, escolha branco ou escuro, envie a foto e baixe o PNG.

Irmão do Estúdio Aspas Rondoniaovivotv, com o layout invertido: texto em
cima, cabeçalho (perfil + "DEBATE / SIC TV | RECORD") embaixo, barra de cores
deitada no rodapé e o bico de balão saindo do canto de cima à esquerda.

```bash
py -3 servidor.py        # http://localhost:8796
```

## Medidas

Vêm do Figma "DA Mídia — MR 2026", página "silas - edição", os dois
TWEET-DEBATE-SIC-TV (2476:744 branco, 2476:766 escuro), cada um num grupo com
o triângulo "Polygon 5". Estão em auto-layout: Conteúdo com padding
36 / 67 / 45 / 72 e gap 32; o card de 808 cresce para baixo e a barra (22 de
altura, absoluta) fica presa ao rodapé.

O bico usa os vértices medidos no Figma: (0, 46,5), (0, −26,25), (63,01, 10,12)
no espaço do card. Ele entra no mesmo caminho do card para a sombra sair uma
só.

O card fica em Work Sans com entreletra de −4% no texto: sem isso a quebra de
linha sai diferente do Figma.

## Autossuficiente

Nenhuma chamada externa. Fontes do card e foto de perfil em base64 no
`index.html`; a Encode Sans da interface vem de `ativos/fontes/`.
