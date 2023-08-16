# Henry: Proyecto Individual Análisis de datos
*Contexto.* Este proyecto responde a las consignas establecidas por la organización Henry como parte del segundo proyecto individual: [Análisis de datos](https://github.com/soyHenry/PI_DA).

## Motivación
Desde el comienzo del siglo XXI, Argentina se ha enfrentado a una alta volatilidad en la tasa de cambio de su Peso Argentino (ARS), junto con niveles elevados de inflación. Esto plantea retos para las familias argentinas que poseen activos líquidos en moneda local, como por ejemplo, ahorros. En este contexto, algunas familias argentinas han aprovechado la estabilidad cambiaria del dólar estadounidense (USD) para construir un portafolio de divisas con el fin de reducir su exposición a la volatilidad del ARS y a la inflación local.

No obstante, algunos especialistas argumentan que las criptomonedas también podrían constituir una divisa adicional que se podría incorporar en dicho portafolio. Este argumento se basa en la documentada correlación negativa entre algunas criptomonedas y el USD, así como en el potencial de algunas criptomonedas para actuar como depósitos de valor. De esta manera, las criptomonedas adquieren propiedades de cobertura ("hedge") y de diversificación, convirtiéndolas en candidatas ideales para ser incorporadas en dichos portafolios.

A pesar de esto, la volatilidad inherente del mercado de criptomonedas también ha generado varias alertas al considerarlas para un portafolio de divisas. Por lo tanto, surge la necesidad de obtener claridad con respecto al potencial de las criptomonedas en un portafolio de divisas que busque disminuir la exposición a la volatilidad del ARS en contextos de elevados niveles de inflación local.

Con base en lo anterior, surgen las siguientes preguntas:
- Primero **(P1)**, ¿cuáles son las criptomonedas que poseen propiedades de cobertura con relación al USD?; es decir, ¿cuáles criptomonedas evidencian una mayor correlación negativa con el USD?
- Segundo **(P2)**, ¿cuáles son las criptomonedas que poseen propiedades de diversificación?; es decir, ¿cuáles criptomonedas actúan como un depósito de valor relativamente independiente de la volatilidad de la moneda local?
- Finalmente, tercero **(P3)**, si tengo pesos argentinos (es decir, activos líquidos en moneda local), ¿cuál sería la mejor manera de construir un portafolio de divisas (compuesto por ARS, USD y una combinación de criptomonedas) para disminuir mi exposición a la volatilidad que caracteriza al ARS?; particularmente, ¿cuál sería su composición ideal (%) que garantice la estabilidad del valor del portafolio en un contexto de elevados niveles de inflación local?

## Objetivos y métodos
En esta sección, planteamos los objetivos (p. ej., O1) para dar respuesta a cada pregunta (p. ej., P1.O1).

**(P1)** ¿cuáles son las criptomonedas que poseen propiedades de cobertura con relación al USD?
- P1.O1.: Medir el grado de correlación entre ARS, USD y diferentes criptomonedas, ajustando por cambios en la inflación local.
- P1.O2.: Seleccionar las criptomonedas que *no se mueven* en la misma dirección al USD y ARS.
- P1.O3.: Hacer un ranking de criptomonedas con base en un KPI que evidencie propiedades de cobertura ("hedge").

**(P2)** ¿cuáles son las criptomonedas que poseen propiedades de diversificación?
- P1.O1.: Medir el valor de depósito de cada criptomoneda con relación al USD y al ARS.
- P1.O2.: Medir la estabilidad de cada criptomoneda con base un KPI pertinente.
- P1.O3.: Medir la independencia de cada criptomoneda con relación a la volatilidad del ARS con base un KPI pertinente.
- P1.O4.: Hacer un ranking de criptomonedas con base en una combinación de KPI que evidencie propiedades de diversificación (i.e., almacenamiento de valor relativamente independiente de la volatilidad de la moneda local).
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