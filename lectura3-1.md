El paper hablaba de como RMSE no era una buena metrica para evaluar top-N recomendacion, por lo que ellos proponian una metrica que directamente media el top-N performance, que consistia en usar el recall y presicion que ellos definian, ademas el set de test solo debia tener aquellos elementos que se sabian eran aceptados por el usuario (5 estrellas). Para terminar propusieron cambios en 2 sistemas recomendadores conocidos que buscaran mejorar la top-N performance, de manera que no se basaran en diminuir el MSE, estos eran: pureSVD y NNCosNgbr.

me gusto agregaran el analisis para longTail, ya que a pesar de no ser siempre el main problema, recomendar items no populares o conocidos es una herramienta util para promocionar productos emergentes

fue bueno que usaran mas de un dataset y que compararan con modelos que se enfocan en tener un maximo RMSE porque asi se destaca la diferencia entre esta forma de evaluar y la propuesta

no me gusta que antes de proponer sistemas recomendadores que mejoren la metrica propuesta, no prueben que la metrica funciona, por ejemplo si ellos dicen que RMSE no sirve para los motivos mencionados y proponen una metrica para solucionarlos deben antes ver que esa metrica efectivamente solucione esos problemas, hacen un analisis de sus modelos sin saber si sobre lo que los evaluaron era fiable.

tampoco me parece correcto que solo a sus metricas hayan agregado el analisis para diferentes variables latentes y svd++ y asynSVD lo hayan dejado con 200, no hace asumir que ellos probaron con distintas variables latentes para ellos y dejaron la mejor, pero no hay diferencia entre long tail y completo, debieron escoger la mejor cantidad para cada uno de estos

