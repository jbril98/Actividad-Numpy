# Actividad-Numpy

Análisis de 4 indicadores de libre elección en 3 catálogos de datos diferentes.

Indicadores usados para el primer archivo de datos:
    - Orden de los diferentes pueblos de menor a mayor según el crecimiento vegetativo.
    - Media de nacidos vivos por residencia materna
    - Número máximo de muertes fetales tardías por residencia materna
    - Desviación típica de matrimonios por el lugar en el que han fijado la residencia
    
Indicadores usados para el segundo archivo de datos:
    - precio máximo de una vivienda
    - municipio que se repite más veces 
    - calles que empiezen con la letra "A"
    - La tasa de capitalización ordenada de menor a mayor
    
Indicadores usados para el tercer archivo de datos:
    - mayor government expenditure en cualquier año
    - government expenditure ordenado de mayor a menor
    - menor government expenditure en cualquier año 
    - media de government expenditure 
    
He análizado todos estos índices usando únicamente la librería Numpy. Además he usado la librería matplotlib para hacer 3 gráficos.
Los pasos seguidos para el análisis han sido los siguientes:

1º He descargado los datos de los 3 catálogos en un archivo .csv
2º He cargado los datos. Había distintas formas de cargar los datos:
     - mediante la función np.genfromtxt. 
     - mediante la función np.loadtxt.
     - mediante un with. Esta última ha sido la que mejor me ha funcionado
     
Me he encontrado problemas en cuanto a la carga de datos. Esto se debe a que Numpy suele trabajar con números y en los datos aparecían cadenas de strings. Pero finalmente probando diferentes parámetros y maneras he conseguido cargarlos exitosamente.

3º He usado varias funciones que nos sirven para analizar la matriz de datos y ver las características del dataset que tenemos para poder trabajar mejor con los datos:
print(data.shape)
print(data.size)
print(data.ndim)
print(data.dtype)

4º He calculado los indicadores usando Numpy.
5º He generado algunas gráficas que nos ayudan a interpretar los datos.
