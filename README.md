# colab-
O código apresentado é um exemplo de processamento básico de imagens utilizando a biblioteca OpenCV em Python. 
No geral, esse código é um exemplo básico de processamento de imagens com o OpenCV, 
demonstrando algumas operações comuns como conversão para escala de cinza, negativo, ajuste de contraste e brilho, e suavização.

Primeiramente, as bibliotecas necessárias são importadas, incluindo cv2 para a manipulação de imagens
numpy para operações numéricas e matplotlib.pyplot para exibição de gráficos. 
Em seguida, é importada a biblioteca cv2_imshow do Google Colab para exibir as imagens.

O código começa abrindo a imagem "t1.jpg" utilizando cv2.imread('/t1.jpg', 1). 
O valor 1 indica que a imagem será lida em cores. A função cv2_imshow é utilizada para exibir a imagem no Google Colab.

Em seguida, é aplicada a conversão ponderada para escala de cinza. 
Os canais de cores (B, G, R) são separados utilizando cv2.split(img), e então é feito um cálculo ponderado para obter a imagem em escala de cinza.

O código também demonstra como obter o negativo da imagem. 
A imagem original é lida em cores ou escala de cinza, dependendo do valor da variável colorida. 
Em seguida, a operação de negativo é realizada através de 255 - img_in.

Em seguida, é aplicado um ajuste de contraste e brilho na imagem em escala de cinza. 
Os valores de a e b podem ser ajustados para controlar o contraste e brilho da imagem. 
A imagem de entrada é multiplicada por a e somada a b, resultando na imagem de saída.

Por fim, é aplicada uma suavização à imagem utilizando um kernel de média. 
O kernel é definido como uma matriz 5x5 com valores iguais a 1/25. 
A função cv2.filter2D é utilizada para aplicar o filtro à imagem de entrada, resultando na imagem suavizada. 

