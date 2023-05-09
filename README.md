Project_ETL 

![Captura](https://github.com/Lorensou/-w4-project_ETL/blob/main/img/Captura%20de%20pantalla%202023-05-09%20091502.png)

OBJETIVO DEL TRABAJO:

El principal objetivo de este trabajo es encontrar el surfista adecuado para promover una campaña publicitaria en instagram por parte de una compañia multinacional de gafas de sol.

Requerimientos por parte de la compañía:
    - El surfista debe estar en el top de la liga mundial de surfing (WSL)
    - El surfista debe tener una gran repercusión en Instagram.
    - La empresa quiere conocer tanto la edad como características físicas del surfista(peso y altura)

Una vez esta claro que datos quiere la empresa procedemos a realizar la búsqueda, extracción, transformación y carga de los datos.


ESTRUCTURA DEL PROYECTO

En la carpeta del proyecto se encuentra:
       
    - Carpeta csvs_limpios: donde se encuentran las dos tablas(df_prosurfers y df_surfers_ig) que hemos elaborado en formato csv.
    - Carpeta SQL: Contiene el acceso a las dos tablas importadas a MySQL y el diagrama ERR.
    - Carpeta img: Contiene 2 imagenes de las querys de selección de las tablas.
        - csv de Kaggle (de donde se ha importado la tabla de  los surfistas que obtuvieron más puntos wsl en el 2022)  
        - Las 2 Notebooks de Visual Studio Code, en las que se han importado los datos, limpiado, transformado y por ultimo pasado a csv.


PROCESO ETL

1) Busqueda de datos: 

    En primer lugar se han buscado las fuentes de las que extraer los datos. En este caso se ha tomado un archivo, con la información de los surfistas por puntos obtenidos en competición(wsl), de Kaggle. La segunda fuente ha sido la pagina oficial de la competición, WSL.com. Por último, para obtener datos sobre el instagram de los surfistas se ha tomado como fuente un blog que rankea a los surfistas con mayor influencia, https://blog.feedspot.com/surfing_instagram_influencers/.

2)Extracción de datos:
    Para la extracción de los datos se han empleado dos métodos, el primero ha sido la descarga directa del archivo de Kaggle en formato csv, y para las otras dos fuentes se ha empleado el método de scrapeo mediante selenium.

3) Limpieza y transformación:
    En primer lugar se han creado data frames mediante la libreria pandas, más adelante se ha procedido a eliminar las filas que contenian datos que no nos interesaban, por último se han limpiado las tablas y pasado a formato csv.

4) Carga a base de datos: 
    Por último se ha creado un diagrama ERR en la base de datos de MySQL con las columnas y características que presentan los datos de los df. Más adelante se han importado las tablas en formato csv, que anteriormente se habian descargado, a las tablas de la base de datos. Por ultimo se ha creado la relación entre las dos tablas.

FIN 
