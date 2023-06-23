# Trabalho-M3

## Código

Inicialmente, importamos as bibliotecas OpenCV e NumPy para o programa. Em seguida, adicionamos a função 'cv2_imshow' de google.colab.patches, 
para melhorar a exibição das imagens. Na seguinte célula, carregamos a imagem 'j.png' usando a função 'cv2.imread'. Então fazemos o processo de 
conversão da imagem para tons de cinza. Por fim, a imagem resultante é armazenada na variável 'img'. O mesmo processo é repetido na linha 
seguinte, onde a imagem 'j_ruido.png' é carregada com a função 'cv2.imread', convertida para tons de cinza e armazenada na variável 'img_opening'. 
Finalmente carregamos a última imagem, 'j_furos.png', usando a função 'cv2.imread', realizamos a conversão para tons de cinza e a atribuímos à 
variável 'img_closing'.
Acessamos a forma da imagem com 'img.shape', que retorna uma tupla contendo a altura e a largura da imagem. Na linha seguinte criamos uma matriz 
5x5 preenchida com uns e a atribuímos à variável 'kernel'. Logo a exibimos no console o conteúdo da variável 'kernel'.
Na próxima parte do código, utilizamos a função 'cv2.erode()' para executar a erosão na imagem. O mesmo processo é realizado na linha seguinte, 
onde aplicamos a operação de dilatação. As imagens resultantes são armazenadas nas variáveis 'erosion' e 'dilation'.
Na próxima linha, executamos o gradiente morfológico na imagem usando a função 'cv2.morphologyEx()'. Em seguida, aplicamos a operação de abertura 
na imagem 'img_opening' e a operação de fechamento na imagem 'img_closing'. As imagens resultantes são armazenadas nas variáveis 'gradient', 
'opening' e 'closing'.
Finalmente, na última parte do código, usamos a função 'cv2_imshow()' para exibir o conteúdo das variáveis no console. É importante observar que 
forma de uso dessa função varia dependendo se estamos executando o código no Python em um computadorou no Google Colab. Para o Google Colab, 
utilizamos 'cv2_imshow("nome_da_variavel")'. Já para o Python em um computador utilizamos 'cv2.imshow("nome_da_variavel_out", nome_da_variavel)'.



















