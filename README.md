# LABORATORIO 1 PROCESAMIENTO DIGITAL DE SEÑALES
# Análisis estadístico de la señal 
## Docente : Carolina Corredor Bedoya
## Integrantes : Liseth Yuliana Clavijo Mesa                                                                                                                                                                                      Maria Camila Rodriguez                                                                                                                                                                                           Adriana Valentina Alarcon 
## Fecha : Agosto 2025
# Objetivo:
-Identificar los estadísticos que describen una señal biomédica, obtenerlos a partir de algoritmos de programación y mostrarlos. 
# Procedimiento:
## Parte A
Se descargó una señal fisiológica desde PhysioNet, la cual fue importada y graficada en Python utilizando Matplotlib. Posteriormente, se calcularon los estadísticos descriptivos (media, desviación estándar, coeficiente de variación, histograma y función de probabilidad) tanto mediante fórmulas programadas como con funciones predefinidas de NumPy y SciPy.

## Parte B
Se generó una señal fisiológica similar mediante un generador de señales y se capturó con la tarjeta STM32, almacenándola en formato .txt. Luego, se importó y graficó en Python, calculándose los mismos estadísticos para compararlos con los obtenidos en la Parte A.

## Parte C
La señal de la Parte B fue contaminada con ruido gaussiano, impulsivo y de tipo artefacto. En cada caso se midió la relación señal-ruido (SNR) y se analizaron los efectos sobre la calidad de la señal. Finalmente, todos los resultados y códigos fueron documentados en un repositorio de GitHub.
