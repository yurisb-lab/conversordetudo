# Registro de construção — Conversor de Tudo

App em um único `index.html` (HTML + CSS + JS puro). Tudo roda no navegador; bibliotecas vêm do jsDelivr com versão fixa e só são baixadas quando a ferramenta é usada.

| Tela | Data | Status | O que falta | Mais difícil que o esperado |
|---|---|---|---|---|
| S01 Início (busca, categorias, favoritas) | 2026-10-31 | pronto | — | — |
| S02 Ferramenta: envio → opções → processando → resultado/erro | 2026-10-31 | pronto | — | reenviar o mesmo arquivo não disparava o evento (corrigido) |
| S03 Editor de miniaturas (Organizar) | 2026-10-31 | pronto | — | — |
| S04 Editor de página: colocar itens (Assinar, Editar) | 2026-10-31 | pronto | arrastar item entre páginas | posicionar em páginas giradas (resolvido com as coordenadas do pdf.js) |
| S05 Editor de página: áreas (Tarjar, Recortar) | 2026-10-31 | pronto | — | tarja automática em página girada (resolvido calculando os 4 cantos) |
| S06 Histórico | 2026-10-31 | pronto | — | — |
| S07 Como funciona / privacidade | 2026-10-31 | pronto | — | — |
| S08 Paleta de busca (Ctrl+K) | 2026-10-31 | pronto | — | — |

## Testes feitos (Chromium, 1280/1440 px e 390 px)
- 60 ferramentas executadas de ponta a ponta com arquivos reais; vídeos/áudios conferidos com ffprobe, PDFs com pdf-lib e renderização em imagem.
- Sem erros no console; sem rolagem horizontal em 390 px; tema claro e escuro.

## Limitações conhecidas
- PowerPoint → PDF, PDF/A e Traduzir não existem (não dá para fazer bem só no navegador).
- Word/Excel/HTML → PDF geram páginas como imagem (texto não selecionável).
- Vídeos muito grandes (>1–2 GB) podem estourar a memória do navegador (motor single-thread, compatível com GitHub Pages).
