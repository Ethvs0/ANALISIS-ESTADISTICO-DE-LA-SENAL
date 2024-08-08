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
![Ejemplo de Señal](file:///C:/Users/ASUS/Documents/1.png)
#### 3. Evaluación de la Relación Señal-Ruido (SNR):
- Ruido Gaussiano: Se añadió ruido gaussiano a la señal y se calculó el SNR para evaluar el impacto del ruido en la calidad de la señal.

- Ruido Impulso: Se añadió ruido tipo impulso a la señal y se calculó el SNR.
- Ruido Tipo Artefacto: Se añadió ruido tipo artefacto a la señal y se calculó el SNR.
### REQUISITOS
- Python 3.12.4 o algun programa que acepte y copile las librerias
- numpy
- matplotlib
- wfdb
### INSTRUCCIONES DE USO
1. Descargar y guardar una señal fisiológica desde PhysioNet.
2. Ejecutar el código en un entorno Python compatible (como Spyder, Google Colab, o cualquier IDE).
3. Revisar y ajustar los parámetros del código según sea necesario para los diferentes tipos de ruido.
