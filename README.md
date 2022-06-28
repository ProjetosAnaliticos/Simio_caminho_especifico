# Como fazer um objeto seguir por um caminho específico no Simio? 

Suponha que eu tenha um banco, onde pessoas idosas entrem numa fila preferencial, e o restante das pessoas siga pela fila comum. Como criar essa lógica?
 
Layout:
- Adicionar 1 server
-	Adicionar 2 sources
-	Adicionar 2 sinks

Coloque os 2 sources um ao lado do outro e ligue ambos ao server através de um path. Repita o mesmo processo ligando o server aos dois sink através do path também.

Processo:
Selecione o path (entre o servidor e um dos sink) que você quer que seja diferente, depois vá a opção “routing logic”.
 
[](https://github.com/ProjetosAnaliticos/Simio_caminhoespecifico/blob/main/fila01.png)


Dentro de “routing logic” vá a opção selection weigth, lá você encontrará inúmeras formas de programar o path. Digite Is.( nome que você deu ao source desejado)

 [](https://github.com/ProjetosAnaliticos/Simio_caminhoespecifico/blob/main/fila02.png)


Para finalizar, selecione o output do servidor e vá na opção “ routing logic” novamente, porem no servidor você encontrará a opção “outbound link rule”, onde você encontrará 2 alternativas, selecione a “by link weight”

 [](https://github.com/ProjetosAnaliticos/Simio_caminhoespecifico/blob/main/fila03.png)



Você verá que os idosos seguirão por uma fila, e o restante, para a fila comum!

Vide o arquivo em anexo.

Autora: Kelly Alves de Paula
Wagner Gurgel

Revisão: Arnaldo Gunzi

