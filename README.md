# Henry: Proyecto Individual Data Anlytics

*Contexto.* Este proyecto responde a las consignas establecidas por la organizacion Henry como parte del segundo proyecto individual: [Data Analytics](https://github.com/soyHenry/PI_DA).

## Motivación
Desde el principios del XXI, el país Argentina ha enfrentado una elevada volatilidad de su Peso Argentino (ARS) junto con altos niveles de inflación. Esto supone retos para las familias argentinas con activos líquidos en moneda local (p. ej., ahorros). Si bien el dolar (USD) se ha presentado como la divisa por excelencia que algunas familias argentinas han usado para disminuir su exposicion a la volatilidad del ARS y a la inflación local, las criptomonedas se posicionan como una divisa adicional que se podria incorporar en dicho portafolio. La razón: su documentada correlacion negativa con el USD, adquiriendo, por tanto, propiedades de cobertura y de diversificacion que pueden ayudar a disminuir la exposicion de un portafolio de divisas ante cambios drasticos en el ARS en contexto de elevados niveles de inflación local.

## Objetivo y metodo
Con base en lo anterior, en este documento intentamos responder a la siguiente pregunta. Si tengo unos pesos argentinos (i.e., activos liquidos en moneda local), ¿cuál seria la mejor manera de construir un portafolio de divisas (compuesto por ARS, USD and una combinación de criptomonedas) para disminuir mi exposición a la volatidad que caracteriza al ARS? Particularmente, ¿cuál seria su composición ideal (%) que garantice una estabilidad en valor del portafolio en un contexto de elevados niveles de inflación local?

Desarrollo la respuesta a esta pregunta en tres pasos. Primero, me concentro en medir el grado de correlación entre ARS, USD y diferentes combinaciones de criptomonedas, ajsutando por cambios en la inflacion local. Segundo, selecciono la combinación de criptomonedas que *no se mueve* en la misma dirección del USD y del ARS. Tercero, **aún no sé qué haría para identificar su composición ideal**.

 El proyecto esta dividido en 4 partes. En resumen, el proyecto consiste en i. limpiar y normalizar una base datos (ETL), ii. examinar la naturaleza y composicion de los datos (EDA), iii. diseñar e implementar un algoritmo sencillo para determinar la composicion ideal del portafolio de divisas, y iv. alimentar un dashboard en streamlit.

#### 1. ETL
Para facilitar la lectura, dividimos la fase de ETL en 4 fases:
1. Extraer datos.
2. Limpieza de datos.
3. Algortimo para determinar composición del portafolio de divisas.
4. Generar dfs para alimentar las visualizaciones, incluyendo el dashboard.

#### 2. EDA
La fase del analisis exploratorio de datos esta orientada por la siguiente pregunta: ¿Qué podemos esperar como resultado en las consultas?

#### 3. ML del sistema de recomendacion
El sistema de recomendación esta basado en un [modelo no-supervisado.](data_prcssng/06_ml_recomendaciones_v3.ipynb)

#### 4. API de consultas

1. Prueba piloto de funciones que median las consultas: [Test de consultas.](data_prcssng/07_test_funciones.ipynb)
2. El API de consultas implementado en Render: [Enlace API.](https://henry-mlops-imdb.onrender.com/docs)
3. Prueba de implementación del API: [video](https://drive.google.com/file/d/1l_noVxU2NVhfE3jFHW210eWAeEiPmo22/view?usp=sharing)