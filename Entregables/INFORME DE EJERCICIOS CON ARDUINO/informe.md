![logo](https://github.com/Sawamurarebatta/GRUPO_4_FDD/blob/main/Entregables/INFORME%20DE%20EJERCICIOS%20CON%20ARDUINO/imagenes_informe/1.png)
  
  
**FACULTAD DE CIENCIAS E INGENIERÍA

![arduino](https://github.com/Sawamurarebatta/GRUPO_4_FDD/blob/main/Entregables/INFORME%20DE%20EJERCICIOS%20CON%20ARDUINO/imagenes_informe/2.png)


*INFORME DE EJERCICIOS CON ARDUINO Y COMPONENTES ELECTRÓNICOS BÁSICOS



**CURSO:


FUNDAMENTOS DE DISEÑO



Integrantes:

·   	Cosme Pérez Yosselin Lizeth

·   	Rebatta Jeri Patricia Del Pilar

·   	Michael Geser Andrés



EJERCICIOS CON COMPONENTES ELECTRÓNICOS BÁSICOS

Ejemplo 1 (motor direccion basica)

En este primer ejemplo hicimos el control de dirección de un motorreductor GA12-N20 utilizando un módulo L298N y una placa Arduino UNO. El objetivo fue invertir el sentido de giro del motor cada 5 segundos. Para esto, conectamos los pines IN1 e IN2 del L298N a los pines digitales del Arduino (D4 y D5), y habilitamos el pin ENA con un jumper para mantener el motor activo. No se controló la velocidad, solo la dirección. Este ejercicio nos ayudó a entender cómo usar un controlador L298N para manejar motores DC en proyectos.



**Materiales
1 motorreductor GA12-N20 (6 V)


1 módulo controlador de motores L298N


1 placa Arduino UNO o compatible


1 fuente de alimentación externa (batería o adaptador de 6–12 V)


1 placa de pruebas (protoboard)


Cables Dupont (macho-macho o macho-hembra)


1 cable USB para programar el Arduino


Software Arduino IDE

Evidencia:
![evidencia_1](https://github.com/Sawamurarebatta/GRUPO_4_FDD/blob/main/Entregables/INFORME%20DE%20EJERCICIOS%20CON%20ARDUINO/imagenes_informe/3.jpg)


















Ejemplo 2 (Potenciómetro de velocidad del motor)

En este segundo ejemplo hicimos el control de velocidad de un motor GA12-N20 usando un potenciómetro y un módulo L298N con Arduino. El objetivo fue variar manualmente la velocidad del motor a través de una señal PWM, generada a partir de la lectura analógica del potenciómetro. La dirección del motor se mantuvo fija (sentido horario), y los valores leídos (ADC) junto con los valores PWM calculados se mostraron en el monitor serial para observar cómo influye el giro del potenciómetro en la velocidad. Este ejercicio fue útil para entender cómo se pueden usar entradas analógicas para controlar motores en aplicaciones.

Materiales
1 motorreductor GA12-N20 (6 V)


1 potenciómetro lineal (10kΩ recomendado)


1 módulo controlador L298N


1 placa Arduino UNO o compatible


1 fuente de alimentación externa (6–12 V)


1 placa de pruebas (protoboard)


Cables Dupont


1 cable USB para cargar el programa al Arduino


Software Arduino IDE instalado
Evidencia:


















Ejemplo 3 (servo ds 3235 adc pwm)

En este tercer ejemplo hicimos el control de posición de un servomotor DS3235 usando un potenciómetro y la función writeMicroseconds() de Arduino. El potenciómetro se conectó a una entrada analógica y su valor se convirtió en una señal PWM con un ancho entre 500 y 2400 microsegundos, lo que permitió mover el servo en todo su rango. Aunque el ángulo no se controló directamente, sí se estimó con fines de visualización en el monitor serial. Esto nos permitió observar cómo varía la posición del servo según el valor analógico, lo cual es útil en aplicaciones biomédicas como ortesis robóticas, dispositivos de terapia motora o simuladores de movimiento.
Materiales
1 servomotor DS3235


1 potenciómetro (10 kΩ recomendado)


1 placa Arduino UNO o compatible


1 fuente externa de 6V–7.4V (mínimo 2A)


1 placa de pruebas (protoboard)


Cables Dupont


1 cable USB para la programación del Arduino


Software Arduino IDE instalado


Evidencia :

















Ejemplo 4 (servo_ds3235 control básico)


En este cuarto ejemplo hicimos el control de posición del servomotor DS3235 utilizando la función writeMicroseconds() de la librería Servo de Arduino. Se programaron cuatro posiciones específicas (0°, 90°, 180° y 270°) con sus respectivos valores de ancho de pulso adaptados al mayor rango de este servo de alto torque. Gracias a pausas de 5 segundos entre movimientos, se pudo observar con claridad la respuesta del actuador. Este tipo de control es útil en aplicaciones biomédicas donde se requiere mover articulaciones o mecanismos con precisión, como en órtesis robóticas o dispositivos de asistencia motora.
Materiales
1 servomotor DS3235


1 fuente externa de 6V–7.4V (mínimo 2A)


1 placa Arduino UNO o compatible


Cables Dupont o conectores de 3 pines


1 cable USB para programar el Arduino


Software Arduino IDE instalado

Evidencia :




















Ejemplo 5 (motor de vibración básico)

En este quinto ejemplo hicimos la activación básica de un micromotor de vibración tipo moneda, utilizando un Arduino UNO y un transistor NPN como interruptor electrónico. Programamos el motor para encenderse durante 2 segundos y apagarse por 1 segundo en un ciclo continuo. Este tipo de actuadores es fundamental en sistemas de retroalimentación háptica, como en dispositivos biomédicos para personas con discapacidad auditiva o en interfaces táctiles para rehabilitación. Se empleó también un diodo de protección para evitar daños por picos de voltaje, y se controló el motor con una señal digital desde el pin 3 del Arduino.
Materiales
1 micromotor de vibración tipo moneda (3V–5V)


1 transistor NPN (2N2222 o S8050)


1 diodo de protección (1N4007)


1 resistencia de 220 Ω


1 placa de pruebas (protoboard)


Cables Dupont


1 placa Arduino UNO o compatible


Arduino IDE instalado
Evidencia:












Ejemplo 6 (potenciómetro del motor de vibración)

En este sexto y último ejemplo, controlamos la intensidad de vibración de un micromotor tipo moneda mediante un potenciómetro conectado a una entrada analógica del Arduino. El valor leído se transforma en una señal PWM que regula la potencia entregada al motor a través de un transistor NPN. Esto permite una retroalimentación háptica proporcional, donde la intensidad de la vibración varía suavemente con la posición del potenciómetro. Además, los valores del ADC y del PWM se muestran en el monitor serial, permitiendo el análisis en tiempo real. Esta técnica es especialmente útil en dispositivos biomédicos que requieren estímulos sensoriales graduales o personalizables.

Materiales
1 micromotor de vibración tipo moneda


1 potenciómetro lineal de 10 kΩ


1 transistor NPN (2N2222 o S8050)


1 resistencia de 1 kΩ


1 diodo de protección (1N4007)


1 placa de pruebas (protoboard)


Cables Dupont


1 placa Arduino UNO o compatible


Arduino IDE instalado
Evidencia:









LINK (Del material audiovisual del taller) 
https://drive.google.com/drive/folders/1baGlwDrrcqd-FUc9nttekGmv_WtFbSxM?usp=sharing


