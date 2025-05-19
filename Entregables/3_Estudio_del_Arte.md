# 1. CONTEXTO CIENTÍFICO
### Artículo 1
 #### "Sistema escalable de control y monitoreo de plantas inteligentes basado en IoT para una agricultura sostenible"
 
Foysal et al. (2025) presentan un sistema escalable de monitoreo y control inteligente para agricultura sostenible, basado en la integración de un microcontrolador ESP32 con capacidades de comunicación Wi-Fi y un conjunto de sensores de bajo costo. El sistema mide en tiempo real la humedad volumétrica del suelo, la temperatura, la concentración de iones de hidrógeno (pH) y la humedad ambiental, complementándose con un módulo de cámara para evaluación visual de la salud foliar. Los datos se procesan localmente en el “Edge” para ejecutar lógicas de riego y fertilización automáticas, antes de enviarlos a una plataforma en la nube para análisis histórico. Se destaca la recolección continua con intervalos ajustables (1–10 min), un diseño modular “plug & play” y la capacidad de integrarse en huertos urbanos o grandes fincas sin modificaciones de infraestructura[1].

### Artículo 2
 #### "Sistema de monitoreo de la salud del suelo en tiempo real basado en IoT para agricultura de precisión"

En este trabajo, los investigadores presentan un dispositivo compacto basado en ESP32S3 que incorpora varias sondas electroquímicas para medir en simultáneo la humedad, temperatura, pH y conductividad eléctrica del suelo, así como concentraciones de macronutrientes (N, P, K). El sistema realiza una rutinas de autorcalibración: utiliza un pequeño depósito con solución patrón (pH y conductividad conocidos) para ajustar dinámicamente las curvas de calibración cada 24 h. La transmisión de datos se lleva a cabo mediante LoRaWAN, alcanzando distancias de hasta 8 km en campo abierto. Las baterías recargables Li-Po de alta densidad ofrecen autonomía de hasta 14 días en modo de muestreo cada 15 min. Pruebas en parcelas de maíz mostraron una mejora del 15 % en la eficiencia de fertilización (N y P) y una reducción del 18 % en el consumo de agua comparado con métodos basados en calendario, así como la generación automática de mapas georreferenciados en la plataforma ThingsBoard[2].

### Artículo 3
#### "Development and Application of an IoT-Based System for Soil Water Status Monitoring in a Soil Profile"

Comegna et al. (2024) presentan SHYPROM, un sistema IoT de monitoreo del estado hídrico del suelo diseñado tanto para laboratorio como para campo. El prototipo emplea un microcontrolador ESP32-SIM800L con convertidores ADC de 12 bits que alimentan tres pares de electrodos capacitivos de acero inoxidable y dos transductores de presión MPX5100DP acoplados a tensiómetros porosos. Cada 30 min el dispositivo mide simultáneamente el contenido volumétrico de agua (θ) y el potencial matricial (h) en distintas profundidades, y calcula la curva de conductividad hidráulica K(θ) mediante el método de perfil instantáneo, alcanzando una correlación R² = 0.92 frente a equipos de laboratorio. La plataforma transmite los datos en tiempo real a ThingSpeak vía GSM/Wi-Fi, almacena una copia local en tarjeta SD y dispone de una app Android para visualización y alertas. SHYPROM demostró alta fiabilidad (> 30 días) y un costo por unidad inferior a USD 100[3].

# 2. CONTEXTO COMERCIAL
## 2.1 PATENTES
 ### 2.1.1 US 20150181817A1 – Soil Moisture Sensor
 
Este invento define un sensor inalámbrico con cuerpo plano, dos electrodos inferiores y “barbillas” de anclaje que mide humedad, salinidad y temperatura. Transmite lecturas a un receptor que interrumpe el ciclo de riego al alcanzar un umbral predefinido, mejorando el ahorro de agua y reduciendo la deriva de calibración[4].
                                             ![Sensor](.../IMAGENES/Hito2/Soil moisture sensor.png)

 ### 2.1.2 US 2015/0330932 A1 – Capacitive Soil Moisture Sensor

El sensor descrito en la publicación US 2015/0330932 A1 utiliza una sonda capacitiva enterrada en el suelo cuya capacitancia, directamente influida por la humedad, se excita con un circuito en serie RLC sintonizado entre 100 y 300 kHz para maximizar la relación señal-ruido. La corriente resultante de la sonda se convierte en voltaje mediante un módulo I–V y, a continuación, un microcontrolador genera la señal PWM de excitación y digitaliza la medida con su ADC integrado, procesando así la información de humedad en tiempo real. Gracias a su diseño modular, todos los componentes pueden montarse en una única unidad compacta o separarse en un módulo de campo y otro de procesamiento, comunicándose mediante interfaces cableadas o inalámbricas, lo que facilita su instalación y transporte en aplicaciones agrícolas de campo[5].

 ### 2.1.3 US 7944220 B2-Moisture content sensor and related methods
 
El sensor descrito en la patente US 7,944,220 B2 emplea un bloque poroso de arcilla o gel que, al absorber agua del suelo, modifica la resistencia de un transductor encapsulado. Esa variación de resistencia se traduce en un voltaje proporcional, lo que permite medir con precisión el contenido de humedad y controlar sistemas de riego de forma automática . Al no contar con piezas móviles, el dispositivo responde en menos de 30 s y mantiene una señal estable a lo largo del tiempo. Además, su encapsulado resistente a la corrosión le confiere una larga vida útil incluso en condiciones agrícolas exigentes[6].

## 2.2 PRODUCTO COMERCIAL
 ### 2.2.1 Vegetronix VH400

Sonda capacitiva de humedad volumétrica (0–100 % VWC) con alta resolución (±1 %), cuerpo resistente a la corrosión y diseño compacto. Se integra mediante interfaz analógica en sistemas IoT o controladores de riego comerciales[7].

 ### 2.2.2 Acclima TDR-315H True TDR Soil Moisture Sensor

El TDR-315H utiliza la técnica de Reflectometría en Dominio del Tiempo (TDR) para enviar pulsos de alta frecuencia a través de dos varillas conductoras y medir el tiempo de retorno, calculando con alta exactitud la humedad volumétrica (±1 % VWC). Su electrónica interna corrige automáticamente las variaciones de temperatura y conductividad del suelo, y dispone de carcasa de ABS reforzado con fibra para resistencia UV y a químicos. Ofrece salidas RS-485 (Modbus RTU) y SDI-12, facilitando la integración en redes SCADA, estaciones meteorológicas y microcontroladores. Incluye software de diagnóstico y calibración que permite ajustar parámetros en campo, y su rango operativo se extiende de –40 °C a 70 °C[8].

  ### 2.2.3 Watermark 200SS Soil Moisture Sensor

El HydraProbe® de Stevens Water Monitoring Systems es una sonda multiparámetro que mide simultáneamente el contenido volumétrico de agua (θ) mediante Reflectometría en Dominio de Frecuencia y el potencial matricial (h) con un tensiómetro poroso. Además, integra sensores de conductividad eléctrica (EC) y temperatura para compensar las lecturas en tiempo real. Su carcasa de acero inoxidable y polímero resistente permite instalación permanente en profundidades modulables de 10 a 100 cm. La electrónica de 24 bits ofrece baja deriva (< 0.1 % anual) y consumo reducido (< 0.5 W), con salidas SDI-12 y RS-485. Puede integrarse con gateways LoRaWAN o NB-IoT y se acompaña del software AquaView™ para calibración remota, análisis de curvas θ(h) y generación de informes de trazabilidad. Diseñada para agricultura de precisión y gestión hídrica profesional, combina robustez, exactitud y facilidad de integración[9].




