# REPOSITORIO GIT PARA LA CLASE TC1002S
Repositorio para alojar los ejercicos, prácticas y tareas a realizar 
en el curso de Herramientas Computacionales: El arte de la analítica,
en el Tec de Monterrey campus Sonora Norte.  
Silvana Dorita Ruiz Olivarría   
A01252346  
## ESTUDIANTES EQUIPO 4 
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
Manual de Mapa de Calor y Boxplots  
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
