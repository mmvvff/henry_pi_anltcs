# Henry: Proyecto Individual Análisis de datos
*Contexto.* Este proyecto responde a las consignas establecidas por la organización Henry como parte del segundo proyecto individual: [Análisis de datos](https://github.com/soyHenry/PI_DA).

## Motivación
Algunos especialistas argumentan que las criptomonedas tiene el potencial de constituir una divisa que se podría incorporar en un portafolio de inversión. Este argumento se basa en el potencial de algunas criptomonedas para actuar como depósitos de valor. De esta manera, las criptomonedas adquieren propiedades de diversificación, convirtiéndolas en candidatas ideales para ser incorporadas en portafolios de inversión.

Estas propiedades de las criptomonedas ha llamado la atención de inversionistas en países latinoamericanos. En estos países, familias se han enfrentado a una alta volatilidad en la tasa de cambio de sus monedas locales, junto con niveles elevados de inflación. Esto plantea retos para las familias latino-americanas que poseen activos líquidos en moneda local, como por ejemplo, ahorros. En este contexto, algunas familias de estos países generalmente aprovechan la estabilidad cambiaria del dólar estadounidense (USD) para construir un portafolio de divisas con el fin de reducir su exposición a la volatilidad de las monedas locales y a la inflación local. Pero dada la apreciación del dólar, las criptomonedas también suenan como potenciales candidatas para ser incorporadas en dichos portafolios de inversión.

No obstante, la volatilidad inherente del mercado de criptomonedas también ha generado varias alertas que limitan su incorporación en portafolio de divisas. Por lo tanto, surge la necesidad de obtener claridad con respecto al potencial de las criptomonedas en un portafolio de divisas que busque disminuir la exposición a la volatilidad de las monedas local en contextos de elevados niveles de inflación local, como es el caso de los países latino-americanos.

Con base en lo anterior, surgen las siguientes preguntas:
- Primero **(P1)**, ¿cuáles son las criptomonedas que evidencian una mayor volatilidad y cuáles una menor volatilidad?
- Segundo **(P2)**, Desde el punto de vista del contexto local de los países latino-americanos, ¿se intensifica la volatilidad del mercado de criptomonedas?

## Objetivos y métodos
En esta sección, planteamos los objetivos (p. ej., O1) para dar respuesta a las dos preguntas que orientaran nuestro análisis (p. ej., P1.O1).

**(P1)** ¿cuáles son las criptomonedas que evidencian una mayor volatilidad en relación con la volatilidad inherente del mercado?
- P1.O1.: Medir la volatilidad de cada criptomoneda en relación con la volatilidad de otras criptomonedas.
- P1.O2.: Identificar las criptomonedas relativamente más volátiles y las menos volátiles.

**(P2)** Desde el punto de vista del contexto local de los países latino-americanos, ¿se intensifica la volatilidad del mercado de criptomonedas?
- P2.O1.: Medir la volatilidad de las criptomonedas en una selección de países latino-americanos, controlando por cambios en la inflación y ajustando los precios para que reflejen una paridad en el poder adquisitivo.
- P2.O2.: Comparar la magnitud de la volatilidad entre países y explorar diferencias o similitudes entre contexto locales; es decir, explorar si la volatilidad aumenta en países latino-americanos en relación con un país de referencia (EEUU).

## Desarrollo y hallazgos

Nos concentramos en dos grupos de criptomonedas con dos propiedades tecnológicas: monedas con autonomía tecnológica ([Layer 1](https://www.techopedia.com/definition/layer-1-in-blockchain)) y monedas cuyo valor esté vinculado a otro activo ([stablecoins](https://www.investopedia.com/terms/s/stablecoin.asp)). Consideramos necesario distinguir entre estos dos tipos de monedas dado su impacto en la volatilidad. 

Hacemos uso de una serie de indicadores para responder a nuestras preguntas. Primero, medimos la magnitud de la volatilidad de una moneda por medio del nuestro indicador (KPI) "Volatilidad relativa". Este indicador nos permite medir la magnitud de la volatilidad de una moneda en relación con la volatilidad promedio de otras monedas. De esta manera, si la "Volatilidad relativa" > 1, es relativamente volátil, mientras que si  la "Volatilidad relativa" < 1 es relativamente estable. Nuestro indicador nos permite clasificar las monedas según su volatilidad. En el grupo "Layer-1", bitcoin es la más volátil. Mientras que en el grupo "stable coins", la más volátil es pax-gold dado su vínculo con el oro, un recurso relativamente volátil en comparación a divisas como el USD. Encontramos que, en promedio, el grupo "stable coins" evidencia una menor variación en la volatilidad de sus miembros (monedas) que el grupo  "Layer-1"; esto sugiere que las monedas en grupo "stable coins" pueden ser un mejor candidatos para ser incluidos en portafolios de inversion.

Segundo, identificamos las monedas relativamente más estables por medio de nuestro "Índice estabilidad relativa". En resumen, el "Índice estabilidad relativa" es una métrica ponderada entre la "Volatilidad relativa" y del volumen de transacciones, donde le damos más peso al primero que al segundo. Incorporar el volumen de transacciones nos permite sugerir criptomonedas que no solo son relativamente estables, sino que también evidencien niveles relativamente alto de liquidez. Encontramos que "cardano" ("Layer-1") y "tether" ("stable coins") son las monedas relativamente más estables y con mayor potencial de liquidez; esto sugiere que son monedas con potencial de ser incluidas en portafolios de inversión.

Tercero, exploramos el comportamiento de criptomonedas en diferentes contextos locales. Nos concentramos en los cuatro países más grandes por población de Latino-América: Brasil, México, Argentina y Colombia. Incluimos como país de referencia a EEUU. Como era de esperarse, encontramos que la volatilidad del grupo de criptomonedas observado es más alto desde el punto de vista de países Latino-Americano con relación a EEUU. Esto recomienda que los inversionistas en países Latino-Americano debe ser más cautelosos al momento de incorporar criptomonedas en un portafolio de divisas, dado que la volatilidad se intensifica sustancialmente.

## Ejecución del proyecto
Desarrollamos el proyecto en 3 partes: i. Cargar y limpiar base datos, y generar subconjuntos de datos (ETL); ii. Examinar la naturaleza y composición de los datos (EDA); iii. Alimentar un dashboard en Tableau.

### 1. ETL
Esta fase incluye dos partes:
1. [Extracción de datos](data_process/01_etl_v7.ipynb).
2. [Limpieza y preprocesamiento de datos](data_process/02_etl_tranform_v2.ipynb).

### 2. [EDA](data_process/03_eda_v2.ipynb)
En esta fase, exploramos los datos con el fin de responder a nuestras preguntas.

### 3. Dashboard
Desarrollamos nuestro dashboard en Tableau Public.