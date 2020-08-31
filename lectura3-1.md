El paper hablaba de como RMSE no era una buena metrica para evaluar top-N recomendation, a lo que proponia una metrica que directamente media el top-N performance, esta consistia en usar del set de test solo aquellos elementos que se sabian eran aceptados por el usuario (5 estrellas) y en usar el recall y presicion que ellos definian. Para terminar propusieron modificaciones en 2 sistemas recomendadores conocidos, de manera que se basaran en mejorar la top-N performance y no en diminuir el MSE, estos eran: pureSVD y NNCosNgbr.

Me gusto que agregaran el analisis para longTail, ya que a pesar de no ser siempre el problema principal, recomendar items no populares o conocidos es una herramienta util para diversos problemas, por ejemplo: promocionar productos emergentes.

Fue bueno que usaran mas de un dataset y que compararan con modelos que se enfocan en tener un maximo RMSE porque asi se destaca la diferencia entre esta forma de evaluar y la propuesta.

No me gusta que antes de proponer sistemas recomendadores que mejoren la metrica propuesta, no prueben que la metrica funciona, por ejemplo si ellos dicen que RMSE no sirve para los motivos mencionados y proponen una metrica para solucionarlos deben, antes de proponer algoritmos, ver que esa metrica efectivamente solucione esos problemas, de esta manera no hacen un analisis de sus modelos sin saber si sobre lo que los evaluaron era fiable.

Tampoco me parece correcto que solo a sus sistemas recomendadores modificados hayan agregado el analisis para diferentes variables latentes, puesto que a svd++ y asynSVD los dejaron con 200 de estas. Esto nos hace asumir que ellos probaron con distintas variables latentes para ellos y dejaron la mejor, pero como no hay diferencia entre los graficos para long tail y completo, me genera dudas sobre si realmente lo hicieron, ya que implicaria que esa cantidad de variables latentes es la mejor para ambos en ambos test's.

