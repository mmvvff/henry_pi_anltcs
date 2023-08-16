# Henry: Proyecto Individual Data Anlytics

*Contexto.* Este proyecto responde a las consignas establecidas por la organizacion Henry como parte del segundo proyecto individual: [Data Analytics](https://github.com/soyHenry/PI_DA).

## Motivación
Desde el principios del XXI, el país Argentina ha enfrentado una elevada volatilidad de su Peso Argentino (ARS) junto con altos niveles de inflación. Esto supone retos para las familias argentinas con activos líquidos en moneda local (p. ej., ahorros). Si bien el dolar (USD) se ha presentado como la divisa por excelencia que algunas familias argentinas han usado para disminuir su exposicion a la volatilidad del ARS y a la inflación local, las criptomonedas se posicionan como una divisa adicional que se podria incorporar en dicho portafolio. La razón: su documentada correlacion negativa con el USD, adquiriendo, por tanto, propiedades de cobertura y de diversificacion que pueden ayudar a disminuir la exposicion de un portafolio de divisas ante cambios drasticos en el ARS en contexto de elevados niveles de inflación local.

## Objetivo y metodo
Con base en lo anterior, en este documento intentamos responder a la siguiente pregunta. Si tengo unos pesos argentinos (i.e., activos liquidos en moneda local), ¿cuál seria la mejor manera de construir un portafolio de divisas (compuesto por ARS, USD and una combinación de criptomonedas) para disminuir mi exposición a la volatidad que caracteriza al ARS? Particularmente, ¿cuál seria su composición ideal (%) que garantice una estabilidad en valor del portafolio en un contexto de elevados niveles de inflación local?

Desarrollo la respuesta a esta pregunta en tres pasos. Primero, me concentro en medir el grado de correlación entre ARS, USD y diferentes combinaciones de criptomonedas, ajsutando por cambios en la inflacion local. Segundo, selecciono la combinación de criptomonedas que *no se mueve* en la misma dirección del USD y del ARS. Tercero, **aún no sé qué haría para identificar su composición ideal**.

## Desarrollos
 El proyecto esta dividido en 4 partes. En resumen, el proyecto consiste en i. limpiar y normalizar una base datos (ETL), ii. examinar la naturaleza y composicion de los datos (EDA), iii. diseñar e implementar un algoritmo sencillo para determinar la composicion ideal del portafolio de divisas, y iv. alimentar un dashboard en streamlit.

### 1. ETL
Para facilitar la lectura, dividimos la fase de ETL en 4 fases:
1. Extraer datos.
2. Limpieza de datos.
3. Generar dfs para alimentar las otras fases.

### 2. EDA
La fase del analisis exploratorio de datos esta orientada por la siguiente pregunta: **¿XXXX?**

### 3. Algortimo para determinar composición del portafolio de divisas.
Construimos nuestro algoritmo con base en la literatura sobre propiedad de cobertura y de diversificación de criptomonedas.

### 4. Dashboard
Desarrollamos nuestro dashboard en Streamlit.