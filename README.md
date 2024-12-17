<h1 align="left">Avocado-P1</h1>

###

<p align="left">Un proyecto educativo enfocado en la implementación de soluciones de inteligencia artificial utilizando Python y Jupyter Notebook.</p>

###

<h1 align="left">Descripción</h1>

###

<p align="left">El proyecto Aguacate-IA parece ser un conjunto de notebooks de Jupyter orientados a tareas de inteligencia artificial y análisis de datos. Aunque el repositorio no incluye una descripción detallada, se deduce que cada notebook contiene soluciones o desarrollos específicos, posiblemente relacionados con un conjunto de ejercicios o tareas académicas.<br><br>Punto 1 - Series Temporales<br>Punto 2 -  Gráficos para visualización<br>Punto 3 -  Elasticidad del precio<br>Punto 4 -  Análisis cohortes<br>Punto 5 - Correlación y regresión<br><br>El repositorio, en su estado actual, es una base funcional pero carece de detalles claros sobre los objetivos o casos de uso específicos. Con una mejora en su documentación, podría orientar mejor a los usuarios interesados en replicar o entender el contenido del proyecto.</p>

###

<h1 align="left">Planificación</h1>

###

<div align="center">


![trello](https://github.com/user-attachments/assets/f5bbd595-eae2-4fbd-b817-340d01450caa)


</div>

###

<h1 align="left">EDA (Exploratory Data Analysis)</h1>

###

<p align="left">Iniciamos el análisis realizando un EDA (Exploratory Data Analysis) en el transcurso del cual descubrimos que:<br><br>El dataset tiene 18.249 filas y 11 columnas.<br>Los datos están tomados semanalmente, es decir, hay 4/5 mediciones por cada mes.<br>El rango de fechas para la columna 'Date' incluye los años 2015 a 2018.<br>El año 2018 está incompleto, de modo que sólo tenemos datos de enero a marzo.<br>En las columnas de calibre ('4046', '4225', '4770') hay valores a cero (0.0). En concreto, 242 ceros en la columna '4046', 61 ceros en la columna '4225', 5.497 ceros en la columna '4770'. Todos estos registros corresponden a aguacates de tipo orgánico, excepto una fila (df.iloc[2998]) que es de tipo convencional.<br>La columna 'Total Bags' tiene 15 filas a cero (0.0), todas correspondientes a aguacates de tipo orgánico.<br>Asimismo, las columnas 'Small Bags', 'Large Bags' y 'XLarge Bags' tienen 159, 2.370 y 12.048 filas a cero (0.0) respectivamente.<br>La columna 'region' incluye información heterogénea, es decir, una mezcla de ciudades, regiones, regiones ampliadas (greater regions), y también registros para el total de Estados Unidos (TotalUS).<br>La región WestNewMexico tiene 3 filas menos que el resto de regiones.</p>

###

<h1 align="left">Segmentación</h1>

###

<div align="center">

![USA-regions_coloreado](https://github.com/user-attachments/assets/d8022082-0ab6-4849-9ed1-8d4006561a61)


</div>

###

<h1 align="left">1. Series Temporales</h1>

###

<h2 align="left">1.3</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h2 align="left">1.4</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h2 align="left">1.6</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h1 align="left">2. Gráficos para visualización</h1>

###

<h2 align="left">2.1 Gráfico de Violín de Volumen de Ventas por Región</h2>

###

<p align="left">La distribución es uniforme y simétrica, con una alta concentración alrededor de la mediana, indicando que la mayoría de las ventas totales son intermedias. Los extremos delgados muestran pocos datos en valores muy bajos o muy altos, sugiriendo una distribución normal o ligeramente concentrada.</p>

###

<div align="center">

![2 1](https://github.com/user-attachments/assets/ca1412b1-7f16-4343-892f-26f7314e689e)

</div>

###

<h2 align="left">2.3 Boxplot Comparativo de Precios entre Años</h2>

###

<p align="left">Un boxplot muestra la mediana, la dispersión central (IQR), el rango de los datos (bigotes) y los outliers (valores extremos), permitiendo identificar la simetría o sesgo de la distribución y comparar la dispersión y medianas entre categorías o variables.</p>

###

<div align="center">


![2 2](https://github.com/user-attachments/assets/dae79714-fed6-457e-89a3-35f5119d8b3c)

</div>



###

<h2 align="left">2.3 Gráfico de Líneas de Precios Promedios por Año</h2>

###

###

<div align="center">


  ![2 3](https://github.com/user-attachments/assets/ec55f53b-cb00-4074-ba3e-31e800bcd153)

</div>

###

<h1 align="left">3. Elasticidad del precio</h1>

###

<h1 align="left">3.1</h1>

###

<p align="left">Hello World!!</p>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h2 align="left">3.2</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h2 align="left">3.3</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h1 align="left">4. Análisis cohortes</h1>

###

<h2 align="left">4.1 Cohortes Basadas en Precios Promedios Trimestrales</h2>

###

<p align="left">En esta grafica doble vemos como el precio medio y el volumen tienen una relacion, que esta es la de cuando sube uno baja el otro.</p>

###

<div align="center">


![4 1](https://github.com/user-attachments/assets/c6c086f7-b794-4260-a6ef-e4e57cc2b5ad)


</div>

###

<h2 align="left">4.2 Cohortes por Región y Fecha</h2>

###

<p align="left">En esta veremos lo mismo de lo anterior pero mas detalladamente por trimestre y region</p>

###

<div align="center">




![4 2 1](https://github.com/user-attachments/assets/106d6162-be2e-4464-a942-d7a229a09e29)

 
</div>
<div  align="center">


  ![4 2 2](https://github.com/user-attachments/assets/5d8cd95e-6510-4844-b2e4-33e16e80a2de)

</div>

###

<h2 align="left">4.3 Análisis de Cohortes en Función del Tipo de Bolsa</h2>

###

<p align="left">El análisis de cohorte en función del tamaño de bolsa, vemos claramente que las de tipo Small Bags son las más vendidas. No obstante, son las más inestables también. Aunque las Large Bags se venden en menor cantidad, su volumen de venta es mucho más estable, lo que podría indicar una preferencia de compra por parte de los clientes.</p>

###

<div align="center">

  
  ![4 3](https://github.com/user-attachments/assets/881493f6-874d-41ba-bd06-4ceb60f8c857)

</div>
<div algin="center">



  ![4 3 1](https://github.com/user-attachments/assets/08cdbcba-d3da-42d5-9379-a63d5da024bd)

</div>
###

<h1 align="left">5. Correlación y regresión</h1>

###

<h2 align="left">5.1 Matriz de Correlación</h2>

###

<p align="left">Si seleccionamos las variables numéricas, podemos crear un grafo de tio heatmap para la matiz de coorrelación entre datos</p><br>
<p align="left"> Total Volume esta ligeramente correlacionado con total bags y 4046 como 4225. Esto se debe que la ventea de los calibres de 4046 y 4225 defienen el volument de ventas</p><br>
<p align="left">El hecho de que estas variables estén altamente correlacionadas puede influir en el estudio dado que los modelos de regresión lineal con alta correlación entre sus variables pueden resultar altamente inestables, generar errores numéricos y un rendimiento de predicción muy deficiente.</p>

###

<div align="center">


 ![5 1](https://github.com/user-attachments/assets/65235a73-b7df-4fed-bd1f-2405d61e8bd0)

</div>

###

<h2 align="left">5.2 Análisis de Dispersión entre Variables Clave</h2>

###

<p align="left">Regresión lineal (rojo):
Modelo simple que asume una relación lineal negativa, No captura bien la tendencia real de los datos debido a su simplicidad. Útil como referencia inicial o para datos estrictamente lineales.</p>
<p align="left">Regresión polinómica de grado 2 (verde):
Modelo más flexible que captura mejor la curvatura en la relación, Ajuste superior al modelo lineal, especialmente cuando los datos tienen una tendencia no lineal. Muestra que el precio promedio disminuye rápidamente al inicio y luego se estabiliza o sube en volúmenes altos.</p>
###

<div align="center">

  
![5 2](https://github.com/user-attachments/assets/c438a870-a249-487b-8d28-afd332dba555)

</div>

###

<h2 align="left">5.3 Predicciones Mensuales Usando Datos Trimestrales</h2>

###

<p align="left">El gráfico principal muestra los datos de entrenamiento y prueba, Puntos azules datos entrenamiento, Puntos naranjas dataos evaluativos.
pendiente negativa, lo que indica que a medida que Total Volume aumenta, AveragePrice tiende a disminuir modelo no captura bien la variabilidad.</p>

###

<div align="center">


![5 3 b](https://github.com/user-attachments/assets/a45dbd74-df99-4214-a415-a9895622c8fe)

</div>
<div align="center">
<p align="left">El Error Porcentual varía considerablemente, con valores negativos y positivos, lo que indica subestimación y sobreestimación en diferentes puntos. El modelo no predice con alta precisión, ya que los errores no son pequeños y están dispersos. </p>

![5 3 a](https://github.com/user-attachments/assets/06274cfb-95da-4ae3-aa4e-7de6a8f6308a)

</div>
<p align="left">Un valor de 0.8275 indica que hay una desviación significativa </p>
<p align="left">Un valor de 0.1782 significa que el modelo solo explica el 17.82% de la variabilidad </p>
###

<h2 align="left">5.4 Modelos de Regresión para Diferenciar Volúmenes de Ventas</h2>

###

<p align="left">regresión lineal muestra las predicciones frente a los valores reales de AveragePrice. Los puntos azules siguen una tendencia lineal débil alrededor de la línea diagonal (que indica la predicción perfecta). Esto sugiere que el modelo tiene dificultades para ajustar bien los datos, especialmente cuando se trata de valores reales más altos, ya que no captura correctamente la dispersión de los precios en esas áreas.</p>
<p align="left">regresión polinómica muestra cómo las predicciones se ajustan mejor a los valores reales de AveragePrice. Los puntos rojos se acercan más a la línea diagonal, indicando un ajuste más preciso en comparación con el modelo lineal. Este modelo parece capturar mejor la variabilidad de los datos, logrando una representación más adecuada de las relaciones entre los valores reales y las predicciones.</p>


<div align="center">


![5 8](https://github.com/user-attachments/assets/3c68c45f-f992-4465-90d2-2474c219cc4e)

</div>
<p align="left">El RMSE mide la precisión de las predicciones de un modelo</p><br>
<p align="left">Un valor más bajo indica predicciones más cercanas a los valores reales. En este caso, el modelo polinómico tiene un RMSE de 0.8542, ligeramente más bajo que el modelo lineal (RMSE de 0.8634), lo que indica que el modelo polinómico tiene predicciones más precisas en promedio.</p><br>
<p align="left">El R² mide cuánta variabilidad de los datos es explicada por el modelo</p><br>
<p align="left"> Un valor más alto de R² indica un mejor ajuste. En este caso, el modelo polinómico tiene un R² de 0.2529, mayor que el modelo lineal (R² de 0.1257), lo que sugiere que el modelo polinómico captura mejor la variabilidad de los datos. Sin embargo, ambos valores son bajos, lo que indica que ninguno de los modelos explica una gran parte de la variabilidad, sugiriendo que podrían existir otros factores que influyen en los precios de los aguacates.</p>
<div align="center">

  ![5 8 2](https://github.com/user-attachments/assets/bac7466c-b23f-473c-a1d1-80fd1529a251)

</div>
###
<h2 align="left">5.5  Análisis de la Influencia de las Ventas Totales en el Precio Promedio</h2>

###

<p align="left">La imagen muestra una representación gráfica de la relación entre Total Volume (volumen total) y Average Price (precio promedio) junto con dos modelos de tendencia: lineal (en azul) y polinómica de segundo grado (en rojo punteado)</p>

###

<div align="center">


![5 9](https://github.com/user-attachments/assets/80c8ca48-85c5-4599-a9cc-7a81e7cfa684)

</div>

<p align="left">Gráfico de dispersión:

Cada punto muestra la relación entre Total Volume (volumen total) y Average Price (precio promedio).
Los puntos se concentran en valores bajos de Total Volume y muestran una tendencia descendente: al aumentar el volumen, el precio tiende a disminuir.
Se observa una ligera curvatura, indicando que la relación no es completamente lineal.</p><br>
<p align="left">Línea de tendencia lineal (azul sólida):

Modelo de regresión lineal con pendiente negativa.
Representa que al aumentar el Total Volume, el Average Price baja.
La banda azul clara indica mayor incertidumbre en valores altos de volumen.</p><br>

<p align="left">Tendencia polinómica de segundo grado (roja punteada):

Modelo cuadrático que captura mejor la curvatura de los datos.
Es más preciso que la regresión lineal, especialmente en valores bajos y altos de volumen.</p><br>
<p align="left">Comparación de modelos:

Regresión Lineal: Sencilla pero no captura la curvatura; funciona bien en valores centrales.
Regresión Polinómica: Más flexible y ajustada, aunque la curvatura es ligera.</p>

###
