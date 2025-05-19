# 1. CONTEXTO CIENTÍFICO
### Artículo 1
 #### "Scalable IoT-based Smart Plant Monitoring and Control System for Sustainable Agriculture"
 
Foysal et al. (2025) presentan un sistema escalable de monitoreo y control inteligente para agricultura sostenible, basado en la integración de un microcontrolador ESP32 con capacidades de comunicación Wi-Fi y un conjunto de sensores de bajo costo. El sistema mide en tiempo real la humedad volumétrica del suelo, la temperatura, la concentración de iones de hidrógeno (pH) y la humedad ambiental, complementándose con un módulo de cámara para evaluación visual de la salud foliar. Los datos se procesan localmente en el “Edge” para ejecutar lógicas de riego y fertilización automáticas, antes de enviarlos a una plataforma en la nube para análisis histórico. Se destaca la recolección continua con intervalos ajustables (1–10 min), un diseño modular “plug & play” y la capacidad de integrarse en huertos urbanos o grandes fincas sin modificaciones de infraestructura[1].

### Artículo 2
 #### "IoT-Based Real-Time Soil Health Monitoring System for Precision Agriculture"

En este trabajo, los investigadores presentan un dispositivo compacto basado en ESP32S3 que incorpora varias sondas electroquímicas para medir en simultáneo la humedad, temperatura, pH y conductividad eléctrica del suelo, así como concentraciones de macronutrientes (N, P, K). El sistema realiza una rutinas de autorcalibración: utiliza un pequeño depósito con solución patrón (pH y conductividad conocidos) para ajustar dinámicamente las curvas de calibración cada 24 h. La transmisión de datos se lleva a cabo mediante LoRaWAN, alcanzando distancias de hasta 8 km en campo abierto. Las baterías recargables Li-Po de alta densidad ofrecen autonomía de hasta 14 días en modo de muestreo cada 15 min. Pruebas en parcelas de maíz mostraron una mejora del 15 % en la eficiencia de fertilización (N y P) y una reducción del 18 % en el consumo de agua comparado con métodos basados en calendario, así como la generación automática de mapas georreferenciados en la plataforma ThingsBoard[2].

### Artículo 3
#### "Development and Application of an IoT-Based System for Soil Water Status Monitoring in a Soil Profile"

Comegna et al. (2024) presentan SHYPROM, un sistema IoT de monitoreo del estado hídrico del suelo diseñado tanto para laboratorio como para campo. El prototipo emplea un microcontrolador ESP32-SIM800L con convertidores ADC de 12 bits que alimentan tres pares de electrodos capacitivos de acero inoxidable y dos transductores de presión MPX5100DP acoplados a tensiómetros porosos. Cada 30 min el dispositivo mide simultáneamente el contenido volumétrico de agua (θ) y el potencial matricial (h) en distintas profundidades, y calcula la curva de conductividad hidráulica K(θ) mediante el método de perfil instantáneo, alcanzando una correlación R² = 0.92 frente a equipos de laboratorio. La plataforma transmite los datos en tiempo real a ThingSpeak vía GSM/Wi-Fi, almacena una copia local en tarjeta SD y dispone de una app Android para visualización y alertas. SHYPROM demostró alta fiabilidad (> 30 días) y un costo por unidad inferior a USD 100[3].

# 2. CONTEXTO COMERCIAL
## 2.1 PATENTES
 ### 2.1.1 US 20150181817A1 – Soil Moisture Sensor
 
Este invento define un sensor inalámbrico con cuerpo plano, dos electrodos inferiores y “barbillas” de anclaje que mide humedad, salinidad y temperatura. Transmite lecturas a un receptor que interrumpe el ciclo de riego al alcanzar un umbral predefinido, mejorando el ahorro de agua y reduciendo la deriva de calibración[4].

 ### 2.1.2 US 2015/0330932 A1 – Capacitive Soil Moisture Sensor

Esta patente detalla un sensor capacitivo que utiliza un circuito RLC integrado para medir la capacitancia del suelo, correlacionada directamente con su contenido de humedad. El dispositivo incluye un microcontrolador que filtra el ruido eléctrico y aplica correcciones de temperatura y conductividad, usando un sensor de temperatura integrado y un medicor de conductividad. Ofrece una respuesta ultra-rápida (< 0.5 s) y una deriva en señal inferior al 2 % anual. Está diseñado para lecturas continuas en entornos exigentes, con carcasa hermética IP67 y compatibilidad con protocolos UART y I²C [5].

 ### 2.1.3 US 7944220 B2 (“Moisture content sensor and related methods”
 
El sensor descrito en el documento US 7944220 B2 funciona mediante la medición de la variación de resistencia eléctrica en un material poroso, lo que permite determinar con precisión el potencial matricial del suelo. Su diseño incorpora un transductor de resistencia encapsulado que responde a cambios de humedad en un medio de arcilla o gel, ofreciendo una resolución de ±2 centibares en el rango de 0 a –1 bar y ±5 centibares en –1 a –10 bar. Al carecer de componentes mecánicos móviles y emplear un encapsulado resistente a la corrosión, este sensor garantiza tiempos de respuesta inferiores a 30 s, mínima deriva de señal a lo largo del tiempo y una vida útil prolongada en condiciones agrícolas exigentes. Su salida analógica de resistencia puede integrarse directamente en sistemas de registro de datos y control de riego automático[6].



