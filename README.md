# Violence Detection MachineLearning
Proyecto Final de carrera.
Este proyecto podria catalogarse como un proyecto de investigacion, el cual tenia como meta demostrar que era posible crear un algoritmo o red neuronal desde cero y sin usar ninguna bibliotecas keras o open cv o ninguna que resolviera el problema por si misma y sin usar redes convolucionales complejas, el algoritmo debia ser capaz de aprender apartir de un conjunto de imagenes previamente clasificadas en 2 grupos Violentas (agresion fisica) y no-violentas y luego ser capaz de indentificar por si mismo si una imagen nueva contiene violencia fisica o no. 

# Ejemplo Ilustrativo
![ImagenEjemploIlustrativo](https://github.com/YilmerTapias/Violence_Detection_MachineLearning/blob/main/imagen%20de%20cabezera.png)
Adán es el nuevo alcalde de montería, en su primer mandato decide que quiere aumentar la seguridad
de su ciudad, debido a los numerosos reportes diarios de agresión física hacia las mujeres en
lugares públicos. para ello decide implementar en el CCTV de la ciudad, un sistema con inteligencia
artificial, el cual fue entrenado previamente con imágenes violentas y no violentas; usando técnicas
de aprendizaje supervisado concretamente de clasificación de imágenes o visión por computadora
además de otras técnicas de manejo de imágenes y optimización de modelos de aprendizaje como
Adam, el sistema capta la imagen proporcionada por el CCTV y luego de redimensionarla a un
tamaño mucho más pequeño empieza a buscar patrones similares a éste, en el modelo previamente
entrenado y da como resultado las probabilidades de que pertenezca al grupo de violentas o no
violentas, luego escoge la que contenga la mayor probabilidad y determina si es violenta o no violenta,
en el caso de que lo sea enciende las alarmas y notifica a los entes de control. todo esto en cuestión
de segundos.

## Documentacion y explicacion detallada de todo el proyecto
| GoogleDrive | [https://drive.google.com/file/d/1a4z7v6aq0mt2-62MdtQZ0vGrhQvimSkI/view?usp=sharing]

## Conclusiones
![Predicion1](https://github.com/YilmerTapias/Violence_Detection_MachineLearning/blob/main/ImagenesNuevas/resultado1.jpg)
![Predicion2](https://github.com/YilmerTapias/Violence_Detection_MachineLearning/blob/main/ImagenesNuevas/resultado2.jpg)

se creó una red neuronal artificial aplicando transformaciones a las imágenes de nuestro conjunto
de datos y es capaz de diferenciar si una imagen es violenta o no lo es, en tan solo 66 minutos de
entrenamiento en un computador de mesa regular con 4gb de ram con cpu intel celeron de 2.50 GHz
con grafica intel integrada rompiendo así el paradigma de que solo se puede entrenar este tipo de
proyectos en pc de gran potencia, en gran parte se debe al algoritmo de optimización Adam y que el
conjunto de datos no era muy grande.
De todos los datos anteriores vemos que hacer un clasificador de imágenes sin usar convoluciones no
es una idea descabellada podría decirse que es bastante buena, además también queda demostrado que
podemos hacer un clasificador sobresaliente desde cero y sin usar bibliotecas como keras o tensorflow
para su creacion, las cuales nos hacen todo el trabajo sucio. Aun así, estas bibliotecas siempre serán
mucho mejores.
Centrándose un poco más en el problema propuesto y los resultados de las pruebas, vemos como en
algunas imágenes puede predecir con gran seguridad pero en otras aunque predice correctamente
vemos que la precisión de la predicción no es la mejor esto se debe a varios factores destacando el
hecho de que para llevar a cabo un proyecto de esta magnitud que pueda ser usado en las cámaras de
vigilancia de una ciudad o en los pasillos de un colegio, esta debe ser entrenada con muchísimas más
imágenes en distintas situaciones, climas y lugares. Además, como se dijo antes el uso de técnicas
de convolucion para este tipo de problemas sigue siendo la mejor alternativa cuando por ejemplo
tenemos un evento de agresión física en solo una pequeña parte de nuestra imagen o incluso detectar
los gestos de miedo o enojo en una persona, un ejemplo que demuestra esto sería probar nuestro
modelo con imágenes de personas besándose, ya que es cuando nuestro modelo se equivoca más por
la gran cercanía entre los rostros de las personas aunque estas tengan expresiones de felicidad.
También podemos concluir que al hacer pequeñas transformaciones (rotar, zoom, deformar, voltear) a
las imágenes del conjunto de datos puede sacarnos del peligroso camino del sobre ajuste ademas de
ofrecerle a nuestro clasificador vistas diferentes de las imagenes y por lo tanto crear un clasificador
19
mas eficiente, además como se observó en la tabla 1 entre más pequeñas son las dimensiones de las
imágenes en nuestro dataset mas grande se hace el sobre ajuste, quizás usando convolucion sería
distinto.
