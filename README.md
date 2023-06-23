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

## Referências
https://pt.wikipedia.org/wiki/OpenCV
https://www.geeksforgeeks.org/python-opencv-cv2-imread-method/
https://www.geeksforgeeks.org/python-numpy/
https://www.geeksforgeeks.org/python-opencv-cv2-imshow-method/
https://www.geeksforgeeks.org/erosion-dilation-images-using-opencv-python/
https://www.geeksforgeeks.org/python-opencv-cv2-erode-method/
https://www.geeksforgeeks.org/python-grayscaling-of-images-using-opencv/
https://docs.opencv.org/3.4/d3/df2/tutorial_py_basic_ops.html#:~:text=The%20shape%20of%20an%20image,the%20image%20is%20color)%3A
https://docs.opencv.org/4.x/d9/d61/tutorial_py_morphological_ops.html
https://stackoverflow.com/questions/16655962/opencv-understanding-kernel?rq=3
https://stackoverflow.com/questions/21746934/whats-the-meaning-of-the-values-in-the-opencv-image-representation#:~:text=%22imread%22%20defaults%20the%20second%20argument,each%20pixel%20of%20your%20image.
https://blog.xpeducacao.com.br/opencv-em-python/#:~:text=OpenCV%20%C3%A9%20uma%20biblioteca%20de,operacionais%20e%20linguagens%20de%20programa%C3%A7%C3%A3o.
https://opencv24-python-tutorials.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_morphological_ops/py_morphological_ops.html

















