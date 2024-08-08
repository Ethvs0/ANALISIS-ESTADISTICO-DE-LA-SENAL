# ANALISIS-ESTADISTICO-DE-LA-SEÑAL
## DESCRIPCIÓN
Este proyecto se centra en el análisis de señales fisiológicas descargadas de PhysioNet. El objetivo es importar, procesar y analizar estas señales utilizando técnicas estadísticas y de procesamiento de señales en el lenguaje de Python. El análisis incluye la visualización, el cálculo de estadísticos descriptivos y la evaluación de la relación señal-ruido (SNR) bajo diferentes tipos de ruido.
### PROCESAMIENTO DE LA SEÑAL
#### 1. Importación y Visualización: 
Se descargó una señal fisiológica de PhysioNet en este caso cu05(.dat y .hea), luego de esto se debe descargar la biblioteca wfdb, (nota: dependera de la consola o el programa que estes utilizando la forma de instalar esta libreria). La señal se graficó usando matplotlib para una visualización inicial y verificar que la biblioteca se descargo de forma correcta.
#### 2. Cálculo de Estadísticos Descriptivos:
- Media: Se calculó la media de la señal para obtener una medida del valor promedio.
- Desviación Estándar: Se calculó la desviación estándar para medir la dispersión de los valores respecto a la media.
- Coeficiente de Variación: Se determinó el coeficiente de variación para evaluar la relación entre la desviación estándar y la media.
- Histogramas: Se creó un histograma manualmente para representar la distribución de los valores de la señal.
<p align="center">
  <img src="https://github.com/Ethvs0/ANALISIS-ESTADISTICO-DE-LA-SENAL/blob/main/1.png" alt="Texto alternativo" width="400"/>
</p>
<div align="center">
  <p> Gráfica 1. Hidtograma de la señal cu05.</p>
</div>
#### 3. Evaluación de la Relación Señal-Ruido (SNR):
La función snr calcula la relación señal-ruido (SNR), una métrica clave en el análisis de señales que mide la calidad de una señal en presencia de ruido. La SNR se expresa en decibelios (dB) y proporciona una medida de cuánto de la señal es útil en comparación con la cantidad de ruido que contiene. Para obtener dicha relación se calcula el potencial de la señal y el ruido y luego se aplica la formula:

<p align="center">
  <img src="https://github.com/Ethvs0/ANALISIS-ESTADISTICO-DE-LA-SENAL/blob/main/5.png" alt="imagen 1" width="200"/>
</p>
<div align="center">
  <p> Formula 1. Relación señal ruido.</p>
</div>
- Ruido Gaussiano: Se añadió ruido gaussiano a la señal y se calculó el SNR para evaluar el impacto del ruido en la calidad de la señal.
<p align="center">
  <img src="https://github.com/Ethvs0/ANALISIS-ESTADISTICO-DE-LA-SENAL/blob/main/2.png" alt="Texto alternativo" width="600"/>
</p>
<div align="center">
  <p> Grafica 2. Grafica Señal y ruido Gaussiano.</p>
  <p> Se añade ruido gaussiano a la señal y grafica la señal original, el ruido normalizado, y la señal contaminada con ruido gaussiano.</p>
</div>

- Ruido Impulso: Se añadió ruido tipo impulso a la señal y se calculó el SNR.

<p align="center">
  <img src="https://github.com/Ethvs0/ANALISIS-ESTADISTICO-DE-LA-SENAL/blob/main/3.png" alt="Texto alternativo" width="600"/>
</p>
<div align="center">
  <p> Grafica 2. Grafica Señal y ruido pulso.</p>
  <p> Se añade  ruido de pulso a la señal y grafica la señal original, el ruido de pulso, y la señal contaminada con ruido de pulso.</p>
</div>

- Ruido Tipo Artefacto: Se añadió ruido tipo artefacto a la señal y se calculó el SNR.
<p align="center">
  <img src="https://github.com/Ethvs0/ANALISIS-ESTADISTICO-DE-LA-SENAL/blob/main/4.png" alt="Texto alternativo" width="600"/>
</p>
<div align="center">
  <p> Grafica 2. Grafica Señal y ruido artefacto.</p>
  <p> Se añade  ruido de tipo artefacto a la señal y grafica la señal original, el ruido de artefacto, y la señal contaminada con ruido de artefacto..</p>
</div>

### REQUISITOS
- Python 3.12.4 o algun programa que acepte y copile las librerias
- numpy
- matplotlib
- wfdb
### INSTRUCCIONES DE USO
1. Descargar y guardar una señal fisiológica desde PhysioNet.
2. Ejecutar el código en un entorno Python compatible (como Spyder, Google Colab, o cualquier IDE).
3. Revisar y ajustar los parámetros del código según sea necesario para los diferentes tipos de ruido.
