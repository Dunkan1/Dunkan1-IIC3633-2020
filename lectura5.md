### Combining Predictions for Accurate Recommender Systems
El paper basicamente exploraba distintas formas de bending para mejorar el performance, usando distintos algoritmos CF (colaborative filtering), y con un modelo de regresion lineal como baseline. los resutados mostraron que con bending's se puede mejorar el RMSE de modelos individuales (Donde incluso el que les reporto mayor RMSE que fue K-Nearest Neighbors Blending con 0.885-0.884 es mejor que los 18 modelos individuales que probaron).

En  particular a mi me sorprendio los tiempos que toma entrenar algunos bendings por ejemplo en "Bagging with Neural Networks, Polynomial Regression
and GBDT" tomo (total train time: 158.2[h]) entrenarlo y (prediction time 4.5[h]) para predecir. Por eso me gusto que incluyeran esto al final, donde al recomendar un "sistema recomendador" no solo se basan en el RMSE sino que tambien en el tiempo de prediccion.

Me hubiera gustado ver otras metricas, porque como vimos en otros papers hay mas formas de medir una recomendacion, por ejemplo otros atractivos en un sistema recomendador son su: Serendipity, Robustness, etc. [Evaluating Recommendation Systems] los cuales se pueden medir con metricas distintas a RMSE. Sin embargo entiendo que se escapa del alcance del paper.

Para finalizar me gustaria decir que este paper es bueno navegar sobre distintos metodos de bending, y permite probar su importancia en los systemas recomendadores.
