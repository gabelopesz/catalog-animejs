# Coletânea de Animações

Coleção de animações standalone (Bootstrap 5 + anime.js, via CDN) para reaproveitar em outros projetos.
Abra `index.html` para navegar pelo catálogo.

## Estrutura

```
catalog-animejs/
  index.html                              <- catálogo (exemplos agrupados por categoria)
  examples/<nome>/index.html              <- um exemplo autocontido por pasta
  2026-07-23-.../                         <- protótipos originais (CSS puro), mantidos como referência
```

As pastas em `examples/` são planas; as categorias existem no catálogo (`index.html`) e nesta lista.

## Exemplos por categoria

### Logotipos & Marca

| Pasta | O que demonstra |
| --- | --- |
| `logo-reveal` | traçado do contorno + revelação vertical, depois preenchimento |
| `logo-wordmark-build` | abertura do lockup em timeline: símbolo, régua, letras em stagger, brilho e tagline |
| `logo-morph-mark` | loop de morphing do atributo `d` entre formas de mesma estrutura |
| `logo-loader-progress` | um valor de progresso alimenta traçado, preenchimento por `clipPath` e contador |

### Imagens & Galerias

| Pasta | O que demonstra |
| --- | --- |
| `notched-accordion-gallery` | galeria accordion com cantos recortados |
| `tile-mosaic-reveal` | imagem remontada em ladrilhos (stagger em grade) |
| `ken-burns-slideshow` | zoom/panorâmica com crossfade e barra de progresso |
| `flip-lightbox-grid` | miniatura que cresce até o visualizador (FLIP) |
| `slice-slider` | troca de imagens em fatias verticais alternadas |

### Formulários & Interface

| Pasta | O que demonstra |
| --- | --- |
| `snake-highlight-form` | borda SVG que "rasteja" até o campo em foco |

## Convenção de cada exemplo

- Um único arquivo `examples/<nome>/index.html`, autocontido (HTML + CSS + JS inline).
- Bootstrap 5 via CDN para reset/layout/utilitários.
- anime.js via CDN para a animação em si — preferir o padrão "objeto de progresso + `update`"
  (ver `logo-reveal`) quando a interpolação não for uma propriedade CSS simples.
- Para reusar em outro projeto: copie a pasta do exemplo e ajuste os assets/imagens conforme necessário.

## Adicionar um novo exemplo

1. Crie `examples/<nome-do-exemplo>/index.html`.
2. Adicione um card em `index.html` (raiz), na seção da categoria correspondente, e atualize
   a contagem no cabeçalho dela.
3. Registre a pasta na tabela da categoria acima.
