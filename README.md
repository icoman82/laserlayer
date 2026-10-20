# Laserlayer

**https://laserlayer.icoman.com.br**

Web app que transforma um STL em peças planas para montar, no estilo dos troféus de parede em MDF:

- **Corte a laser (MDF)**: **egg crate** (fatias que se cruzam com encaixes, monta sem cola) ou **empilhado** (camadas coladas, com guia de alinhamento gravada). Exporta **SVG** e **DXF**, uma chapa por arquivo (vermelho/CORTE = corte, azul/GRAVACAO = gravação).
- **Impressora 3D (FDM)**: só egg crate, peças de 2–3 mm com folga de impressão. Lista de impressoras conhecidas (Bambu, Prusa, Creality, Elegoo, Anycubic, Voron) ou mesa personalizada. Exporta **3MF** (uma mesa por arquivo, cada peça como objeto nomeado) e **STL**.

Outros recursos:

- **Exemplos prontos**, modelados em código: lobo-guará, onça-pintada, capivara, tamanduá-bandeira, veado-campeiro, unicórnio, dragão oriental, dragão alado e tiranossauro rex.
- **Simplificação low-poly** ao carregar o STL (meshoptimizer), para peças com contornos retos.
- **Placa de parede**: escudo clássico, brasão, oval, retângulo, hexágono ou um **SVG** próprio (formas internas viram furos). Pode ter de 1 a 5 camadas em degraus, cada uma menor que a de trás, e borda gravada (linha simples, dupla, tracejada, pontilhada, ondas ou zigue-zague). Uma **base sólida** com o contorno das costas do modelo encaixa num rebaixo da placa, e as espinhas ganham abas que atravessam base e placa até a parede.
- **Partes soltas**: mapa de ligações entre as peças, pontes automáticas e um botão que testa mais espinhas e costelas até tudo ficar conectado.
- **Modo vitrine**: textura de MDF, bordas queimadas pelo laser, sombra na parede e exportação em PNG.
- **Janela de prévia** no canto, que troca de lugar com a vista principal.

Tudo roda no navegador. O STL é lido do computador da pessoa e nunca é enviado a nenhum servidor.

## Como usar localmente

Abra `index.html` no navegador (precisa de internet para carregar three.js, Clipper, JSZip, meshoptimizer e as fontes via CDN).

## Publicação

O site é publicado pelo GitHub Pages a partir da branch `main`. O arquivo `CNAME` aponta para o domínio `laserlayer.icoman.com.br`.
