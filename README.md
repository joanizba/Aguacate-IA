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

<h2 align="left">2.1</h2>

###

<p align="left">La distribución es uniforme y simétrica, con una alta concentración alrededor de la mediana, indicando que la mayoría de las ventas totales son intermedias. Los extremos delgados muestran pocos datos en valores muy bajos o muy altos, sugiriendo una distribución normal o ligeramente concentrada.</p>

###

<div align="center">

![2 1](https://github.com/user-attachments/assets/ca1412b1-7f16-4343-892f-26f7314e689e)

</div>

###

<h2 align="left">2.3</h2>

###

<p align="left">Un boxplot muestra la mediana, la dispersión central (IQR), el rango de los datos (bigotes) y los outliers (valores extremos), permitiendo identificar la simetría o sesgo de la distribución y comparar la dispersión y medianas entre categorías o variables.</p>

###

<div align="center">


![2 2](https://github.com/user-attachments/assets/dae79714-fed6-457e-89a3-35f5119d8b3c)

</div>



###

<h2 align="left">2.6</h2>

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

<h2 align="left">4.1</h2>

###

<p align="left">En esta grafica doble vemos como el precio medio y el volumen tienen una relacion, que esta es la de cuando sube uno baja el otro.</p>

###

<div align="center">


![4 1](https://github.com/user-attachments/assets/c6c086f7-b794-4260-a6ef-e4e57cc2b5ad)


</div>

###

<h2 align="left">4.2</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">




![4 2 1](https://github.com/user-attachments/assets/106d6162-be2e-4464-a942-d7a229a09e29)

 
</div>
<div  align="center">


  ![4 2 2](https://github.com/user-attachments/assets/5d8cd95e-6510-4844-b2e4-33e16e80a2de)

</div>

###

<h2 align="left">4.3</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">

  
  ![4 3](https://github.com/user-attachments/assets/881493f6-874d-41ba-bd06-4ceb60f8c857)

</div>

###

<h1 align="left">5. Correlación y regresión</h1>

###

<h2 align="left">5.1</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">


 ![5 1](https://github.com/user-attachments/assets/65235a73-b7df-4fed-bd1f-2405d61e8bd0)

</div>

###

<h2 align="left">5.2</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">

  
![5 2](https://github.com/user-attachments/assets/c438a870-a249-487b-8d28-afd332dba555)

</div>

###

<h2 align="left">5.3</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">


![5 3 b](https://github.com/user-attachments/assets/a45dbd74-df99-4214-a415-a9895622c8fe)

</div>
<div align="center">


![5 3 a](https://github.com/user-attachments/assets/06274cfb-95da-4ae3-aa4e-7de6a8f6308a)

</div>

###

<h2 align="left">5.4</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">


![5 8](https://github.com/user-attachments/assets/3c68c45f-f992-4465-90d2-2474c219cc4e)

</div>
<div align="center">

  ![5 8 2](https://github.com/user-attachments/assets/bac7466c-b23f-473c-a1d1-80fd1529a251)

</div>
###
<h2 align="left">5.5</h2>

###

<p align="left">Hello World!!</p>

###

<div align="center">


![5 9](https://github.com/user-attachments/assets/80c8ca48-85c5-4599-a9cc-7a81e7cfa684)

</div>

###
