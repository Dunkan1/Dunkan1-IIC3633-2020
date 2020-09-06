En el paper proponian usar una factorizacion matricial no negativa (NMF) para poder hacer clusters de documentos segun sus topicos. La razon de porque proponian esto en vez de SVD es que, SVD crea un espacio latente ortogonal, como es ortogonal cada dimension es independiente, lo cual no es cierto ya que hay topicos que no lo son, por lo tanto usaron (NMF) que no crea un espacio ortogonal. NMF basicamente consiste en usar factorizar la "term-
document matrix X" en las matrices U y V, y por ultimo usar V para determinar a que cluster pertencen. 

Por las tablas de resultados se puede ver que NMF no logra una mejora sobre SVD con respecto a Accuracy en ninguna de las 2 tablas, de hecho es al contrario. El que si lo logra es NMF-NCW pero en la explicacion de resultados esto no se indaga, lo que me parece un error del paper.

Por otro lado me parece una gran idea como desde una persepcion del problema, se adapta a una solucion matematica. En este paper esto se ve en que la matriz sea no negativa. Lo que perciben en el problema es que los Documentos deben ser la adicion de distintos topicos, por lo tanto la traduccion matematica de esto fue usar una matriz no negativa para representarlo.  

Una idea que se me ocurre de este paper seria adaptar el probabilistic clustering, manteniendo la idea de adiccion de distintos topicos y topicos que pueden tener "overlap" entre ellos, esto seria permitiendo "overlap" en las gaussianas. 
