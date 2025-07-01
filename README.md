# Challenge_TelecomX
Proyecto de análisis de datos de una empresa de telecomunicaciones (analisis churn)

1.- PROPOSITO

Realizar un Análisis churn para encontrar las posibles causas de la alta cancelación de los contratos de servicio de la empresa TELCOM. Proponer soluciones para evitar el churn.

2.- ESTRUCTURA DEL PROYECTO 

El proyecto está ordenado por 5 Puntos importantes:
	Comprobación de incoherencias en los datos:
		El cual es la extracción de los datos y a su vez localizar casillas con información nula que pueda afectar en el libre análisis o transformación del tipo de dato de las columnas. Por lo que se realiza la busque da de elementos vacíos en la columna tenure, ya que se localizó casillas vacias que no permiten modificar el tipo de dato.

	Una vez eliminadas esas 11 filas, se busca elementos vacíos en la columna churn para poder analizarla y dependiendo del tipo de datos se le dé un valor para poder ser analizado. valor 0 por si el cliente continua con el contrato y 1 si el cliente cancela el contrato.

PREPARACION DE DATOS
	En esta parte, convertimos la información de ciertas columnas en 1 y 0 para poder ser utilizados en cálculos mas adelante, las columnas modificadas son Churn, Partner, Dependents, Phone service. 

	En mi caso, yo no creí necesario las columnas CustomerID y PaperlessBilling por lo que fueron eliminadas para cuestiones de análisis de información.

	De igual forma como requerimiento del mismo proyecto, se creo la columna 'Cuentas_Diarias el cual posteriormente se utiliza.

	Ya teniendo todo esto ordenado, se realiza un análisis descriptivo de la tabla de datos, el cual se analizan las cols: Churn, tenure, Monthly, Total y Cuentas_Diarias para conocer cuantos datos tenemos, los tipos de datos, sus máximos y mínimos, ya que esas estadísticas nos servirán para el planteamiento de los cálculos posteriores.

DISTRIBUCIÓN DE EVASIÓN

	En esta parte se comienza el análisis de las distintas columnas:

- Demostrar el porcentaje de churn.
- Si el cliente que cancelo contrato contaba con linea telefónica, internet, que tipo de internet (DSL o Fibra Optica) o si contaba con soporte técnico.
- De igual forma en el estudio socioeconómico saber que porcentaje de gente cancelo contrato, esto analizando las columnas, Tipo de Contrato, Tipo de Pago, si es retirado o no, si esta casado, soltero y si tiene o no hijos. Con base a esta info ver que características tienen los clientes que mas índice de churn tienen.
- Otro análisis es el tipo de contrato y formato de pago para revisar quienes son los que cancelan mas.

CONTEO DE EVASION POR VARIABLES NUMERICAS.

En esta parte, como continuación de análisis de información se hicieron agrupaciones de datos para saber, en que bloque de info había mas casos de cancelación, el primero fue hecho para la cantidad de meses que llevaba el cliente y el segundo para el total que había gastado en todo el tiempo de su contrato, así también se analizó el costo diario y cual era el gasto diario que tuvo mas cancelaciones de servicios

CANTIDAD DE SERVICIOS CONTRATADOS VS PROBABILIDAD DE CHURN

Este análisis fue para confirmar que dependiendo de la cantidad de servicios contratados, ligado a la cantidad de cuota, convertia en un costo muy alto que se veía reflejado en la cancelación de contratos debido al costo elevado que se convertía el servicio general.

CORRELACIÓN DE VARIABLES.

Este punto fue requerido como parte fundamental del proyecto donde por medio de código se requiere una correlación de la columna CHURN con las demás columnas para encontrar relaciones que puedan ayudar al análisis de todo el proyecto.

INFORME FINAL

En esta parte se describen los resultados, así como las conclusiones del análisis de la información así como sus posibles soluciones o modificaciones.



3.- INSIGHTS OBTENIDOS.

Estos están descritos en la parte final del notebook, favor de leer el texto al final del notebook del código. De igual forma las descripciones y graficos de los distintos cálculos se encuentran en ese link

4.- INSTRUCCIONES PARA EJECUTAR NOTEBOOK

1.- descargar notebook
2.- Abrirlo en el ambiente Colab y seleccionar donde guardarlo
3.- Abra el notebook en Colab y dar clic en botón conectar y después ejecutar todo.
4.-Una vez ejecutado revisar los resultados de cada perfil.
