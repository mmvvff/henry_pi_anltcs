# Henry: Proyecto Individual Análisis de datos
*Contexto.* Este proyecto responde a las consignas establecidas por la organización Henry como parte del segundo proyecto individual: [Análisis de datos](https://github.com/soyHenry/PI_DA).

## Motivación
Algunos especialistas argumentan que las criptomonedas tienen el potencial de constituir una divisa que podría incorporarse en un portafolio de inversión. Este argumento se basa en la cualidad de algunas criptomonedas para actuar como depósitos de valor. De esta manera, las criptomonedas adquieren propiedades de diversificación, convirtiéndolas en candidatas ideales para ser incorporadas en portafolios de inversión. Sin embargo, su volatilidad también ha generado alertas que dificultan su incorporación en dichos portafolios, especialmente entre inversionistas conservadores con baja tolerancia al riesgo.

En este contexto, la propiedad de diversificación de las criptomonedas ha llamado la atención de inversionistas conservadores en países latinoamericanos. En estos países, las familias de clase media se han enfrentado a una alta volatilidad en la tasa de cambio de sus monedas locales, junto con niveles elevados de inflación. Esto plantea desafíos para las familias latinoamericanas que poseen activos líquidos en moneda local, como por ejemplo, ahorros. En este contexto, algunas familias de estos países suelen aprovechar la estabilidad cambiaria del dólar estadounidense (USD) para construir un portafolio de divisas con el fin de reducir su exposición a la volatilidad de las monedas locales y a la inflación local. No obstante, debido a la depreciación de sus monedas locales frente al USD, las criptomonedas también parecen ser candidatas para ser incorporadas en dichos portafolios de inversión.

A pesar de ello, la volatilidad inherente del mercado de criptomonedas también ha generado diversas alertas que limitan su incorporación en un portafolio de divisas de inversionistas con un perfil conservador y con baja tolerancia al riesgo. La volatilidad del mercado de criptomonedas ha sido ampliamente documentada (ver [ref](https://jfin-swufe.springeropen.com/articles/10.1186/s40854-021-00321-6)) pero no está claro en qué medida varía la volatilidad entre una y otra criptodivisa, considerando la heterogeneidad en sus propiedades tecnológicas. Por lo tanto, consideramos que es esencial obtener claridad respecto a la volatilidad de las criptomonedas según sus propiedades tecnológicas, con el fin de comprender mejor los riesgos al incorporarlas en un portafolio de divisas de familias conservadoras.

Con base en lo anterior, surgen los siguientes conjuntos de preguntas:
- Primero **(P1)**, Desde el punto de vista del contexto internacional: ¿cuál es la volatilidad entre criptodivisas? ¿Qué tanto varía la volatilidad entre una criptodivisa y otra?; puntualmente, ¿qué tanto varía la volatilidad entre criptomonedas según sus propiedades tecnológicas?
- Segundo **(P2)**, Desde el punto de vista del contexto local de los países latino-americanos, ¿se intensifica la volatilidad del mercado de criptomonedas? Es decir, ¿el riesgo aumenta en un país latino-americano si se compara con un país como EEUU?
- Tercero **(P3)**, ¿cuáles son las criptomonedas que evidencian una mayor volatilidad y cuáles una menor volatilidad?, ¿cuáles criptomonedas serían las más apropiadas para una familia conservadora de Latinoamérica?

## Objetivos y KPIs
En esta sección, planteamos los objetivos (p. ej., O1) para dar respuesta a las preguntas que orientaran nuestro análisis (p. ej., P1.O1).

**(P1)** Desde el punto de vista del contexto internacional: ¿Cuál es la volatilidad de las criptodivisas? ¿Qué tanto varía la volatilidad entre una criptodivisa y otra?; puntualmente, ¿qué tanto varía la volatilidad entre criptomonedas según sus propiedades tecnológicas?
- P1.O1.: Medir la volatilidad de una conjunto de criptomonedas por año por medio de la desviación estándar (KPI #1).
- P1.O2.: Comparar la variación en volatilidad (KPI #1) entre de dos grupos de criptomonedas con propiedades tecnológicas similares.

**(P2)** Desde el punto de vista del contexto local de los países latino-americanos, ¿se intensifica la volatilidad del mercado de criptomonedas?
- P2.O1.: Medir la volatilidad de las criptomonedas en una selección de países latino-americanos, en un conjunto de datos transformados que controla por cambios en la inflación y ajusta los precios para que reflejen una paridad en el poder adquisitivo.
- P2.O2.: Comparar la magnitud de la volatilidad entre países (KPI #1) y explorar diferencias o similitudes entre contexto locales; es decir, explorar si la volatilidad aumenta en países latino-americanos en relación con un país de referencia (EEUU).

**(P3)** ¿cuáles son las criptomonedas que evidencian una mayor volatilidad en relación con la volatilidad inherente del mercado?, ¿cuáles criptomonedas serían las más apropiadas para portafolio de inversión conservador?
- P3.O1.: Medir la magnitud de la volatilidad de cada criptomoneda en relación con la volatilidad de otras criptomonedas (KPI #2).
- P3.O2.: Identificar las criptomonedas relativamente más volátiles y las menos volátiles.
- P3.O3.: Sugerir las criptomonedas relativamente más estables para portafolios de inversión conservadores (KPI #3).

## Desarrollo y hallazgos

Hemos dividido nuestro proyecto en dos grupos de criptomonedas, cada uno con propiedades tecnológicas específicas: las monedas con autonomía tecnológica (conocidas como ["Layer 1"](https://www.techopedia.com/definition/layer-1-in-blockchain)) y las monedas cuyo valor está vinculado a otros activos (conocidas como [stablecoins](https://www.investopedia.com/terms/s/stablecoin.asp)). Consideramos que esta distinción es relevante para nuestro estudio, basándonos en la siguiente evaluación teórica. En primer lugar, las monedas con autonomía tecnológica dependen menos de los cambios tecnológicos de otras monedas, ya que se encuentran al inicio de la cadena de producción de la arquitectura blockchain. Por otro lado, otras criptomonedas, como las ["Layer-2"](https://www.coingecko.com/learn/what-are-layer-2-crypto-protocols), dependen tecnológicamente del grupo "Layer-1", puesto que se construyen sobre la arquitectura de estas últimas. Creemos que esta dependencia tecnológica también se refleja en los precios. En otras palabras, consideramos que la autonomía tecnológica de las "Layer-1" contribuye a que la volatilidad de sus precios no esté directamente ligada a la volatilidad de criptomonedas ubicadas más abajo en la cadena de producción. En segundo lugar, el precio de las criptomonedas "stablecoins" es relativamente independiente del precio de otras criptomonedas, ya que su valor está anclado a otros activos intercambiables, como el USD o el oro; esto las convierte en un grupo ideal que actúa como punto de referencia para evaluar la variación en volatilidad entre diferentes criptomonedas. Consideramos que examinar estos grupos nos permite comprender mejor las variaciones en la volatilidad de los precios según las diferentes propiedades tecnológicas, y así identificar las criptomonedas relativamente más estables. 

Utilizamos una serie de tres (3) indicadores clave de rendimiento (KPI) para abordar nuestros tres conuntos de interrogantes. *En primer lugar*, empleamos la desviación estándar como nuestro **KPI No.1** para medir la volatilidad anual de cada moneda en ambos grupos **(P1)**. En términos generales, encontramos que, en promedio, el grupo "Layer-1" es sustancialmente más volátil que el grupo  "stable coins" en todos los años. También encontramos que el grupo de "stable coins" demuestra una variación menor en la volatilidad de sus miembros (monedas) en comparación con el grupo "Layer-1". En principio, estos dos hallazgos indica que el grupo "stable coins" es un mejor candidato para portafolios de inversión conservadores. Sin embargo, se presentan algunas diferencias al analizar caso por caso. Por un lado, constatamos que efectivamente el grupo "Layer-1" contiene las criptomonedas más volátiles en términos absolutos, mientras que el grupo "stable coins" incluye las menos volátiles. De otro lado, también encontramos que no todas las criptomonedas del grupo de "stable coins" son necesariamente menos volátiles; específicamente, identificamos que algunas criptomonedas del grupo "Layer-1" son menos volátiles que algunas de sus contrapartes del grupo "stable coins". En términos generales, esto sugiere que las monedas del grupo "stable coins" podrían ser candidatas más sólidas para ser incluidas en portafolios de inversión conservadores. No obstante, en el análisis a nivel individual, esto también señala la posibilidad de tener candidatos individuales de ambos grupos.

*En segundo lugar*, exploramos si la volatilidad varía en diferentes contextos locales **(P2)**. Dado nuestro interés en explorar el posible papel de las criptomonedas para inversionistas en países latinoamericanos con perfiles conservadores, consideramos esencial examinar las diferencias en la volatilidad entre diferentes entornos locales. Para lograr esto, empleamos el **KPI No.1** para medir la volatilidad, pero aplicamos transformaciones a los datos para controlar los cambios en la inflación (precios constantes) y ajustamos los precios para reflejar la paridad del poder adquisitivo (precios constantes ajustados mediante PPP). Nos enfocamos en los cuatro países más poblados de América Latina: Brasil, México, Argentina y Colombia. También incluimos a Estados Unidos como país de referencia. Como era de esperar, encontramos que la volatilidad en el grupo de criptomonedas observado es más alta desde la perspectiva de los países latinoamericanos en comparación con Estados Unidos. Esto sugiere que los inversionistas conservadores en países de América Latina deben ser más cautelosos al considerar la incorporación de criptomonedas en un portafolio de divisas, ya que la volatilidad se intensifica significativamente en sus contextos locales.

*En tercer lugar*, evaluamos la magnitud de la volatilidad de una moneda utilizando nuestro **KPI No.2**, denominado "Volatilidad relativa" **(P3)**. Este indicador nos permite cuantificar la intensidad de la volatilidad de una moneda en relación con la volatilidad promedio de otras monedas con propiedades tecnológicas similares. En este sentido, si la "Volatilidad relativa" es > 1, consideramos que la moneda es relativamente volátil; si la "Volatilidad relativa" es < 1, la consideramos relativamente estable. Este KPI permite categorizar las monedas según su nivel de volatilidad y comparar su rendimiento a lo largo del tiempo, así como también contrastar las magnitudes entre distintos grupos. Resaltamos algunos hallazgos. Dentro de los grupos "Layer-1" y "stable coins", Bitcoin y Pax Gold se distinguen como los casos con la mayor magnitud de volatilidad relativa a lo largo de los años, respectivamente. De manera específica, estas monedas son aproximadamente 10 veces más volátiles en comparación con el promedio de sus respectivos grupos. Además, es relevante señalar que tanto los casos extremos como las medianas de las magnitudes son muy similares entre los dos grupos, lo cual sugiere que ambos grupos se comportan bajo dinámicas muy parecidas.

*En cuarto lugar*, hemos identificado las monedas que son relativamente más estables a través de nuestro **KPI No.3**, denominado "Índice de Estabilidad Relativa" (IER) **(P3)**. En resumen, nuestro IER es una métrica ponderada que considera tanto la "Volatilidad relativa" como el volumen intercambiado, otorgando un mayor peso al primero (66%) que al segundo (34%). La inclusión del volumen intercambiado nos permite recomendar criptomonedas que no solo son relativamente estables, sino que también demuestran niveles relativamente altos de liquidez. Hemos determinado que "Cardano" ("Layer-1") y "Tether" ("stable coins") son las monedas relativamente más estables y con un mayor potencial de liquidez. Este hallazgo sugiere que estas monedas tienen el potencial de ser incluidas en portafolios de inversión con un perfil conservador y una baja tolerancia al riesgo.

## Ejecución del proyecto
Desarrollamos el proyecto en 3 partes: i. Cargar y limpiar base datos, y generar subconjuntos de datos (ETL); ii. Examinar la naturaleza y composición de los datos (EDA); iii. Alimentar un dashboard en Tableau.

### 1. ETL
Esta fase incluye dos partes:
1. [Extracción de datos](data_process/01_etl_v7.ipynb).
2. [Limpieza y preprocesamiento de datos](data_process/02_etl_tranform_v2.ipynb).

### 2. [EDA](data_process/03_eda_v2.ipynb)
En esta fase, exploramos los datos con el fin de responder a nuestras preguntas.

### 3. Dashboard
Desarrollamos nuestro dashboard en Tableau Public: acceso.