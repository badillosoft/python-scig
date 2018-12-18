# python-scig
Curso de Python Científico versión 6

# Proyectos Finales

## Compresor de archivos (1pt)

Documentación:

https://www.tutorialspoint.com/python/os_walk.htm
https://docs.python.org/3/library/zipfile.html

1. Solicitar la ruta completa del directorio a comprimir
2. Obtener el nombre de todos los archivos usando `os.walk`
3. Abrir (crear) un archivo zip usando `zipfile`
4. Escribir cada archivo del directorio usuando `myzip.file(...)`
5. Cerrar el archivo zip
6. Descomprimir el archivo zip manualmente para comprobar la integridad

## Reporte pdf (1pt)

Documentación:

https://www.reportlab.com/docs/reportlab-userguide.pdf

Ver páginas 12, 13 y 14

1. Crear un archivo pdf
2. Crear un objeto canvas
3. Escribir un título y subtítulo en el documento en la parte superior al centro
4. Escribir la fecha y hora actual en la parte inferior derecha
5. Generar una gráfica cualquiera en matplotlib
6. Guardar la gráfica en un archivo usando `plt.savefig("g.png")`
7. Colocar la imagen "g.png" en el canvas
8. Guardar el documento pdf

## Consulta sql con pandas (1pt)

Documentación:

https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_sql.html

1. Definir la uri de conexión a la base de datos (`mysql://localhost/MyDB`)
2. Definir el query para recuperar la tabla (`select * from TABLE ...`)
3. Ejecutar el query en pandas con `pd.read_sql(...)`
4. Mostar los primeros registros del dataframe con `df.head()`


## Recolectar información del clima (1pt)

Documentación:

https://scrapy.org/

1. Visitar https://weather.com/es-MX/tiempo/hoy/l/MXDF0132:1:MX
2. Obtener los datos del clima (tamperatura, descripción, sensación, máx-mín, índice UV)
3. Guardar los datos en un archivo de texto `cdmx-XXXX` dónde `XXXX` es la fecha actual

## Buscador de archivos (2pt)

1. Solicitar el directorio raíz
2. Solicitar una palabra a buscar
3. Buscar todos los archivos y carpetas
4. Para los archivos de texto (`*.txt`) buscar la palabra solicitada en su nombre y en su contenido
5. Si la palabra coincide guardar la ruta del archivo en otro archivo de rutas encontradas (una por línea) y el número de caractér dónde se encontró y finalizó la coincidencia

## Geolocalización (2pt)

1. Solicitar una latitud y longitud
2. Solicitar otra latitud y longitud
3. Usar la ecuación para calcular la distancia geoespacial entre las dos coordenadas
4. Mostrar la distancia en `cm`, `m` y `km`.
5. Calcular el tiempo en `segundos`, `minutos` y `horas` que tardaría un peatón a `2km/h` y un auto a `60km/h` en recorrer la distancia anterior, por ejemplo:

~~~txt
Coordenada A: (19.414805,-99.1729187)
Coordenada B: (19.423203,-99.1657197)
Distancia: (11700000cm, 117000m, 1.17km)
Tiempo:
Peatón: (2106seg, 35.1min, 0.585h)
Peatón: (70.2seg, 1.17min, 0.0195h)
~~~
