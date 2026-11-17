# Manual de Estilo — Fase 1 (referência analisada)

Fonte: reel de referência baixado e medido com ffmpeg/OpenCV/librosa. Itens marcados [não medido] exigem escuta ou transcrição e ficam para a próxima rodada.

## 1. Formato
- Vertical 9:16, 1080x1920, 30 fps, vídeo VP9 + áudio AAC.
- Duração 12min43s (763 s). Não é um reel curto: serve bem como modelo de densidade para vídeo longo.

## 2. Cortes
- 95 cortes duros detectados (scene > 0,25) = 7,5 por minuto. Plano médio 7,9 s, mediana 5,8 s.
- Cortes por minuto ao longo do vídeo: 10, 10, 9, 9, 8, 7, 8, 6, 7, 4, 8, 6, 4. A densidade é maior na abertura e cai até o fim.
- Tipo: corte seco. Só 1 evento com mais de um quadro de transição (aprox. 4 quadros, em 10:35). Não há dissolve recorrente.
- Planos longos sem corte (> 20 s): 6 trechos (20 s, 22 s, 22 s, 25 s, 28 s e 47 s). O motivo de cada um [não verificado]; precisa de transcrição para ligar ao conteúdo.
- O que é removido (pausas, "é...", repetições) e quanto silêncio sobra entre frases: [não medido]. Há cama de música contínua, então não existe silêncio absoluto; a medição fina exige separar a voz.

## 3. Zoom / enquadramento
- Fala em primeiro plano com mudança abrupta de escala entre planos (jump cut com punch-in): 104 mudanças de área do rosto/pele maior que 25% (aprox. 12% linear), ou 8 por minuto. As razões típicas de área ficam em 1,3x a 2,4x, o que corresponde a um punch-in de ~15% a ~55% linear.
- Zoom lento nos B-rolls: presente visualmente; magnitude [não medida com confiança].

## 4. Transições e efeitos
- Fala -> B-roll e B-roll -> fala: corte seco.
- Texto entra com fade curto e leve subida (aparente). Duração exata [não medida].
- Clipe de transição estilizado (flash, whip, glitch): não detectado.

## 5. B-roll
- Presente, aprox. 44% do tempo. 76 inserções (>= 1 s) = 6 por minuto. Mediana 3,5 s, média 4,4 s, máximo 20 s.
- Estilo: cenas cinematográficas verticais, escuras, baixa chave, tons azul/ciano com acento quente (aeroporto, servidor, globo, mãos, moedas, cruz, montanha). Parece material gerado ou de banco cinematográfico; a origem [não determinada].
- Quase todo B-roll tem um cartão de texto (dado ou versículo) sobre ele.

## 6. Legenda (na fala)
- Fonte mais parecida: Montserrat Bold/ExtraBold, caixa alta.
- Branco quente (~#F2E7DF) com destaque em laranja (#E5A05C) na palavra-chave ou meia frase.
- Posição: bloco entre 67% e 71% da altura, centralizado, ocupando ~69% da largura.
- Duas linhas, cerca de 3 a 5 palavras por linha. A frase aparece inteira de uma vez, não palavra por palavra.
- Sem caixa nem contorno; legibilidade vem de um degradê escuro suave na parte inferior do quadro.
- Não é transcrição literal: são frases-chave resumidas.

## 7. Textos na tela
- Cartão de dado: número grande em branco + linha pequena em caixa alta embaixo ("74 países / MAIS DE UM DIA FORA DO AR"). Linha curta de fonte acima quando cabe ("TESOURO NACIONAL").
- Cartão de versículo/citação: texto em caixa alta com destaque laranja e referência em laranja pequena abaixo ("LUCAS 21:28"), sobre B-roll escurecido.
- Sem logo, sem marca d'água fixa.

## 8. Cor
- Look quente e escuro. Pretos esmagados (percentil 1 da luma ~5), brilhos sem estourar (percentil 99 ~202). Saturação média (S ~88/255). B-roll em baixa chave (luma média ~74).
- Pele e fundo verde/madeira da fala com contraste moderado; B-roll frio com acento laranja.

## 9. Trilha sonora
- Cama de música contínua: nenhum silêncio abaixo de -35 dB no vídeo inteiro.
- Nível da cama cresce ao longo do vídeo: piso de ~-35 dBFS no minuto 0 até ~-26 dBFS do minuto 6 em diante; a voz sobe junto (de ~-21 a ~-11 dBFS). É uma construção gradual, não uma cama fixa.
- Distância voz x cama (aproximação pelo pico de voz menos o piso): ~12 a 16 dB, estável.
- Andamento estimado 110 a 130 BPM, medida instável (a fala contamina). Gênero, instrumentação, trocas de música e efeitos sonoros: [não medidos; exigem escuta].
- Ducking: como a distância voz x cama é estável, a música deve estar abaixando sob a fala; confirmação [pendente].

## 10. Áudio da voz
- Loudness final integrado -14,3 LUFS, pico real +0,3 dBTP, faixa dinâmica (LRA) 10,1 LU. Pico acima de 0 dBFS: pequeno clip possível; na nossa entrega vamos manter em -1 dBTP.
- Limpeza e compressão da voz: [não medido].

## 11. Abertura e final
- Abertura: fala direta já no quadro 0, com o texto-gancho "SERÁ QUE A GENTE TÁ PERTO DO FIM?" (pergunta) sobre o rosto; corta para B-roll aos 5 s.
- Final: sequência de versículos sobre cruz e montanha, volta ao rosto para fechamento. Texto exato [não transcrito].

## Tabela REGRA -> MEDIDA POR MINUTO
| Regra | Medida |
|---|---|
| Cortes duros | ~7,5 por min (10 na abertura, 4 a 6 no final) |
| Plano médio / mediana | 7,9 s / 5,8 s |
| Mudanças de escala (punch-in em jump cut) | ~8 por min, +15% a +55% linear |
| B-roll | 6 inserções por min, mediana 3,5 s, ~44% do tempo |
| Planos longos sem corte | 6 no vídeo, de 20 a 47 s |
| Transições | corte seco; efeito pontual raro |
| Legenda | caixa alta, 2 linhas, 69% da largura, entre 67 e 71% da altura |
| Destaque | laranja #E5A05C em 1 palavra-chave ou meia frase |
| Cartões de texto | dado ou versículo sobre B-roll, em quase todo B-roll |
| Música | cama contínua, crescente de -35 a -26 dBFS |
| Voz x música | ~12 a 16 dB de diferença |
| Loudness final | -14 LUFS integrado |
