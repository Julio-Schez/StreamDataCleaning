Bienvenido a este proyecto donde implementamos un **algoritmo de limpieza de datos en tiempo real para nodos de IoT Subterráneas** basado en Arduino MKR WAN 1310. Este sistema mejora la calidad de los datos recolectados por sensores de **temperatura, humedad y pH del suelo 🌡️💧**, procesándolos en tiempo real para asegurar su fiabilidad.

🛠️ Descripción del Nodo

El nodo sensor utiliza la placa Arduino MKR WAN 1310, que permite la comunicación eficiente a través de LoRaWAN 📡, ideal para proyectos en áreas subterráneas o remotas. Los sensores conectados al nodo incluyen:

- Sensor de temperatura. Monitorea la temperatura del suelo 🌡️.
- Sensor de humedad. Mide la humedad del suelo 💧.
- Sensor de pH. Registra los niveles de acidez o alcalinidad del suelo ⚗️.


Algoritmo de Limpieza de Datos en Tiempo Real ⏳ 

El algoritmo está optimizado para funcionar en tiempo real, procesando cada dato conforme llega. Esto es crucial en aplicaciones donde los datos se utilizan para la toma de decisiones inmediatas, como en agricultura de precisión 🌾.

Características Principales ✨ 
- Detección de valores atípicos. A medida que los datos llegan, el algoritmo verifica si están dentro de los umbrales esperados o si caen fuera de rangos utilizando el rango intercuartil (IQR), eliminando lecturas inusuales en tiempo real. 📊 
- Manejo de datos faltantes. Si hay pérdida de datos, el algoritmo aplica el método Last Observation Carried Forward (LOCF) al instante, garantizando que los huecos se llenen sin interrupciones. ❌ 
- Eliminación de duplicados. Los datos duplicados son detectados y eliminados inmediatamente, evitando que se procesen varias veces. 🗑️ 
