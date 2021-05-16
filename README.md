# Ejercicio de análisis de datos

El archivo adjunto [`datos.csv`](./datos.csv) contiene los registros de experimentos realizados con un grupo de microorganismos diferentes durante el año 2020.

Cada columna contiene los valores correspondientes a los parámetros y resultados codificados que se indican como encabezado de la misma.

El organismo está identificado por la columna `OrgID`.

La `Fecha` está indicada en el formato `dd/mm/aaaa`.

Todos los valores a partir de la cuarta columna (parámetro `P001_G`) son números positivos o valores en blanco.

Crear programas en Python para:

1. Obtener una lista de los diferentes organismos utilizados.

2. Sumar, para cada microorganismo, los totales de los parámetros `PG` y `PX`. Los parámetros `PG` se refieren a las columnas que inician con la letra `P` y terminan en `_G`. Los parámetros `PX` se refieren a las columnas que inician con `P` y terminan con `_X`. Los nombres de las columnas no deben codificarse de manera estática en el programa, sino que el mismo programa debe generar la lista de los parámetros que pertenecen a cada categoría. ***Tip***: La clase `str` posee métodos `.startswith` y `.endswith`... o puede, simplemente, usarse *slicing*.

3. Crear una gráfica del resultado `D002` contra el parámetro `P001_G`.

4. Extraer, para el `OrgID=220`, la información de los registros que presentan valores (diferentes de cero) para las columnas `PX`. Excluir de este análisis el parámetro (columna) `P005_X`. Reportar la fecha y los valores individuales de los parámetros `PX` (`P001_X`, `P002_X`, `P003_X`, etc.), así como el total `PX`.

Para trabajar con el ejercicio, puedes [clonarlo de GitHub](https://github.com/jz-ayp/ejercicio-analisis-datos.git) o [descargar solo el archivo de datos](./datos.csv).
