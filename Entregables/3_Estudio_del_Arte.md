# CONTEXTO CIENTÍFICO
### Artículo 1
 #### "Scalable IoT-based Smart Plant Monitoring and Control System for Sustainable Agriculture"
 
Foysal et al. (2025) presentan un sistema escalable de monitoreo y control inteligente para agricultura sostenible, basado en la integración de un microcontrolador ESP32 con capacidades de comunicación Wi-Fi y un conjunto de sensores de bajo costo. El sistema mide en tiempo real la humedad volumétrica del suelo, la temperatura, la concentración de iones de hidrógeno (pH) y la humedad ambiental, complementándose con un módulo de cámara para evaluación visual de la salud foliar. Los datos se procesan localmente en el “Edge” para ejecutar lógicas de riego y fertilización automáticas, antes de enviarlos a una plataforma en la nube para análisis histórico. Se destaca la recolección continua con intervalos ajustables (1–10 min), un diseño modular “plug & play” y la capacidad de integrarse en huertos urbanos o grandes fincas sin modificaciones de infraestructura[1].

### Artículo 2
"IoT-Based Real-Time Soil Health Monitoring System for Precision Agriculture"

En este trabajo, los investigadores presentan un dispositivo compacto basado en ESP32S3 que incorpora varias sondas electroquímicas para medir en simultáneo la humedad, temperatura, pH y conductividad eléctrica del suelo, así como concentraciones de macronutrientes (N, P, K). El sistema realiza una rutinas de autorcalibración: utiliza un pequeño depósito con solución patrón (pH y conductividad conocidos) para ajustar dinámicamente las curvas de calibración cada 24 h. La transmisión de datos se lleva a cabo mediante LoRaWAN, alcanzando distancias de hasta 8 km en campo abierto. Las baterías recargables Li-Po de alta densidad ofrecen autonomía de hasta 14 días en modo de muestreo cada 15 min. Pruebas en parcelas de maíz mostraron una mejora del 15 % en la eficiencia de fertilización (N y P) y una reducción del 18 % en el consumo de agua comparado con métodos basados en calendario, así como la generación automática de mapas georreferenciados en la plataforma ThingsBoard[2].

### Artículo 3
"Development and Application of an IoT-Based System for Soil Water Status Monitoring in a Soil Profile"

Comegna et al. (2024) presentan SHYPROM, un sistema IoT de monitoreo del estado hídrico del suelo diseñado tanto para laboratorio como para campo. El prototipo emplea un microcontrolador ESP32-SIM800L con convertidores ADC de 12 bits que alimentan tres pares de electrodos capacitivos de acero inoxidable y dos transductores de presión MPX5100DP acoplados a tensiómetros porosos. Cada 30 min el dispositivo mide simultáneamente el contenido volumétrico de agua (θ) y el potencial matricial (h) en distintas profundidades, y calcula la curva de conductividad hidráulica K(θ) mediante el método de perfil instantáneo, alcanzando una correlación R² = 0.92 frente a equipos de laboratorio. La plataforma transmite los datos en tiempo real a ThingSpeak vía GSM/Wi-Fi, almacena una copia local en tarjeta SD y dispone de una app Android para visualización y alertas. SHYPROM demostró alta fiabilidad (> 30 días) y un costo por unidad inferior a USD 100[3].


