Este paper trataba de como, en la competicion de netflix este equipo llego estar en el top 10. Resumiendo brevemente como lo hicieron, ellos basicamente usaron SVD, de manera de obtener las preferencias de usuarios por features y las features de las peliculas, para luego multiplicar ambas matrices obteniendo el ptje. asignado por ese usuario a esa pelicula. Tambien se usaron priors para que cuando solo 1 usuario a dado ptje. a tal pelicula se tenga mas incerteza en estos casos que cuando muchos usuarios le han asignado ptje.

me habria gustado que contara porque se arrepiente de haber puesto lrate=0.001 [learning rate] cuando hace el entrenamiento del SVD-like model, y como esto afecta al resultado final. 

me parecio adecuado el uso de priors para resolver los problemas de falta de datos, mejor dicho los errores que surgen cuando hay pocos datos.

una cosa que me gustaria ver seria como afecta el numero de features usadas, si solo afecta en la velocidad o tambien lo hace en rendimiento.

cuando menciona priors no puedo evitar pensar en que pasaria si hubiera ido full bayesiano, pero como solo usa prior para los espacios en blanco y usarlo no es ligero en computo, lo mas probable es que el beneficio habria sido nulo y solo habria hecho mas lento todo.
