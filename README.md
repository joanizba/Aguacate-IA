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
<p align="left"># Planificación y Progreso del Análisis de Aguacates

En este trabajo, hemos organizado las tareas en **tres categorías**: **pendientes**, **en progreso** y **completadas**.

---

## **1. Tareas Pendientes**
- **Análisis de series temporales**:  
  Descompondremos los precios de los aguacates para identificar **tendencias** y **estacionalidades**.  
- **Creación de gráficos para visualización de datos**:  
  Nos permitirá **presentar los resultados de manera clara y comprensible**.  
- **Cálculo de la elasticidad del precio**:  
  Ayudará a entender cómo los **cambios en los precios** afectan la **demanda** de los aguacates.  

---

## **2. Tareas en Progreso**
- **Matriz de correlación**:  
  Estamos explorando las **relaciones entre variables clave**.  
- **Análisis de dispersión entre variables**:  
  Facilitará visualizar cómo se distribuyen los **datos**.  
- **Predicciones (mensuales, trimestrales y anuales)**:  
  Nos permitirá **anticipar el comportamiento del mercado**.  

---

## **3. Tareas Completadas**
- **Gráfico de violín del volumen de ventas por región**:  
  Proporciona una visión detallada de cómo varía el **volumen de ventas** en diferentes regiones.  
- **Gráfico de líneas de precios promedio por año**:  
  Permite observar la **evolución** de los precios a lo largo del tiempo.  
- **Análisis de cambios en precios anuales**:  
  Ofrece una visión clara de las **fluctuaciones del mercado**.  

---

## **Conclusión**
Con esta planificación, esperamos completar las **tareas pendientes** y lograr un **análisis exhaustivo** que nos permita hacer **recomendaciones informadas** sobre la venta de aguacates.

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

<h2 align="left">1.1 Descomposición de Series Temporales de Precios</h2>
<p align="left">
  - Introducción:
Esta gráfica muestra la descomposición de la serie temporal de los precios promedio de aguacates. Se separa en tres componentes: tendencia, estacionalidad y residuos.
</p>
<br>
<p align="left">
  - Serie Original:
La parte superior muestra la serie original, donde se observan las fluctuaciones de los precios a lo largo del tiempo.
</p>
<br>
<p align="left">
  - Tendencia:
El segundo gráfico muestra la tendencia, que indica la dirección general de los precios. Aquí, los precios han tenido una tendencia ligeramente descendente.
</p>
<br>
<p align="left">
  - Estacionalidad:
El tercer gráfico muestra la estacionalidad, que resalta las variaciones regulares y predecibles en los precios, como picos y valles, a lo largo de los años.
</p>
<br>
<p align="left">
  - Residuos:
Finalmente, los residuos son las fluctuaciones aleatorias que no se explican por la tendencia ni la estacionalidad. Aparecen dispersos alrededor de la línea base.
</p>
<br>
<p align="left">
  - Conclusión:
En resumen, la descomposición nos ayuda a entender cómo los precios varían por la tendencia general, los patrones estacionales y las fluctuaciones aleatorias, lo que es útil para análisis futuros.
</p>

<div align="center">

  ![1 1](https://github.com/user-attachments/assets/b68bb608-36fa-49dc-938e-3a791d9d1a6e)

</div>

###

<h2 align="left">1.2 Tendencia de Ventas a lo Largo del Tiempo</h2>
<p align="left">
  - Introducción:
Esta gráfica muestra la tendencia del volumen total de ventas de aguacates a lo largo del tiempo. Los puntos verdes representan los datos mensuales de ventas, conectados por líneas que permiten visualizar la evolución del volumen de ventas.
</p>
<br>
<p align="left">
  - Fluctuaciones y Picos:
Podemos observar una gran variabilidad en los datos, con picos notables en ciertos momentos. Por ejemplo, se destacan picos altos en febrero de 2015, febrero de 2016 y febrero de 2017, lo que indica que en esos meses hubo un aumento significativo en las ventas de aguacates.
</p>
<br>
<p align="left">
  - Tendencia General:
A pesar de los picos, podemos ver que el volumen de ventas tiene una tendencia general creciente después de 2015, con un incremento sostenido en los últimos años, lo que indica un aumento en la demanda de aguacates.
</p>
<br>
<p align="left">
  - Ciclicidad:
Aunque no es tan marcado, podemos percibir una posible estacionalidad en las ventas, con algunos picos y valles que se repiten en ciertos meses del año, como en febrero y agosto.
</p>
<br>
<p align="left">
  - Conclusión:
En resumen, la gráfica ilustra cómo el volumen de ventas de aguacates ha fluctuado a lo largo del tiempo, con picos en ciertos meses y una tendencia creciente general. Estos datos son útiles para prever futuros patrones de demanda y para tomar decisiones estratégicas relacionadas con la distribución y los precios.
</p>

<div align="center">

![1 2](https://github.com/user-attachments/assets/11b491e9-8eb1-49ef-b6c5-8ef2c8450427)

  
</div>

###

<h2 align="left">1.3 Comparación de Precios Promedio Mensuales</h2>

###

<p align="left">
  - Introducción:
La gráfica muestra la tendencia del precio promedio mensual de los aguacates entre 2015 y 2018. Los puntos y líneas permiten ver las fluctuaciones de los precios a lo largo del tiempo.
</p>
<br>
<p align="left">
  - Fluctuaciones y Picos:
Podemos observar una gran variabilidad en los precios a lo largo del tiempo, con caídas y subidas marcadas. Un detalle importante es el pico máximo que se alcanza en mediados de 2017, donde el precio supera los 1.8 dólares. Esto representa un aumento significativo en comparación con otros períodos.
Por otro lado, también se nota una caída pronunciada entre finales de 2015 y principios de 2016, donde el precio llega a su punto más bajo, cercano a 1.2 dólares.
</p>
<br>
<p align="left">
  - Tendencia General:
A lo largo de los años, la gráfica refleja una tendencia general ascendente en los precios, especialmente desde mediados de 2016 hasta 2017, donde se observa un incremento sostenido. Este comportamiento sugiere un aumento en la demanda o posibles factores externos que afectaron la disponibilidad del producto, como la producción o el mercado internacional.
</p>
<br>
<p align="left">
  - Ciclicidad:
Aunque no es completamente regular, se pueden identificar patrones cíclicos en los precios, con períodos de caída seguidos de recuperación. Es posible que estos ciclos estén relacionados con factores estacionales, como la oferta limitada en ciertos meses o la mayor demanda en otros, lo cual explica las subidas y bajadas que se repiten parcialmente.
</p>
<br>
<p align="left">
  - Conclusión:
En resumen, la gráfica muestra que los precios promedio mensuales de los aguacates presentan fluctuaciones importantes, con picos notables en 2017 y caídas destacadas en 2016. A pesar de estas variaciones, hay una tendencia general al alza, lo que podría indicar un aumento en la demanda a lo largo del tiempo. Estos datos son útiles para entender los patrones de precios y analizar cómo factores como la producción, el clima o el comercio afectan al mercado de los aguacates.
</p>

###

<div align="center">

  ![1 3](https://github.com/user-attachments/assets/4091de00-a5db-40cf-b300-f76dc98dfa0b)


</div>

###

<h1 align="left">2. Gráficos para visualización</h1>

###

<h2 align="left">2.1 Gráfico de Violín de Volumen de Ventas por Región</h2>

###

<p align="left">
  - Introducción:
La gráfica muestra la distribución del volumen total de ventas en una región seleccionada ("GreaterRegion"). Es una gráfica de violín que combina un diagrama de caja y un histograma suavizado para representar cómo se distribuyen los datos de ventas.
</p>
<br>
<p align="left">
  - Distribución de los Datos:
Se observa que el volumen total de ventas está concentrado en un rango específico, con una mayor densidad alrededor de valores cercanos al centro de la distribución. La anchura del "violín" indica dónde se agrupan más los datos, mientras que en los extremos la densidad es menor.
</p>
<br>
<p align="left">
  - Variabilidad:
La forma de la gráfica muestra que hay una variabilidad moderada en los volúmenes de ventas, con valores que van desde muy bajos hasta niveles más altos. Sin embargo, los datos tienden a concentrarse hacia la parte central, lo que sugiere que la mayoría de las ventas están en un rango medio.
</p>
<br>
<p align="left">
  - Valores Centrales:
La línea central dentro del "violín" corresponde al rango intercuartil, donde se encuentran el 50% de los datos más cercanos al valor central (la mediana). Este rango es estrecho, indicando que los valores centrales de ventas no varían mucho.
</p>
<br>
<p align="left">
  - Conclusión:
En resumen, la gráfica muestra que la distribución del volumen total de ventas en la región tiene una concentración clara en el centro, aunque existen valores extremos con menor frecuencia. Esto permite entender la dispersión y tendencia central de los datos, lo que es útil para analizar el comportamiento general de las ventas en la región seleccionada.
</p>

###

<div align="center">

![2 1](https://github.com/user-attachments/assets/ca1412b1-7f16-4343-892f-26f7314e689e)

</div>

###

<h2 align="left">2.2 Boxplot Comparativo de Precios entre Años</h2>

###

<p align="left">
  - Introducción:
La gráfica muestra la distribución del precio promedio de aguacates por región entre los años de 2015 a 2018. Se trata de una gráfica de cajas (boxplot) que muestra la dispersión de los precios en cada región a lo largo de esos años. Cada color representa una región diferente, lo que facilita la comparación entre ellas.
</p>
<br>
<p align="left">
  - Distribución y Variabilidad:
La gráfica muestra la distribución de los precios promedio de los aguacates por región. Las cajas representan el rango intercuartil y la mediana está marcada por la línea central. Los puntos fuera de la caja son valores atípicos. En general, los precios se concentran alrededor de la mediana, con algunas regiones como California mostrando precios más altos y otras como Great Lakes más bajos y estables.
</p>
<br>
<p align="left">
  - Tendencias y Patrones:
En 2017, la variabilidad de precios fue mayor en muchas regiones, lo que puede haber sido causado por factores externos como cambios en la producción o la demanda. En 2015 y 2018, los precios fueron más constantes, lo que indica menos fluctuación.
</p>
<br>
<p align="left">
  - Conclusión:
Este análisis nos da una visión detallada de cómo el precio promedio de los aguacates ha variado no solo en el tiempo, sino también dependiendo de la región. Esto es útil para prever futuras tendencias en el mercado y tomar decisiones basadas en cómo los precios se comportan en diferentes zonas del país.
</p>

<div align="center">


![2 2](https://github.com/user-attachments/assets/dae79714-fed6-457e-89a3-35f5119d8b3c)

</div>

###

<h2 align="left">2.3 Gráfico de Líneas de Precios Promedios por Año</h2>

###
<p align="left">
  - Tendencia:
- 2015: El precio promedio comienza alrededor de 1,425.
<br>
- 2016: Hay una ligera caída del precio promedio, bajando a aproximadamente 1,385.
<br>
- 2017: Se produce un pico importante, donde el precio sube abruptamente hasta alrededor de 1,560, el valor más alto en toda la gráfica.
<br>
- 2018: El precio vuelve a descender, situándose alrededor de 1,400.
<br>
</p>
<br>
<p align="left">
  - Subida de precios de 2016 a 2017:
El aumento drástico del precio promedio en 2017 podría deberse a diferentes factores económicos o específicos del mercado, tales como:
<br>
  - Mayor demanda internacional: El auge del consumo de aguacates en mercados como Estados Unidos y Europa, impulsado por tendencias de alimentación saludable.
  <br>
  - Tendencias de consumo saludable y dietas que promueven el aguacate (como la dieta keto o vegetariana) pudieron impulsar la demanda.
<br>
  - Costos externos: Incrementos en costos de transporte, producción y fluctuaciones en el tipo de cambio, encareciendo las exportaciones.
  <br>
<p align="left">
  - Bajada de precios de 2017 a 2018:
La caída de precios pudo explicarse por:
  <br>
  - Aumento en la oferta: Mejoras climáticas y expansión de áreas de cultivo permitieron una producción mayor y más estable.
  <br>
  - Corrección del mercado: Después del pico de 2017, el mercado se ajustó, eliminando factores especulativos y reduciendo precios.
  <br>
  - Reducción de la demanda: Los altos precios de 2017 pudieron haber disminuido el consumo, llevando a una caída en la demanda en 2018.
  <br>
</p>
<br>
<p align="left">
  - Conclusión:
En conclusión, mientras que el incremento de 2016 a 2017 fue impulsado principalmente por un desequilibrio entre oferta y demanda, la caída de 2017 a 2018 estuvo relacionada con la corrección del mercado y una mayor producción que equilibró la oferta.
</p>
<br>
<div align="center">


  ![2 3](https://github.com/user-attachments/assets/ec55f53b-cb00-4074-ba3e-31e800bcd153)

</div>

###

<h1 align="left">3. Elasticidad del precio</h1>

###

<h2 align="left">3.1 Comparación de Elasticidad en Diferentes Mercados</h2>

###

## Título
**Elasticidad Precio-Demanda por Región**

---

## Introducción
- La **elasticidad precio-demanda** mide cómo cambia la **demanda** cuando varía el **precio**.
- **Valores negativos** son normales, ya que, al subir el precio, la demanda tiende a bajar.
- **Objetivo de la gráfica**: Comparar la elasticidad promedio en tres regiones:
  - **Spokane**
  - **Hartford-Springfield**
  - **New York**

---

## Explicación de la Gráfica
- En el **eje X** se representan las **regiones**.
- En el **eje Y** están los **valores de elasticidad promedio** (negativos).
- Las barras muestran:
  - **Spokane** ≈ **-35**
  - **Hartford-Springfield** ≈ **-55**
  - **New York** ≈ **-58**

---

## Interpretación de Resultados
- **Spokane**:
  - Elasticidad promedio ≈ **-35**
  - La demanda es **poco sensible** a los cambios de precio.
  - Puede significar que hay **menos alternativas** o que el producto es **esencial** en esta región.
- **Hartford-Springfield**:
  - Elasticidad promedio ≈ **-55**
  - La demanda es **más sensible** que en Spokane.
  - Los consumidores **reaccionan más** cuando cambia el precio.
- **New York**:
  - Elasticidad promedio ≈ **-58**
  - Es la región **más elástica**, con la mayor sensibilidad al precio.
  - Sugiere un mercado **más competitivo** o con **mayores sustitutos** disponibles.

---

## Comparación entre Regiones
| **Región**                | **Elasticidad Promedio** | **Sensibilidad**       |
|---------------------------|--------------------------|------------------------|
| **Spokane**               | -35                      | Baja sensibilidad      |
| **Hartford-Springfield**  | -55                      | Sensibilidad moderada  |
| **New York**              | -58                      | Alta sensibilidad      |

---

## Conclusión
- **New York**: La demanda es más **sensible** debido a una mayor **competencia** o **sustitutos** disponibles.
- **Spokane**: La demanda es **menos sensible**, mostrando **estabilidad** ante cambios de precios.
- **Hartford-Springfield**: Se encuentra en un **punto intermedio**.

### Reflexión Final:
- Las regiones con **alta elasticidad** (como **New York**) deben tener estrategias de precios cuidadosas, ya que un aumento significativo podría reducir la demanda.
- En regiones con **baja elasticidad** (como **Spokane**), los consumidores son **menos reactivos** al precio, lo que sugiere un **mercado más estable**.
###
<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###

<h2 align="left">3.2 Análisis de Elasticidad Comparativa entre Orgánicos y Convencionales</h2>

###

# Elasticidad Precio-Demanda por Tipo de Aguacate

---

## 1. Introducción: Contextualización
- **Inicio**:  
  En esta gráfica estamos analizando la **elasticidad precio-demanda** para dos tipos de aguacate: el **convencional** y el **orgánico**.  
  La elasticidad precio-demanda mide cómo **reacciona la cantidad demandada** de un bien cuando **cambia el precio**.

- **Definición breve**:  
  - Si la elasticidad es **negativa**, significa que al aumentar el precio, la demanda **disminuye** (bien normal).  
  - Si es **positiva**, indica que al aumentar el precio, la demanda también **aumenta** (bien Giffen o de lujo).

---

## 2. Descripción de la Gráfica
- **Ejes**:  
  - En el **eje X** (horizontal) se encuentran los dos tipos de aguacate: **convencional** y **orgánico**.  
  - En el **eje Y** (vertical) se representa la **elasticidad promedio**.

- **Barras**:  
  - La **barra verde** representa la elasticidad promedio del aguacate **convencional**.  
  - La **barra naranja** representa la elasticidad promedio del aguacate **orgánico**.

---

## 3. Análisis de Resultados
- **Elasticidad del aguacate convencional** (barra verde):  
  - Observamos que tiene un valor **negativo**, aproximadamente **-6**.  
  - Esto indica que el aguacate convencional tiene una **alta elasticidad negativa**, es decir, es **muy sensible** a los cambios en precio. Si el precio sube, la demanda cae drásticamente.

- **Elasticidad del aguacate orgánico** (barra naranja):  
  - Por otro lado, el aguacate orgánico presenta una elasticidad **positiva** cercana a **4.5**.  
  - Esto indica un **comportamiento opuesto**, ya que al subir el precio, la demanda **aumenta**, lo que sugiere que se percibe como un **bien de lujo** o exclusivo.

---

## 4. Interpretación de los Resultados
- **Comportamiento del Consumidor**:  
  - El aguacate **convencional** es un producto básico con alta elasticidad negativa porque los consumidores pueden buscar alternativas si el precio sube demasiado.  
  - Por el contrario, el aguacate **orgánico** podría representar un **bien de lujo**, ya que los consumidores están dispuestos a pagar precios más altos, posiblemente por sus características percibidas de **salud, sostenibilidad o exclusividad**.

- **Importancia Económica**:  
  Esto es crucial para los productores y vendedores. Si quieren ajustar precios, deben tener en cuenta que:  
  - Un aumento en el precio del aguacate **convencional** puede reducir sus ventas **significativamente**.  
  - Un aumento en el precio del aguacate **orgánico** podría incluso **aumentar su demanda**.

---

## 5. Cierre y Conclusión
- **Conclusión General**:  
  En resumen, esta gráfica muestra que los consumidores responden de manera **muy diferente** al precio según el tipo de aguacate.  
  - El aguacate **convencional** tiene una **alta elasticidad negativa**.  
  - El aguacate **orgánico** presenta una **elasticidad positiva**, típica de productos percibidos como lujosos o exclusivos.

- **Mensaje Final**:  
  Comprender esta diferencia puede ayudar a los productores y comerciantes a tomar **decisiones estratégicas** sobre precios y enfoques de mercado.

---
###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

<h2 align="left">3.3 Análisis de la Elasticidad Precios-Ventas</h2>

###

<p align="left">
### Elementos de la Gráfica

### **Eje X (horizontal):**
- Representa el **cambio porcentual en el precio**.  
- Valores **negativos** indican **disminuciones de precio**.  
- Valores **positivos** indican **aumentos de precio**.  

### **Eje Y (vertical):**
- Representa el **cambio porcentual en el volumen de ventas**.  
- Valores **más altos** indican un **aumento considerable en las ventas**.  
- Valores **bajos** indican **cambios menores o ninguna variación** en las ventas.  

### **Puntos Azules:**
- Cada punto muestra **cómo cambia el volumen de ventas** en relación con un **cambio en el precio**.  
- La **dispersión de los puntos** muestra la **variabilidad** de la relación entre precio y ventas.  

### **Línea Roja (tendencia):**
- Es una línea de **ajuste lineal** que resume la **tendencia general** de los datos.  
- Si la línea tiene **pendiente negativa**, indica una **relación inversa**:  
  - Al **subir el precio**, **bajan las ventas**.  
## Interpretación de la Gráfica

### **Tendencia General:**
- La **línea roja** parece tener una **pendiente ligeramente negativa**, lo que sugiere que **a medida que aumenta el precio**, el **volumen de ventas** tiende a **disminuir**.  
- Esta relación es típica en **bienes elásticos** donde la **demanda** responde a los cambios de precio.

### **Observaciones Dispersas:**
- La mayoría de los **puntos azules** están cerca de la **línea horizontal** (cambio porcentual de ventas ≈ 0).  
  - Esto indica que, en muchos casos, los **cambios en el precio** no tienen un gran impacto en las ventas.  
- Algunos puntos **muy elevados** (valores grandes en Y) representan **casos atípicos** donde un **pequeño cambio de precio** resultó en un gran aumento de ventas.

### **Cambios Negativos en Precio (Izquierda del eje X):**
- Cuando los **precios bajan**, se observan casos donde las **ventas aumentan significativamente**.  
  - Esto podría indicar que los **consumidores responden favorablemente** a las **reducciones de precios**.

### **Cambios Positivos en Precio (Derecha del eje X):**
- Al **aumentar los precios**, las **ventas** tienden a **mantenerse bajas** o **caer**.  
  - Este comportamiento respalda la idea de que la **demanda es sensible al precio**.

### **Conclusión General:**
- Existe una **relación inversa débil** entre el cambio en precio y el cambio en ventas:  
  - **Al subir el precio**, las **ventas** tienden a **disminuir**.  
  - **Al bajar el precio**, las **ventas** tienden a **aumentar**, aunque hay **mucha variabilidad en los datos**.  
- La **dispersión de los puntos** indica que hay otros factores además del **precio** que afectan las ventas.

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
