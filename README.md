**Abril 5, 2026 — Inicio del proyecto y organización**

En esta primera clase el profesor nos pidió crear una bitácora personal en GitHub para documentar todo el desarrollo del proyecto durante la cursada.

Decidí estructurar el repositorio en dos áreas principales:

Seguimiento automático de la ISS utilizando una cámara montada sobre un sistema motorizado.
Diseño y análisis de antenas para recepción de señales reflejadas por la Estación Espacial Internacional.

La idea es registrar avances, simulaciones, pruebas y resultados obtenidos durante cada etapa.

**Abril 8, 2026 — Primer contacto con antenas y mediciones**

Comenzamos a trabajar con hardware y herramientas de medición.

Las actividades principales fueron:

Construcción de un dipolo para 163 MHz.
Armado de una antena radial de 13 cm.
Intento de recepción de señales en 22.116 MHz relacionadas con ARTEMIS.

También aprendimos conceptos básicos de uso del NanoVNA y la importancia de mantener una impedancia cercana a 50 Ω para evitar problemas con el RTL-SDR.

Se trabajó con:

S11 (CH0): medición de reflexión y ROE.
S21 (CH1): análisis de transmisión/recepción.

Además, realizamos pruebas con RTL1090 para detectar señales ADS-B de aviones en 1090 MHz.

**Abril 10, 2026 — Análisis EXIF y parámetros fotográficos**

La clase estuvo enfocada en la parte óptica del proyecto.

Un grupo investigó herramientas para leer datos EXIF de fotografías utilizando programas como ExifViewer. El objetivo fue obtener información de captura como:

Apertura.
Tiempo de exposición.
Configuración de cámara.

Estos parámetros servirán para intentar replicar condiciones similares entre distintas cámaras y mejorar la calidad de las capturas de la ISS.

**Abril 12, 2026 — Trabajo dividido y simulación en MMANA-GAL**

La clase se dividió en dos actividades:

Un grupo continuó trabajando con datos EXIF.
El grupo en el que participé realizó el modelado de una antena radial con plano de tierra artificial para 22,116 MHz utilizando MMANA-GAL.

Esto permitió comenzar a familiarizarnos con herramientas de simulación y análisis de antenas.

**Abril 15, 2026 — Batido de ondas y montaje experimental**

Estudiamos el fenómeno de batido de ondas mediante la suma de señales sinusoidales, tema fundamental para entender cómo funcionan los SDR y la conversión de frecuencias.

El profesor compartió scripts en R para analizar matemáticamente estos fenómenos.

También se definieron aspectos importantes del sistema mecánico:

Uso de montura ecuatorial.
Configuración compatible con Gpredict.
Uso de correas en lugar de engranajes.
Limitación de tensión a 5V para proteger el Arduino.

Al finalizar la clase se instaló una antena de hilo largo en el mástil de la bandera para monitorear señales entre 7 MHz y 28 MHz.

**Abril 16, 2026 — Cambio de software SDR**

Debido a problemas de estabilidad de SDR# en Windows 10 y 11, se decidió migrar a SDR++, el cual presentó un funcionamiento más estable durante las pruebas realizadas.

**Abril 22, 2026 — Integración Arduino + Gpredict y comparación de antenas**

Se trabajó en la integración entre Arduino y Gpredict para controlar el movimiento de los motores del sistema de seguimiento.

Además:

Observamos una antena Magnetic Loop del laboratorio.
Exploramos Xnec2c como alternativa de simulación.

La actividad principal fue la simulación de antenas para 144.400 MHz utilizando MMANA-GAL. Se compararon distintos diseños:

Dipolo.
Moxon.
Yagi.

Los resultados obtenidos mostraron:

Antena	Ganancia
Yagi 3 elementos	7,83 dB
Moxon	5,43 dB

En esta etapa, la Yagi parecía la mejor opción por su mayor ganancia.

**Abril 29, 2026 — Selección final de la antena Moxon**

Luego de comparar distintas alternativas, finalmente se decidió utilizar una antena Moxon para el prototipo final.

Aunque la Yagi presentaba mejores resultados teóricos, la Moxon ofrecía ventajas importantes:

Menor tamaño.
Mayor robustez mecánica.
Mejor adaptación al sistema motorizado.

Se calcularon las dimensiones necesarias para una Moxon diseñada para 145 MHz utilizando conductor de 1 mm:

A: 748,8 mm
B: 108,0 mm
C: 25,8 mm
Longitud del excitador: 964,7 mm
Longitud del reflector: 1031,9 mm

La profundidad total del diseño fue cercana a 275,4 mm.

Además:

Continuamos estudiando el material teórico sobre batido de ondas.
Realizamos prácticas de soldadura con cautín.

**Mayo 6, 2026 — Suspensión de actividades por Zonda**

Las actividades presenciales fueron suspendidas debido al viento Zonda.

Aun así, el profesor compartió material y referencias sobre diseños de antenas Moxon para continuar avanzando de manera teórica.

**Mayo 20, 2026 - Armado antena**

Armamos la antena, cortamos tubos con las dimensiones adecuadas y colocamos los cables
Hicimos una prueba con walkie tokie
