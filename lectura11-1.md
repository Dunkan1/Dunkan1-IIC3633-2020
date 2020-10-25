## Deep Learning based Recommender System: A Survey and New Perspectives (desde 3.5)

Desde la seccion 3.5 del articulo, se proponen mas algortimos, entre estos se usan GAN's, Deep Reinforcement Learning, Neural AutoRegressive, Neural Attention, Restricted Boltzmann Machine y Recurrent Neural Networks, para realizar recomendaciones, ademas de estos se habla tambien de los modelos hibridos. Para finalizar el articulo se mencionan las futuras lineas de investigacion del campo, asi como los problemas a resolver.  

Durante el articulo hay algunas aplicaciones que solo se mencionan en algunos algoritmos, un ejemplo es Session-based Recommendation without User Identifier donde se usan coockie's para recomendar, esta aplicacion de los sistemas recomendadores solo se menciona en los recomendadores basados en Recurrent Neural Networks. Me gustaria que se hubiera indicado en el articulo si esto es porque no hay investigaciones en esto o porque otros recomendadores basados en DP, no funcionan tan bien como en el que esta mencionada la aplicacion.

En el articulo se menciona en la parte de RNN lo siguiente:
_"Despite the success of RNNs in session-based recommendation, Jannach et al. [68] indicated that simple
neighbourhood approach could achieve same accuracy results as GRU4Rec. Combining the neighbourhood with
RNNs methods can usually lead to best performance. This work suggests that some baselines in recent works are
not well-justified and correctly evaluated."_

Esta parte me hace pensar en lo importante que es ver como se evaluo el modelo y tambien contra que se comparo. Como se indica en lo destacado, en un paper se puede hablar del exito de un algoritmo, y si uno se deja llevar solo por esto puede encontrarse con que el algoritmo no es tan bueno como lo que se mencionaba en el paper, por lo tanto se debe ser mas minucioso al revisar los metodos de evaluacion que usaron, las BD sobre las que compararon y los baseline usados.

Otorgando una review completa de los sistemas recomendadores con deep learning, este articulo nos permite tener una idea general del estado del arte y de los problemas a solucionar en esta rama de los sistemas recomendadores, facilitando el estudio posterior mas profundo. 



























