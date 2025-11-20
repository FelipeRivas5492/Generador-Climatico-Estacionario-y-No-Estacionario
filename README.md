<strong> GENERADOR CLIMATICO ESTACIONARIO. BASADO EN: </strong>

<p align="justify">
<strong>Chadwick, C., Gironás, J., Vicuña, S., Meza, F., and McPhee, J. (2018) Using a statistical pre-analysis approach as an ensemble technique for the unbiased mapping of GCM changes to local stations. J. Hydrometeor., 19(9), 1447-1465. https://doi.org/10.1175/JHM-D-17-0198.1 </strong>
</p>

<strong>  y GCM EN: </strong>

<p align="justify">
<strong>Vasquez, Nicolas; Mendoza, Pablo A., 2024, "Statistically downscaled and bias corrected CMIP6 models for Continental Chile under scenario SSP5-8.5", https://doi.org/10.7910/DVN/O3YBOT, Harvard Dataverse, V1.</strong>
</p>


<p align="justify"> 
1. El generador climático se basa en ajustar a los anuales de temperatura y precipitación distribuciones de probabilidad, luego, con números aleatorios correlacionados y aplicando la inversa de la distribución ajustada se generan los valores simulados.
  
  
<p align="justify"> 
 2. Para obtener los números aleatorios se calcula la descomposición de Cholesky de la matriz de correlación, que permite transformar valores independientes en valores correlacionados según la estructura intra e inter variable del clima observado. Con la descomposición de Cholesky y una matriz con valores que distribuyen normal e independiente se obtiene una matriz de aleatorios correlacionados entre 0 y 1. 
</p>

<p align="justify">
3. Para la generación de series no estacionarias, se usan las métricas de cambio NMAP_gcm_t, DMAT_gcm_t, NMSDP_gcm_t y DMSDT_gcm_t, estas se calculan para cada GCM y cada año tal que t_i &lt; t, con t_i el fin del período histórico. Estas métricas representan los cambios relativos móviles proyectados, para el caso de la precipitación corresponde a la proporción entre el promedio móvil y el promedio histórico del GCM y para las temperaturas es la diferencia entre el promedio móvil y el promedio histórico del GCM. 
</p> 


<p align="justify">
4. Con las métricas explicadas, se corrigen los parámetros relacionados a la media y la desviación ajustados para cada estación para cada año. En Chadwick et al., 2018 se sugiere el análisis de las métricas de cambio para abordar los cambios proyectados desde una perspectiva de los percentiles y escenarios más o menos probables.
</p>


<div align="center">
  <img src="https://raw.githubusercontent.com/FelipeRivas5492/Generador-Climatico-Estacionario-y-No-Estacionario/main/OEPUCON.png" alt="PLOT_PUCON">
</div>
<p><strong>Figura 5</strong>: Serie anual de precipitación para finales de 2099 según la situación estacionaria y no estacionaria con generador climático para modelos probabilísticos con mejor ajuste según KS. Se muestran los estadísticos no estacionarios para P50, de acuerdo con las probabilidades de excedencia de cambios proyectados. </p>

https://www.youtube.com/watch?v=kCMFqDb-uXs







