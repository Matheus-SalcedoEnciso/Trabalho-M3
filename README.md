# Trabalho-M3

## Código
Primeiramente são importadas as bibliotecas OpenCV , Numnby para o programa. Depois é adicionada a função 'cv2_imshow' da google.colab.patches, para melhor exibição de imagens.
Na segunda célula, carregamos a imagem 'j.png' com a função 'cv2.imread', depois vem o processo de conversão da imagem de outros espaços de 
cores para tons de cinza. Por último, a imagem resultante é armazenado na variável 'img'.
O mesmo processo de repete na próxima linha, a imagem 'j_ruido.png' é carregada com a função 'cv2.imread', então a imagem é convertida para 0 numa 
escala de tons de cinza de 0 até 255 e acaba sendo guardada na variável 'img_opening'.
Finalizando, carregamos a última imagem 'j_furos.png' com a função 'cv2.imread', convertimos a imagem em tons de cinza, e a atribuimos à variável 
'img_closing'.
Acessamos a forma da imagem com 'img.shape'. Ele retorna uma tupla do número da altura e largura. Na próxima linha, criamos uma matriz ( 5 por 5 ) 
e o atribuimos ao kernel. Depois exibimos no console o conteúdo da variável do Kernel.
Na terceira célula, utilizamos a função cv2.erode() para executar erosão na imagem. O mesmo processo é feito na próxima linha. Ambas imagens 
resultantes são armazenadas em suas respectivas variáveis.
Na quarta célula, executamos o gradiente morfológico na imagem utilizando a função. morphologyEx(). Na próxima linha executamos a abertura da 
imagem. E na próxima linha aplicamos o fechamento da imagem. Todos as imagens resultantes são guardados nas suas respectivas variáveis, gradient, 
opening e closing.
Na última parte do código, usamos a funação cv2.imshow() para exibir todos os conteúdos da variáveis que utilizamos no console. Observando que há 
uma diferença dependendo se estamos utilizando o Python no próprio computador ou estamos usando o Google Colab.
Se utilizamos o Google Colab, usariamos: cv2_imshow("nome da variável").
Se utilizamos o computador: sv2_imshow('nome da variável'_out, nome da variavél).


















