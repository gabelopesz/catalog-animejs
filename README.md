# Coletânea de Animações

Coleção de animações standalone (Bootstrap 5 + anime.js, via CDN) para reaproveitar em outros projetos.
Abra `index.html` para navegar pelo catálogo.

## Estrutura

```
sync-animate/
  index.html                              <- catálogo (lista todos os exemplos)
  examples/
    logo-reveal/
      index.html                          <- traçado de logo + revelação
    notched-accordion-gallery/
      index.html                          <- galeria accordion com cantos recortados
    snake-highlight-form/
      index.html                          <- borda SVG que "rasteja" até o campo em foco
    tile-mosaic-reveal/
      index.html                          <- imagem remontada em ladrilhos (stagger em grade)
    ken-burns-slideshow/
      index.html                          <- zoom/panorâmica com crossfade e barra de progresso
    flip-lightbox-grid/
      index.html                          <- miniatura que cresce até o visualizador (FLIP)
    slice-slider/
      index.html                          <- troca de imagens em fatias verticais alternadas
  2026-07-23-.../                         <- protótipos originais (CSS puro), mantidos como referência
```

## Convenção de cada exemplo

- Um único arquivo `examples/<nome>/index.html`, autocontido (HTML + CSS + JS inline).
- Bootstrap 5 via CDN para reset/layout/utilitários.
- anime.js via CDN para a animação em si — preferir o padrão "objeto de progresso + `update`"
  (ver `logo-reveal`) quando a interpolação não for uma propriedade CSS simples.
- Para reusar em outro projeto: copie a pasta do exemplo e ajuste os assets/imagens conforme necessário.

## Adicionar um novo exemplo

1. Crie `examples/<nome-do-exemplo>/index.html`.
2. Adicione um card em `index.html` (raiz) apontando para o novo arquivo.
