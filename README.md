# LABORATORIO 1 PROCESAMIENTO DIGITAL DE SEÑALES
# Análisis estadístico de la señal 
## Docente : Carolina Corredor Bedoya
## Integrantes : Liseth Yuliana Clavijo Mesa                                                                                                                                                                                      Maria Camila Rodriguez                                                                                                                                                                                           Adriana Valentina Alarcon 
## Fecha : Agosto 2025
# Introduccion: 
Las señales biomédicas constituyen una fuente esencial de información clínica, ya que permiten analizar el funcionamiento de diferentes sistemas fisiológicos. Sin embargo, dichas señales suelen estar afectadas por diversos tipos de ruido, lo que dificulta su interpretación. En este laboratorio se trabajó con señales fisiológicas reales y generadas, con el objetivo de calcular sus principales parámetros estadísticos, evaluar la relación señal-ruido (SNR) y comparar los resultados obtenidos en diferentes condiciones de adquisición.
# Marco teorico:
Las señales biomédicas son variaciones eléctricas, mecánicas o químicas generadas por el cuerpo humano que permiten analizar la actividad fisiológica. Entre las más comunes se encuentran el electrocardiograma (ECG), el electroencefalograma (EEG) y la electromiografía (EMG).

El análisis de estas señales requiere considerar tanto la información útil (amplitud, frecuencia, patrones característicos) como la presencia de ruido, entendido como cualquier perturbación que distorsiona la señal original y puede provenir de fuentes internas (movimientos, interferencias fisiológicas) o externas (equipos, ambiente).

Para caracterizar cuantitativamente una señal, se emplean estadísticos descriptivos, entre los que destacan:

·Media: valor promedio de la señal, indica la tendencia central.

·Desviación estándar: mide la dispersión de los datos respecto a la media.

·Coeficiente de variación: relaciona la desviación estándar con la media, expresando la variabilidad relativa.

·Histograma: representa gráficamente la distribución de frecuencias.

·Función de probabilidad: describe la probabilidad de ocurrencia de ciertos valores de la señal.

Además, la relación señal-ruido (SNR) es un parámetro fundamental que compara la potencia de la señal útil frente a la potencia del ruido. Un SNR alto implica una señal clara y confiable, mientras que un SNR bajo indica una señal fuertemente contaminada.

El uso de herramientas computacionales como Python, con librerías como NumPy, SciPy y Matplotlib, permite importar, procesar y analizar señales fisiológicas de manera eficiente. Asimismo, plataformas como PhysioNet ofrecen bases de datos abiertas que facilitan el acceso a señales reales para fines académicos e investigativos.
# Objetivo:
-Identificar los estadísticos que describen una señal biomédica, obtenerlos a partir de algoritmos de programación y mostrarlos. 
- Implementar algoritmos de Python.
- comparara señales fisiologicas de bases de datos con señales que fueron generadas en un laboratorio
- analizar el efecto del ruido sobre las señales capturadas 
# Procedimiento:
Se descargaron señales fisiologicas desde una base de datos estas señales fueron importadas en Python para luego hacer un calculo estadisticos de esta señal como la medioa, la desviacion, coeficientes de variacion entre otro.
se tomaron datos fisiologicos en el laboratorio y a estos se les realizo el mismo poceso que a la señal tomada de la base de datos para luego hacer una comparacion de estas señales.
por ultimo se implemento ruido a la señal analizando el efecto que tenia sobre esta

## Parte A
Se descargó una señal fisiológica desde PhysioNet, la cual fue importada y graficada en Python utilizando Matplotlib. Posteriormente, se calcularon los estadísticos descriptivos (media, desviación estándar, coeficiente de variación, histograma y función de probabilidad) tanto mediante fórmulas programadas como con funciones predefinidas de NumPy y SciPy.

## Descarga y grafica de la señal código de google colab

<img width="1264" height="610" alt="image" src="https://github.com/user-attachments/assets/b111faff-c743-4442-89d3-0011f030ab37" />

señal descargada. 
<img width="973" height="546" alt="image" src="https://github.com/user-attachments/assets/28ff3b58-3761-4a1e-87d4-f14bd1581a89" />

<img width="1241" height="386" alt="image" src="https://github.com/user-attachments/assets/7a17c113-a4de-432e-a08f-4263bde8d7a2" />

señal electrocardiografica 
<img width="948" height="573" alt="image" src="https://github.com/user-attachments/assets/b1e51e8e-fe81-4643-987b-c33e15283a9c" />

## interpretación de esta grafica 
Esta corresponde a una señal electrocardiografica en el eje X se representa el tiempo y en el eje Y se observa la amplitud de la señal, esta tiene un comportamiento oscilatorio coon variaciones peridicas de amplitud, se pueden inferir picos recurrentes de ondas R que correponden a la actividad delectrica que tiene el corazón
a su vez se puede evidenciar presencia de riodos y variaciones irregurales lo cuak se acerca a una señal biomedica real.

## Calculos estadisticos descriptivos de la señal.
<img width="695" height="668" alt="image" src="https://github.com/user-attachments/assets/211fc051-e369-40f1-b38c-4d00be19ffe8" />

## Histograma y funcion de probabilidad 
<img width="910" height="470" alt="image" src="https://github.com/user-attachments/assets/f673f5c9-f848-4c18-a4b2-8a6ccdfd176c" />
<img width="890" height="465" alt="image" src="https://github.com/user-attachments/assets/0ed9a05a-8c3e-459e-9b52-abbe72439063" />




## Parte B
Se generó una señal fisiológica similar por medio del ruido gaussiano.Luego, se importó y graficó en Python, calculándose los mismos estadísticos para compararlos con los obtenidos en la Parte A.


## Parte C
La señal de la Parte B fue contaminada con ruido gaussiano, impulsivo y de tipo artefacto. En cada caso se midió la relación señal-ruido (SNR) y se analizaron los efectos sobre la calidad de la señal. Finalmente, todos los resultados y códigos fueron documentados en un repositorio de GitHub.

# Resultados:
## Parte A:
## Señal descargada y análisis estadístico

## Señal 1 descargada de PhysioNet sin rangos de datos

# <img width="757" height="521" alt="image" src="https://github.com/user-attachments/assets/14f240c5-f7e0-4e59-a487-ae08b373bcd5" />


## Señal 2 descargada de PhysioNet con rangos de datos


# <img width="694" height="512" alt="image" src="https://github.com/user-attachments/assets/16b174ca-c8b8-4cb8-82d0-b5c504eed5cb" />





# Conclusiones: 
El análisis de señales fisiológicas permitió comprender cómo las variables estadísticas (media, desviación estándar, coeficiente de variación, curtosis, entre otras) contribuyen a la caracterización y comprensión del comportamiento de las señales biomédicas.

La comparación entre la señal real obtenida desde PhysioNet (Parte A) y la señal generada artificialmente (Parte B) evidenció similitudes en sus propiedades estadísticas, pero también diferencias que reflejan la naturaleza más idealizada y menos contaminada de las señales simuladas.

La incorporación de ruido gaussiano, impulsivo y por artefactos (Parte C) permitió observar la degradación de la señal y cuantificarla a través de la relación señal-ruido (SNR), resaltando la importancia de esta métrica para evaluar la calidad de los datos biomédicos.

El trabajo integró el uso de herramientas computacionales como Python y librerías científicas para el procesamiento, análisis y visualización de señales, fortaleciendo competencias prácticas en el área de bioseñales.

En conjunto, la práctica demostró que el análisis estadístico y la evaluación de la calidad de señales son pasos fundamentales para garantizar la correcta interpretación clínica y el desarrollo de sistemas biomédicos más robustos y confiables.

# Referencias: 
·Goldberger, A. L., Amaral, L. A. N., Glass, L., Hausdorff, J. M., Ivanov, P. C., Mark, R. G., Mietus, J. E., Moody, G. B., Peng, C. K., & Stanley, H. E. (2000). PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. Circulation, 101(23), e215–e220. https://doi.org/10.1161/01.CIR.101.23.e215

·Clifford, G. D., Azuaje, F., & McSharry, P. (2006). Advanced Methods and Tools for ECG Data Analysis. Artech House.

·Acharya, U. R., Joseph, K. P., Kannathal, N., Lim, C. M., & Suri, J. S. (2006). Heart rate variability: a review. Medical & Biological Engineering & Computing, 44, 1031–1051. https://doi.org/10.1007/s11517-006-0119-0

·Hamilton, P. S. (2002). Open source ECG analysis. Computers in Cardiology, 29, 101–104. https://doi.org/10.1109/CIC.2002.1166717

·Stoica, P., & Moses, R. L. (2005). Spectral Analysis of Signals. Pearson Prentice Hall.

·Shumway, R. H., & Stoffer, D. S. (2017). Time Series Analysis and Its Applications: With R Examples (4th ed.). Springer.

·Oppenheim, A. V., & Schafer, R. W. (2010). Discrete-Time Signal Processing (3rd ed.). Pearson.

·Proakis, J. G., & Manolakis, D. G. (2007). Digital Signal Processing: Principles, Algorithms, and Applications (4th ed.). Pearson.

·Rangayyan, R. M. (2015). Biomedical Signal Analysis: A Case-Study Approach (2nd ed.). IEEE Press & Wiley.
