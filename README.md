# CHAMA DeepMap

Gere mapas de profundidade (deep maps) coloridos a partir de qualquer vídeo, direto no navegador.

- Suba um vídeo ou imagem, escolha resolução e fps e clique em **Gerar deep map**.
- Ajuste paleta, intensidade, contraste, anti-flicker e cortes de perto/longe em tempo real.
- Exporte em **MP4**, **PNG** do frame atual ou **sequência PNG (.zip)**.

Tudo roda no seu computador: o vídeo não é enviado para nenhum servidor.

## Como funciona

- Modelo: [Depth Anything V2 Small](https://huggingface.co/onnx-community/depth-anything-v2-small) (ONNX), rodando com [ONNX Runtime Web](https://onnxruntime.ai/) via WebGPU (placa de vídeo) ou WebAssembly (processador).
- O modelo é baixado do Hugging Face na primeira vez e fica guardado no navegador.
- Exportação MP4 com WebCodecs + [mp4-muxer](https://github.com/Vanilagy/mp4-muxer). Funciona no Chrome e no Edge.

## Licenças

O modelo Depth Anything V2 Small é distribuído sob a licença Apache-2.0.

Feito por Guilherme Guisolfi · [@chamadegui](https://instagram.com/chamadegui)
