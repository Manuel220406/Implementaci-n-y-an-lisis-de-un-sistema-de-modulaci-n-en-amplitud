# Modulación en Amplitud (AM) – Actividad 4    
Materia: Señales y Sistemas  
Alumno: Manuel Banda González

# Descripción del proyecto
Este repositorio contiene la implementación de un sistema de **modulación en amplitud (AM)** desarrollado en Python como parte de la Actividad Formativa 4 del curso *Señales y Sistemas*.  
El proyecto incluye:
  - Generación de la señal de mensaje
  - Modulación AM
  - Análisis en el dominio del tiempo y la frecuencia
  - Simulación de ruido AWGN
  - Simulación de distorsión mediante un filtro pasa-bajas
  - Visualización y análisis de resultados
El propósito es comprender cómo se comporta un sistema AM bajo diferentes condiciones de canal y cómo se ve afectado por el ruido y la distorsión.

# Conceptos aplicados
- Modulación en amplitud (AM)
- Transformada Rápida de Fourier (FFT)
- Ruido blanco gaussiano aditivo (AWGN)
- Atenuación y distorsión
- Análisis temporal y espectral
- Procesamiento digital de señales (DSP)

# Requisitos
Utilizar Python e instalar las librerias necesarias:
 -numpy
 -matplotlib
 -scipy

---Estas librerias se pueden instalar con el comando "pip install numpy matplotlib scipy" utlizado en la linea de comandos o terminal---

# Ejecución
Basta con ejecutar el archivo principal:
  python Sistema_de_Modulacion_AM.py
El script generará las gráficas correspondientes a cada etapa.

# Estructura del código
El proyecto está organizado en las siguientes secciones:

1. Parámetros generales
  -Frecuencia de muestreo
  -Frecuencia del mensaje
  -Frecuencia de la portadora
  -Índice de modulación

2. Generación de la señal de mensaje
  -Onda sinusoidal de baja frecuencia

3. Modulación AM
  Aplicación de la ecuación:
    𝑠(𝑡)=𝐴𝑐(1+𝑘𝑎 𝑚(𝑡))cos(2𝜋𝑓𝑐𝑡)

4. Espectro en frecuencia (FFT)
  -Transformada rápida de Fourier

5.Ruido AWGN
  -Cálculo correcto según la potencia de la señal y el SNR deseado

6.Distorsión (Filtro pasa-bajas)
  -Implementado con Butterworth orden 4

# Resultados obtenidos
El programa genera las siguientes gráficas:
  -Señal de mensaje
  -Señal AM modulada
  -Espectro en frecuencia
  -Señal con ruido AWGN
  -Señal distorsionada por un filtro pasa-bajas
Estas visualizaciones permiten comparar cómo se altera la señal en distintos escenarios de transmisión.

# Gráficas generadas
Las graficas incluyen:
  -Dominio del tiempo de la señal original
  -Señal modulada AM
  -Espectro mostrando portadora y bandas laterales
  -Señal con ruido (SNR = 10 dB)
  -Señal filtrada mostrando atenuación de componentes altas

# Conclusiones
El experimento permitió analizar el funcionamiento de la modulación AM y estudiar cómo se ve afectada por condiciones del canal como ruido y distorsión. Se comprobó:
  -La portadora aparece claramente en el espectro junto con las bandas laterales.
  -El ruido AWGN degrada la señal pero mantiene su estructura principal.
  -Un filtro pasa-bajas atenúa las componentes altas de la portadora, generando distorsión notable.
  -Python es una herramienta eficaz para visualizar y comprender el comportamiento de sistemas de comunicación.
  -El proyecto demuestra cómo un sistema de comunicación analógico se ve afectado por las condiciones del canal.
