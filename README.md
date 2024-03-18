# Transformando Imagens em Objeto 3D com Python
Este código em Python utiliza as bibliotecas NumPy, OpenCV (cv2) e Mayavi para carregar uma imagem, convertê-la em tons de cinza, e depois visualizá-la em um gráfico 3D.

Aqui está uma descrição linha por linha:
- import numpy as np: Importa a biblioteca NumPy e a renomeia como np.
- import cv2: Importa a biblioteca OpenCV para manipulação de imagens.
- from mayavi import mlab: Importa o módulo mlab da biblioteca Mayavi para visualização em 3D.

A partir daqui, o código realiza as seguintes operações:
- Carrega uma imagem no formato PNG usando a função cv2.imread() e armazena-a na variável imagem_png.
- Converte a imagem para tons de cinza usando cv2.cvtColor(), armazenando-a na variável imagem_cinza.
- Obtém as dimensões da imagem (altura e largura).
- Cria um grid 2D para os pontos da imagem usando np.meshgrid().
- Converte as coordenadas x, y e os valores dos pixels em arrays 1D usando ravel().
- Define os valores z como zeros, já que estamos lidando com uma imagem 2D.
- Armazena as intensidades dos pixels em um array 1D.

A partir da linha 14, a biblioteca Mayavi é utilizada para a visualização 3D:
- Inicia uma nova figura 3D com um fundo branco usando mlab.figure().
- Plota os pontos 3D da imagem usando mlab.points3d(). Os argumentos passados são as coordenadas x, y e z dos pontos, bem como as intensidades dos pixels. O modo de exibição é configurado como 'cube' e o modo de escala como 'none', o que significa que cada ponto é representado como um cubo e sua escala não é alterada.
- Exibe a figura usando mlab.show().

Essencialmente, este código carrega uma imagem, converte-a para tons de cinza e, em seguida, exibe-a como uma representação 3D onde a altura dos pontos é determinada pela intensidade dos pixels na imagem original.

## Rodando projeto

Clone o projeto

```bash
  git clone https://github.com/python-brasil/Transformando-Imagens-em-Objeto-3D-com-Python.git
```
Recomandamos criar uma venv antes de instalar as dependências
```bash
  python -m venv venv
```
em Linux
```bash
  python3 -m venv venv
```
Instale as dependências

```bash
  pip install -r requirements.txt
```

em Linux

```bash
  pip3 install -r requirements.txt
```
## Screenshot

![Transformando Imagens em Objeto 3D com Python](https://github.com/python-brasil/Transformando-Imagens-em-Objeto-3D-com-Python/assets/126124866/742a847d-891d-4590-9cdc-186c36f5bb2c)


## Infos de commits

- :package: novas funcionalidades
- :up: atualizações
- :ant: correções de bug
- :checkered_flag: release


## Nos acompanhe nas redes

- Instagram - [@python_brasil](https://www.instagram.com/python_brasil/)
- LinkedIn - [Comunidade Python Brasil](https://www.linkedin.com/company/comunidade-python-brasil)
- GitHub - [python-brasil](https://github.com/python-brasil)
- YouTube - [@Python_Brasil](https://www.youtube.com/@Python_Brasil)
- Pinterest - [Python Brasil](https://br.pinterest.com/pythonbrasil/)
- TikTok - [@python_brasil](https://www.tiktok.com/@python_brasil)

