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
Se generó una señal fisiológica de tipo ECG mediante un generador de señales biológicas en Python, buscando que tuviera características similares a la señal real descargada en la Parte A. Posteriormente, la señal fue graficada utilizando Matplotlib, lo que permitió observar su comportamiento en el dominio temporal.

Creacion de la señal
<img width="512" height="574" alt="image" src="https://github.com/user-attachments/assets/5e436dd6-6b5f-46a8-a07e-9ef37dca5ed1" />
## Grafica de la señal creada en google Colab
<img width="1085" height="471" alt="image" src="https://github.com/user-attachments/assets/75175293-e6fc-4695-8191-ed0ba647fe1b" />
## Calculos estadisticos descriptivos de la señal.

<img width="455" height="560" alt="image" src="https://github.com/user-attachments/assets/4614d604-4005-4697-b76b-15f7e70b5aa9" />

## Histograma y funcion de probabilidad 

<img width="1052" height="565" alt="Captura de pantalla 2025-08-24 234515" src="https://github.com/user-attachments/assets/1ce45b45-aac2-4772-aa82-0f52910d1dd3" />

<img width="1089" height="564" alt="image" src="https://github.com/user-attachments/assets/07da9e96-8a5e-43ba-bf96-6246021ca8c9" />










## Parte C
La señal de la Parte B fue contaminada con ruido gaussiano, impulsivo y de tipo artefacto. En cada caso se midió la relación señal-ruido (SNR) y se analizaron los efectos sobre la calidad de la señal. Finalmente, todos los resultados y códigos fueron documentados en un repositorio de GitHub.
¿Que es es la relación señal ruido (SNR)?
La relación señal-ruido, S/R o del inglés SNR (Signal to Noise Ratio) se define como la proporción existente entre la potencia de salida de la señal que se transmite y la potencia del ruido que la corrompe (por lo tanto hablamos únicamente de dispositivos que emiten sonido y nunca de dispositivos que lo captan). Este margen se mide, como casi todo lo relacionado con el audio, en decibelios y a continuación os vamos a explicar todo lo que debéis saber sobre este tema para ser capaces de comprar vuestros próximos dispositivos conociendo cada pequeño detalle de su rendimiento y si, por desgracia, sus niveles de ruido en la señal son demasiado altos para lo que nuestros oídos están preparados para captar.
<img width="277" height="51" alt="image" src="https://github.com/user-attachments/assets/dc940f33-0f53-4399-9fdc-8c6ecefd95bc" />


Señales con ruidos contaminados
<img width="876" height="394" alt="image" src="https://github.com/user-attachments/assets/51d622f8-772c-4c5c-88fd-1cb3571f3718" />
<img width="868" height="393" alt="image" src="https://github.com/user-attachments/assets/e897fda6-dc5c-4b6d-8d97-00d28fe62fec" />
<img width="851" height="398" alt="image" src="https://github.com/user-attachments/assets/061fa7e7-3f4a-44b4-9f01-f829362da1df" />

Se analizo de las señales

<img width="925" height="374" alt="image" src="https://github.com/user-attachments/assets/c43a9642-b69f-471b-92b4-7f82d6234483" />

Se demostró que la SNR disminuye a medida que la señal es contaminada con ruidos más agresivos.
El ruido gaussiano tiene menor impacto sobre la morfología de la señal.
El ruido de impulso es altamente perjudicial, ya que introduce picos falsos.
Los artefactos afectan la estabilidad de la línea base y complican el análisis de tendencias.
Este ejercicio permitió comprender la importancia de filtrado y preprocesamiento en señales biomédicas antes de su análisis clínico o estadístico.


# Diagramas de flujo
## Parte A
![Imagen de WhatsApp 2025-08-24 a las 23 25 39_2998a633](https://github.com/user-attachments/assets/3d85a266-f8e9-4b3b-bc94-fdec726d1f2a)
## Parte B
![Imagen de WhatsApp 2025-08-24 a las 23 25 39_b47ca1b3](https://github.com/user-attachments/assets/6ffda53e-68d6-4b77-a224-77b3c4a325a6)
## Parte C
![Imagen de WhatsApp 2025-08-24 a las 23 25 39_efe2239c](https://github.com/user-attachments/assets/f0f3b550-e8f0-41a1-90bf-c5ea6372aad2)


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
