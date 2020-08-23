El paper propone un criterio de optimizacion derivado de la maxima a posterior que usa la comparacion entre un item y otro, esto es si j se sintonizo y i no, entonces j>i, de esta manera no se incurre en el error de tratar a los elementos sin informacion como informacion negativa. Luego proponen un algoritmo para maximizar BPR-OPT (criterio anteriormente mencionado) que se basa en desenso del gradiente con bootstrap sampling, se usa sampling ya que solo se necesita una fraccion de una iteracion completa para que el algoritmo converga. Por ultimo nos proponen como usar sus ideas en 2 de los sistemas recomendadores mas populares que son knn y factorizacion de matriz.

Me parecio ingeniosa la idea de usar una matriz para mantener un orden entre items y asi no tener que ponerle - a los ? de esta.

Como es bayesiano pudieron haber puesto como varia la confianza en la prediccion del parametro, me habria gustado ver mas graficos de esto.

Una de las cosas que critico es que segun el paper "All users are presumed to act independently of each other." se que esto es para poder aplicar bayes y facilitar los calculos, pero tambien siento que se esta perdiendo informacion importante al hacer esto.

Otra cosa es que no explican porque el prior es una normal, me imagino que tambien fue para simplicar ya que la normal es ampliamente conocida, de todas formas siento que esto es asumir demasiado si se toma en cuenta que hablamos del prior de parametros en distintos modelos.
