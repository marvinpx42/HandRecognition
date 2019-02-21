# Visualização com Legos
Visão Computacional voltada para legos e visualização da informação.


## Reconhecimento de mãos
Um processo em três etapas: capturar o frame base, 
detectar a média de cor das mãos e 
reconhecimento se tem mãos ou não na cena

Capturar o frame base - exige interação!!!!!!!
```bash
python recog_utils.py -v "caminho_video"
```

Extrair média de cor - automático
```bash
python handcolorextraction.py -v "caminho_video"
```

Verificar se está funcionando - automático (TODO: verificar se precisa de pausa
```bash
python handdetection.py -v "caminho_video"
```

Atalho para uma execução só:
```bash
VIDEO_PATH=videos/videoTeste2.webm
python recog_utils.py -v VIDEO_PATH && python handcolorextraction.py -v VIDEO_PATH 
&& python handetections.py -v VIDEO_PATH
```

```bash
set VIDEO_PATH=videos\videoTeste2.webm
python recog_utils.py -v %VIDEO_PATH% && python handcolorextraction.py -v %VIDEO_PATH% && python handdetection.py -v %VIDEO_PATH%
```