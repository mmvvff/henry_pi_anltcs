# Henry: Proyecto Individual Análisis de datos
*Contexto.* Este proyecto responde a las consignas establecidas por la organización Henry como parte del segundo proyecto individual: [Análisis de datos](https://github.com/soyHenry/PI_DA).

## Motivación
Desde el principio del siglo XXI, el país Argentina se ha enfrentado a una alta volatilidad en la tasa de cambio de su Peso Argentino (ARS), junto con elevados niveles de inflación. Esto supone retos para las familias argentinas con activos líquidos en moneda local (p. ej., ahorros). En este contexto, algunas familias argentinas han aprovechado la estabilidad cambiaria del dólar estadounidense (USD) para construir un portafolio de divisas con el fin de disminuir su exposición a la volatilidad del ARS y a la inflación local. Sin embargo, algunos especialistas argumentan que las criptomonedas también constituyen una divisa adicional que se podría incorporar en dicho portafolio. Este argumento se basa en la documentada correlación negativa entre algunas criptomonedas y el USD, lo cual hace que estas divisas digitales adquieran propiedades de cobertura ("hedge") y de diversificación. De esta manera, la incorporación de criptomonedas en un portafolio de divisas puede ayudar a disminuir su exposición a cambios drásticos en la tasa de cambio de la moneda local y en contextos de elevados niveles de inflación.

En este contexto, surgen las siguientes preguntas. Primero **(P1)**, ¿cuáles son las criptomonedas que poseen propiedades de cobertura con relación al USD?; es decir, ¿cuáles criptomonedas evidencian una mayor correlación negativa con el USD? Segundo **(P2)**, ¿cuáles son las criptomonedas que poseen propiedades de diversificación?; es decir, ¿cuáles criptomonedas actúan como un depósito de valor relativamente independiente de la volatilidad de la moneda local? Finalmente, tercero **(P3)**, si tengo pesos argentinos (es decir, activos líquidos en moneda local), ¿cuál sería la mejor manera de construir un portafolio de divisas (compuesto por ARS, USD y una combinación de criptomonedas) para disminuir mi exposición a la volatilidad que caracteriza al ARS?; particularmente, ¿cuál sería su composición ideal (%) que garantice la estabilidad del valor del portafolio en un contexto de elevados niveles de inflación local?

## Objetivos y métodos

En esta sección, planteamos los objetivos (p. ej., O1) para dar respuesta a cada pregunta (p. ej., P1.O1).

**(P1)** ¿cuáles son las criptomonedas que poseen propiedades de cobertura con relación al USD?
P1.O1.: Medir el grado de correlación entre ARS, USD y diferentes criptomonedas, ajustando por cambios en la inflación local.
P1.O2.: Seleccionar las criptomonedas que *no se mueven* en la misma dirección al USD y ARS.
P1.O3.: Hacer un ranking de criptomonedas con base en un KPI que evidencie propiedades de cobertura ("hedge").

**(P2)** ¿cuáles son las criptomonedas que poseen propiedades de diversificación?
P1.O1.: Medir el valor de depósito de cada criptomoneda con relación al USD y al ARS.
P1.O2.: Medir la estabilidad de cada criptomoneda con base un KPI pertinente.
P1.O3.: Medir la independencia de cada criptomoneda con relación a la volatilidad del ARS con base un KPI pertinente.
P1.O4.: Hacer un ranking de criptomonedas con base en una combinación de KPI que evidencie propiedades de diversificación (i.e., almacenamiento de valor relativamente independiente de la volatilidad de la moneda local).

## Desarrollo
Desarrollamos el proyecto en 4 partes: i. cargar y limpiar base datos, y generar subconjuntos de datos (ETL); ii. Examinar la naturaleza y composición de los datos (EDA); iii. Procesar los datos; iv. Analizar los resultados; y, v. alimentar un dashboard en Streamlit.

### 1. ETL
Para facilitar la lectura, dividimos la fase de ETL en 4 fases:
1. Extraer datos.
2. Limpieza de datos.
3. Generar subconjuntos de datos para alimentar las otras fases.

### 2. EDA
La fase del análisis exploratorio de datos está orientada por la siguiente pregunta: **¿XXXX?**

### 3. Procesamiento de datos
Desarrollamos nuestros objetivos planteados.

### 4. Análisis y conclusiones
Damos respuesta a nuestras preguntas y delineamos unas conclusiones.

### 5. Dashboard
Desarrollamos nuestro dashboard en Streamlit.