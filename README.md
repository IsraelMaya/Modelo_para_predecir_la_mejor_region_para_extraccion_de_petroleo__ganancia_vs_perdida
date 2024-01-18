## ¿Que región da más fiabiliadad para extraer petroleo y que las ganancias supere a las pérdidas?

Trabajamos para la compañía minera OilyGiant. El objetivo es encontrar el mejor lugar para un nuevo pozo utilizando los siguientes pasos para elegir la ubicación:

    * Recolectar los parámetros del pozo de petróleo en la región seleccionada: calidad del petróleo y volumen de reservas
    * Construir un modelo para predecir el volumen de reservas en los nuevos pozos
    * Seleccionar los pozos de petróleo con los valores estimados más altos
    * Elige la región con el mayor beneficio total para los pozos de petróleo seleccionados.
    
Para ello, se nos dan los datos sobre muestras de crudo de tres regiones. 

Ya se conocen los parámetros de cada pozo petrolero de la región, por lo que vamos a crear un modelo que ayude a elegir la región con el mayor margen de beneficio, tomandose a consideración que, una unidad de producto es igual a 1000 barriles, donde cada barril representa 4.5 USD de ingresos, por lo que una unidad representa 4,500 USD de ingresos, y el presupuesto para el desarrollo de 200 pozos es de 100 millones de USD.

Al final se analiza los beneficios y riesgos potenciales **utilizando la técnica bootstrapping** de 1000 muestras y con un **intervalo de confianza del 95%**.

## Tabla de conteidos del proyecto

* [1 Incialización](#Capítulo_1)
    * [1.1 Cargar los datos](#Sección_1_1)
* [2 Exploración datos iniciales](#Capítulo_2)
    * [2.1 División y codificación de los datos](#Sección_2_1)
* [3 Formulación del cálculo de ganancias](#Capítulo_3)
* [4 Bootstraping](#Capítulo_4)
* [5 Conclusión](#Capítulo_5)


## Paqueteria Utilizada

`pandas`
`numpy`
`matplotlib.pyplot`
`scipy - stats` 
`sklearn` 

## Resultados
Se encontró que de las tres regiones analizadas, la **región 1** es la que da una mejor fiabilidad para hacer la extracción de petroleo en 200 pozos, dado su **bajo RECM** y también a que **se predice un mayor voluemn de reservas**.

Dada la **inversión de 100 millones de USD**, se espera que **en promedio la ganancia por pozo sea 4,537,178.95 de USD** con un **riesgo del 1.6%**, lo cual le puede dar mucha confianza a la empresa `Oily Giant` de relizar su extración en la región 1. 


