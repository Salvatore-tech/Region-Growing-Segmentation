# Segmentación con particionamiento k-means
## Introducción
Agrupamiento es una clase de aprendizaje no supervisado ampliamente utilizado de algoritmos que ha
encontrado en varios problemas como los motores de recomendación, análisis red social, imágenes
médicas, detección de anomalías y segmentación de imágenes.
Los algoritmos de agrupamiento se agrupan en cuatro principales:
- Particionamiento
- Red
- Grafo
- Jerárquico
El algoritmo k-means comparte las características de los algoritmos de particionamiento y ha estado
aplicado con suceso a problemas como reconocimiento de caras en frame de video etc.
Es una técnica de aprendizaje automático no supervisado que podemos aplicar para encontrar nuevos
patrones en nuestros datos. Lo interesante de este algoritmo es que también podemos usarlo para tareas
de procesamiento de imágenes. Y de la misma manera que con otro tipo de datos, podemos encontrar
patrones de píxeles en nuestras imágenes que nos permitirán procesarlos de una manera más rápida y
eficiente. Vamos a utilizar el algoritmo de agrupamiento de k-means para realizar la segmentación en una
imagen. 
## Algoritmo k-means
El algoritmo de agrupamiento de K-Means es un algoritmo de agrupamiento iterativo que intenta asignar
puntos de datos a exactamente un grupo del número K de grupos que predefinimos.
Al igual que con cualquier otro algoritmo de agrupación en clústeres, intenta hacer que los elementos de
un clúster sean lo más similares posible, al mismo tiempo que hace que los clústeres sean lo más diferentes
posible entre sí. Lo hace asegurándose de que la suma de la distancia al cuadrado entre los puntos de datos
en un grupo y el centroide de ese grupo sea mínima. 
El centroide del conglomerado es el valor medio de todos los valores del conglomerado.
De forma más correcta podemos decir que la mejor elección del centro consiste en minimizar la suma de
las distancias cuadráticas tras todos los puntos y el centro más cercano.
## Pasos algoritmo
- Inicialización: en primer lugar, debe inicializar aleatoriamente dos puntos denominados centroides
del clúster. Aquí, debe asegurarse de que los centroides de su clúster representados por una cruz
naranja y azul, como se muestra en la imagen, sean menores que los puntos de datos de
entrenamiento representados por puntos azul marino. El algoritmo de agrupación de k-means es
un algoritmo iterativo y sigue los dos pasos siguientes de forma iterativa.
Una vez que haya terminado con la inicialización, pasemos al siguiente paso. 
- Asignación de objetos a los centroides: en este paso, pasará por todos los puntos de datos azul
marino para calcular la distancia entre los puntos de datos y el centroide del clúster inicializado en
el paso anterior. Ahora, dependiendo de la distancia mínima desde el centroide del cúmulo naranja
o el centroide del cúmulo azul, se agrupará en ese grupo en particular. Entonces, los puntos de
datos se dividen en dos grupos, uno representado en color naranja y el otro en color azul como se
muestra en el gráfico. 
- Actualización de centroides: Se actualiza la posición del centroide de cada grupo tomando como
nuevo centroide la posición media de los objetos pertenecientes a dicho grupo. De manera similar,
moverá el centroide del clúster naranja al promedio de puntos de datos naranjas. Por lo tanto, los
nuevos centroides del clúster se verán como se muestra en el gráfico. 
- Convergencia: se repiten los dos pasos anteriores de forma iterativa hasta que os centroides del
clúster dejen de cambiar sus posiciones y se vuelvan estáticos. Una vez que los clústeres se vuelven
estáticos, se dice que el algoritmo de clústeres de k-medias converge.
Finalmente, el algoritmo de agrupamiento de k-medias converge y divide los puntos de datos en
dos grupos claramente visibles en naranja y azul. Puede suceder que k-means acabe convergiendo
con diferentes soluciones dependiendo de cómo se inicializaron los clústeres. 
