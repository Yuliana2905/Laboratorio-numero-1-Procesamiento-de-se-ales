# LABORATORIO 1 PROCESAMIENTO DIGITAL DE SEÑALES
# Análisis estadístico de la señal 
## Docente : Carolina Corredor Bedoya
## Integrantes : Liseth Yuliana Clavijo Mesa                                                                                                                                                                                      Maria Camila Rodriguez                                                                                                                                                                                           Adriana Valentina Alarcon 
## Fecha : Agosto 2025
# Introduccion: 
Las señales biomédicas constituyen una fuente esencial de información clínica, ya que permiten analizar el funcionamiento de diferentes sistemas fisiológicos. Sin embargo, dichas señales suelen estar afectadas por diversos tipos de ruido, lo que dificulta su interpretación. En este laboratorio se trabajó con señales fisiológicas reales y generadas, con el objetivo de calcular sus principales parámetros estadísticos, evaluar la relación señal-ruido (SNR) y comparar los resultados obtenidos en diferentes condiciones de adquisición.
# Objetivo:
-Identificar los estadísticos que describen una señal biomédica, obtenerlos a partir de algoritmos de programación y mostrarlos. 
# Procedimiento:

## Parte A
Se descargó una señal fisiológica desde PhysioNet, la cual fue importada y graficada en Python utilizando Matplotlib. Posteriormente, se calcularon los estadísticos descriptivos (media, desviación estándar, coeficiente de variación, histograma y función de probabilidad) tanto mediante fórmulas programadas como con funciones predefinidas de NumPy y SciPy.


## Parte B
Se generó una señal fisiológica similar por medio del ruido gaussiano.Luego, se importó y graficó en Python, calculándose los mismos estadísticos para compararlos con los obtenidos en la Parte A.


## Parte C
La señal de la Parte B fue contaminada con ruido gaussiano, impulsivo y de tipo artefacto. En cada caso se midió la relación señal-ruido (SNR) y se analizaron los efectos sobre la calidad de la señal. Finalmente, todos los resultados y códigos fueron documentados en un repositorio de GitHub.

##
