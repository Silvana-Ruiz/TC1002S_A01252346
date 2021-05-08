# REPOSITORIO GIT PARA LA CLASE TC1002S
Repositorio para alojar los ejercicos, prácticas y tareas a realizar 
en el curso de Herramientas Computacionales: El arte de la analítica,
en el Tec de Monterrey campus Sonora Norte.    
## Estudiante  
Silvana Dorita Ruiz Olivarría   
A01252346  
## EQUIPO 4 
Silvana Dorita Ruiz Olivarria  
Randy Oliver Ortega Cota  
Luis Rodolfo Bojorquez Pineda  
Sebastian Galvez Trujillo  

## MATRICULAS
A01252346  
A00232304  
A01250513  
A01251884  

## LISTADO DE EJERCICIOS

### Manual de Mapa de Calor y Boxplots  
Para poder corer el programa primeramente se debe clonar el repositorio TC1002S_A01242346 al presionar el botón verde en Github llamado “Code”. Este desplegará una serie de opciones, se debe proseguir a copiar el URL. Posteriormente en una terminal de computadora Mac o en una terminal Linux, o en caso de contar con sistema operativo Windows, en una Virtual Box con Ubuntu descargado se abre una terminal de Linux. En esta se debe hacer posicionar con el comando cd en la carpeta deseada para posicionar la carpeta del repositorio. Después, se escribe el comando git init y se da enter. Posteriormente, se usa git remot add origin y se pega el URL copiado, se le da enter. Ahora, se debe escribir jupyter notebook y darle enter. Esto abrirá la carpeta que fue copiada en el navegador. Ahora se debe elegir el archivo de MapasDeCalorBoxplots.ipynb. Para correrlo, solo se debe presionar el botón en la esquina derecha de “Run”. Primero se importa las librerías a utilizar, con la import, las cuales son pandas como pd, matplotlib.pyplot como plt y seaborn sns. Posteriormente, se lee el archivo csv “Pace of life.csv”, el cual contiene los datos a trabajar, mediante la función pd.read_csv y se crea un dataframe cuyo nombre es datapf. A continuación, se realizan los boxplots para representar los rangos de las variables numéricas, esto se hace con la función plt.figure para indicar el tamaño, .addaxes para indicar los axes y .boxplot para finalmente crear los bloxplot de valores del arreglo “item”. Después, se realiza el histograma de las variables numéricas con la función Counter, la cual cuenta la cantidad de apariciones de un dato, .bar la cual es responsable de hacer las gráfica e indica detalles de esta, .xticks, .xlabel, .ylabel, .title muestran el formato. Finalmente, .show lo muestra. Con .corr se realiza la matriz para hacer el heatmap, el cual se hace con la función .heatmap y la librería sns.  
Interpretación  
¿Hay alguna variable que no aporta información?  
Este análisis depende de una muy pequeña cantidad de variables por lo que, todas proveen información necesaria para llegar a una conclusión.  
Si tuvieras que eliminar variables, ¿cuáles quitarías y por qué?  
Si fuera necesario eliminar variables, la que quitaría sería la denominada como “Talk” ya que es influenciada por más factores que las otras variables, como el estado de ánimo de la persona, su dominio en el tema y su carácter. Otra opción sería quitar en vez de “Talk” la de “Bank” ya que en el boxplot de esta se puede apreciar que hay un outlier muy lejano de la media y en el resto de los casos no sucede lo mismo.  
¿Existen variables que tengan datos extraños?  
No se percibieron variables con datos extraños a simple vista. Sin embargo, en los boxplots se puedo apreciar que en el de Bank había un outlier representando un tiempo muy bajo a comparación del resto.  
Si comparas las variables, ¿todas están en rangos similares? ¿Crees que esto afecte?  
Todas las variables numéricas están en rangos similares salvo “Bank”. El efecto que se puede tener es que el ritmo de vida de un lugar sea descrito un poco más lento de lo que realmente es, ya que “Bank” mide el tiempo; por lo que, si tiene un rango con un máximo mayor que el del resto, significa que el ritmo es más lento.  
¿Puedes encontrar grupos que se parezcan? ¿Qué grupos son estos?  
Si “grupos” se refiere a filas, es posible encontrar grupos que se parezcan ya que todos son muy similares. Unos ejemplos son Rochester y Kansas City, y Chicago y Younstown. En cambio, si estos se refieren a columnas, las similares son “Walk”, “Talk” y “Heart”.  

## MANUAL de Actividad K-means:   
Descargamos la el código de github y descomprimimos la carpeta .zip   
Ingresar los archivos a nuestra carpeta de nuestra preferencia.  
Abrimos la terminal e ingresamos el comando ‘jupyter notebook’ para utilizar nuestros archivos en jupyter.  
Dentro de jupyter entramos a la carpeta K-Means y abrimos el archivo K_Means.ipynb, aquí ya podemos correr nuestro código de pyhton3.   
Seleccionamos la primera celda y damos CTRL+ENTER para correrla. En el código, empezamos nuestras líneas de código importando todas nuestras librerías que nos permitirá trabajar con nuestra base de datos, como matplotlib.pylab, sklearn, numpy, pandas y seaborn. Luego se lee el documento csv  “Child smokers.csv” con la función de panda pd.read_csv, se genera un marco de datos y es nombrado "data". Posteriormente, se utilizan varias funciones, primero, “.shape” sirve para saber el número de filas y de columnas que tiene el data frame, “.columns” da el título de las columnas.  También se usa “.dtypes” para identificar los tipos de datos con los que se trabaja. Por último, se emplea “.describe” para generar una tabla que da información general de los datos, por ejemplo, el promedio por columna, desviación estándar, máximos y mínimos, etc. Estas funciones son principalmente para asegurar que no hay errores en la base de datos y que es posible trabajar con la misma. Asimismo, antes de poder pasar los datos por el algoritmo K-Means fue necesario normalizar nuestros datos entre valores de 0 a 1 la función MinMaxScaler() de la librería de sklearn.preprocessing. Con esta función se logra hacer que en los datos,  el valor más grande de cada variable se convierta a uno y el más chico a cero, y todos los valores intermedios les da un valor entre cero. Consiguientemente, se usan los datos anteriores ya normalizados para pasarlo por el algoritmo K-Means. Se declara el número de clusters a utilizar, en este caso k = 3, y posterioremnte con la función .cluster_centers se geenran tres vectores (ya que k es igua a 3) con 5 datos cada uno, cada dato representa una variable de las utilizadas en el análisis. Estos datos que se encuentran en los vectores son llamdos centros, los cuales dan información respecto a cómo es que influye la variable a la que corresponde dicho centro en la cantidad de clusters (indica si se necesitaban más clusters  o no).
