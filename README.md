# Estimaciones-Agricolas
Proyecto Nº1- Data Science

INTRODUCCION 

Estimaciones Agrícolas es un documento que continene una serie de estadísticas agrícolas por cultivo, municipios e
inversiones tanto locales como extranjeras. 

OBEJTIVO:
 * Conocer las plantaciones más efectivas.
 * Identificar futuras inversiones.
 * Detectar localidades en territorio argentino para la siembra.

Para lograr cumplir el objetivo, se plantearán situaciónes en gráficos para tener de manera visual lo que queremos
exponer. Al implementar nuestra base de datos lograremos mostrar la cantidad de municipios donde la tierra es fértil para
cosechar. El detectar tanto las zonas cosechadas nos abrirá el conocimiento de dónde se podrá invertir en el corto plazo,
como así también qué tipo de semillas utilizar.

BIBLIOTECA 
* www.argentina.gob.ar/buscar/datasets

DICCIONARIO
Cultivo_nombre: Tipo de cultivo a cosechar en suelo Argentino.
Municipio_nombre: Nombre de cada municipio donde se cosecha. País Argentina.
Superficie_sembrada: Se refiere al área efectivamente sembrada o cubierta por
semilla durante el año calendario, el cual se extiende del 1 de enero al 31 diciembre.
Superficie_cosechada: Superficie de la cual se recoge un cultivo, puede que no toda la superficie haya sido efectivamente
cosechada.
Producción: Es el numero estimado en toneladas efectivamente brindadas.
Rendimiento: Es el importe que nos ha generado ganancia positiva.
Origen_empresa: Define a grandes rasgos la cantidad de empresas que invierten locales/extranjeras, y Nueva Zelanda, nuevo inversor.
Empresa_id: Identificador único del origen de la empresa que invierte en suelo argentino
Inversion_moneda: Define la moneda que ingresa a la Argentina, sean en Pesos Argentinos/Dolares Americanos/Dolares Neozelandeses.
Inversion_Divisa USD: Conversión en dolares americanos del monto en pesos argentinos invertidos, u otra moneda.
Year_fecha: Rango de fechas, en este caso se toman 2 años consecutivos para el análisis
Productor_nombre: Productor que invierte en suelo Argentino, de residencia local o extranjera.
Inverion_moneda: Tipo de moneda que invierte cada productor
Roi_porcent: Muestra el porcentaje del rendimiento obtenido en cada cultivo, ya sea negativo o positivo.


Contexto Comercial
Este modelo puede ser utilizado para empresas de la agroindustria, tanto para la plantaciòn de semillas a utilizar para futuras inversiones, como tambièn identificar terrenos para potenciar la cosecha en territorio argentino. Lo cual terminarà en un gran contexto pues se ampliarà la mano de obra generando ofertas locales, y asì atraer mas inversiones al paìs de origen.

Contexto Analìtico: Se utilizarà un modelo de regresiòn para predecir futuras inversiones para el tipo de semillas a cultivar.

MEDIDAS DESCRIPTIVAS

DISTRIBUCION DE DATOS


1º GRAFICO podemos ver un listado de todo el dataset con el que vamos a trabajar nuestro anàlisis de proyecciones agrìcolas. Que son las proyecciones agrìcolas? Este es un dataset bajado de una web del estado pùblica y con datos modificados, tomando en cuenta los ùltimos 2 años de varios municipios del territorio argentino, donde analizamos los cultivos mas comunes, por ejemplo Soja, Ajo, Cebada... entre otros.
Detectar zona de cultivo/ tipo de cultivo/ origen de inversiones nos permitirà ver en dònde estamos trabajando actualmente y què puntos podemos mejorar para atraer mas inversores en zonas de menor inversiòn, previendo los riesgos que conlleva cada localìa y tambien por supuesto las ganancias que estas generaràn.

2º GRAFICO Reducimos la planilla en 5 columnas para poder ver los cultivos/ Municipios y poder visualizar el origen de las inversiones por empresa. Estas son Locales (es decir de Argentina) y Extranjeras.

3º GRAFICO Nos interesa ver la media y promedio del total de la superficie cosechada, junto a la inversiòn. Gracias a estos datos podemos detectar las zonas de mayor impacto en inversiones con la moneda dolar estadounidense. En cuanto a la superficie, nos permite detectar el radio de municipios donde podemos concentrar mejores inversiones y trabajar en pos de ello.
Esto lo veremos mas abajo en los gràficos de Histogramas

4º GRAFICO Veremos la distribuciòn de la Inversiòn en la divisa USD.

5º GRAFICO Se despliega la lista de Productores

EDA

En Este analisis podremos ver el top 10 de cultivos más utilizados en las localidades que han resultado más fructìferas. Posterior veremos las variables de las superficies cosechadas y sembradas, como referencia para la futura toma de decisiones. En base a esto, detectamos què localidad rinde más para cierto cultivo. Con este resultado se podrà trabajar en más inversiones para la zona.

6º GRAFICO encontramos el top 10 de cultivos mas utilizados con la comparativa de los municipios donde se han sembrado mas.

7º GRAFICO vemos la relaciòn que hay entre todas las variables de nuestro dataset.

8º GRAFICO los histogramas de caracterìsticas del dataset. Posterior se realiza una limpieza de dicho dataset, para llegar a una agrupaciòn pequeña donde podemos observar que la mayor parte de los cultivos se encuentra en algunos municipios especìficos.

En la ùltima codificaciòn implementamos regresiòn lineal usando mètricas para evaluar el rendimiento de nuestro dataset.

CONCLUSIÒN

Al implementar un dataset de Estimaciones Agrìcolas en el territorio Argentino pudimos identificar - separar- y actuar sobre los resultados arrojados a lo largo del anàlisis, cumpliendo el objetivo previamente propuesto.
Los resultados arrojaron que las plantaciones màs efectivas en nuestro territorio son la Cebada Cervecera, Centeno, Trigo Total. Siendo las mejores localidades para trabajar el suelo: Guamina, Hipolito Yrigoyen Junin.
Con esto en vista el Estado Argentino como mayor productor agrìcola e inversor podrà hacer los càlculos necesarios para mejorar el estado de las maquinarias - mano de obra- sueldos.. etc. Y potenciar las localidades mas bajas para armar nuevos proyectos y atraer inversores extranjeros. 
Se entiende que las localidades con menor inversiòn tienen conflictos de suelo bien llamados. Podemos acudir a las inversiones extranjeras para generar una limpieza de tierra y testear nuevos cultivos para su desarrollo.
Cuando realizamos el calculo de "MSE" vemos que el valor arrojado 1.620 es cercano a 0 por lo tanto estamos hablando pràcticamento de un anàlisis sin error.  En la R2 que arrojò 1.0 se denota la variaciòn de los datos entre x e y que son idènticas. 
Por lo tanto, podemos seguir proyectando los pròximos años en base a este anàlisis y prueba que el sector agrìcola irà creciendo y brindando oferta laboral y mejoras en la economìa Argentina.


OBEJTIVO:
 * Conocer las plantaciones más efectivas.
 * Identificar futuras inversiones.
 * Detectar localidades en territorio argentino para la siembra.



