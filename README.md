    
## Preguntas del Ejercicio Practico:

## ***1. El cliente X espera tener acuerdos de pago por valor de 8.000.000 de Pesos, basado en tu análisis de los datos el mes de Septiembre fue un mes en el que se cumplio el objetivo, fue bueno, malo, por que?***


<span style="color: yellow;">Durante el análisis de los datos del mes de septiembre, identifiqué un total de acuerdos de pago que alcanzaron $10,285,458.98. Sin embargo, observo que había duplicados en los registros. Esto puede atribuirse a diversos factores, como la participación de un mismo usuario en varias campañas o el incumplimiento de plazos.</span>

<span style="color: yellow;">Para obtener resultados más precisos, eliminé los duplicados y se conservé únicamente las propuestas más recientes que pertenecían a la misma deuda, siempre y cuando el monto fuera idéntico.</span>

<span style="color: yellow;">Como resultado, obtuve que en septiembre se alcanzó un total de $9,541,661.72 en acuerdos de pago. Este monto supera el objetivo establecido por el cliente, que era de $8,000,000.</span>

<span style="color: yellow;">En cuanto al cumplimiento del objetivo, el mes fue exitoso, ya que éste fué superado en un 19.27%.
Sin embargo para afirmar esto con mas precisión, me gustaría realizar las siguientes comparaciones:</span>

<span style="color: yellow;">1. Evaluar si el desempeño de septiembre es consistente con la media de acuerdos de pago a lo largo del año.</span>

<span style="color: yellow;">2. Comparar los resultados con septiembres de años anteriores para determinar si la mejora es sostenible.</span>

<span style="color: yellow;">3. Analizar cómo se compara septiembre con los otros meses del año en términos de acuerdos de pago.</span>

![evolucion objetivo acuerdos de pago](images/evolacuerdos.png)

[Acceso al Análisis](1.ipynb)

---

## ***2.Cual es el valor promedio de acuerdos de pago por usuario único para el mes de septiembre?***

<span style="color: yellow;">Basado en el análisis de los datos de acuerdos de pago para el mes de septiembre, observé que el valor promedio fue de $34,696.95. 

<span style="color: yellow;">Explorando los datos puedo observar que existen valores extremos (outliers), estos valores atípicos pueden afectar considerablemente el promedio</span>

![Outliers](images/boxplot.png)

<span style="color: yellow;">La mediana es una métrica que representa el valor que divide a la muestra en dos mitades iguales y  no se ve afectada por outliers. Proporciona una representación más precisa del monto de la mayoría de los acuerdos de pago, que  fué de $28,392.</span>

[Acceso al Análisis](2.ipynb)

---

## ***3.El cliente espera tener un 35% de contestación durante el mes de septiembre, según tu análisis cual fue el resultado de este ítem? Fue bueno o malo? y por que?***

<span style="color: yellow;">El resultado del porcentaje de contestación durante el mes de septiembre fue del 10.41%. Teniendo en cuenta el objetivo del cliente de alcanzar un 35%, este resultado puede considerarse malo.</span>

<span style="color: yellow;">Sin embargo este porcentaje se calcula con el número total de llamadas realizadas y las respuestas recibidas. Este cálculo puede no reflejar completamente la efectividad de las gestiones, ya que no tiene en cuenta el número de llamadas realizadas hasta lograr el contacto exitoso.</span>

![Contactación](images/barrascontactacion.png)

<span style="color: yellow;">Como se puede observar en el gráfico, mas del 40% de usuarios, requirió ser llamado 3 veces para lograr la contactación.</span>

<span style="color: yellow;">Por este motivo consideré relevante también, evaluar el porcentaje por usuario único. Al hacerlo, obtuve una métrica que proporciona una visión más precisa de cuántos usuarios se contactaron exitosamente durante el mes de septiembre, lo que puede ser más representativo de la efectividad de las gestiones.</span>

![Porcentaje de contactación](images/torta.png)

<span style="color: yellow;">Por lo tanto, el porcentaje de contestación del 10.41% es bajo en comparación con el objetivo del 35%. 
Considerando la métrica alternativa, el porcentaje de contestación por usuario único fue de 27.53%. Creo que este dato da una imagen más completa de la efectividad de las llamadas.</span>

[Acceso al Análisis](3.ipynb)

---

## ***4.De las llamadas contestadas se espera que al menos el 50% sean titulares, cuéntanos en el mes de septiembre, según tu análisis como estuvo este resultado?***

<span style="color: yellow;">En general, el porcentaje de llamadas contestadas fue del 55.09%. Considerando el campo "contactability_type" en el que, según el diccionario de datos, "Contacto Sí" confirma que se trata de un usuario titular.</span>

<span style="color: yellow;">Luego incluyo registros donde la titularidad se confirma a través de la columna "contact_confirmed," en este caso, se obtiene un resultado del 56.86%.</span>

<span style="color: yellow;">Continuando con el enfoque en el índice de contactabilidad, se procedió a eliminar las llamadas duplicadas que podrían distorsionar los datos. Esto se debe a que en las llamadas en las que el usuario no confirma ser titular o en las que atiende otra persona, es probable que se realicen nuevos intentos de llamada en futuras campañas. </span>

![Porcentaje de Titulares](images/donut.png)

<span style="color: yellow;">En este escenario, el porcentaje de contactación de titulares alcanza el 63.53%.</span>

[Acceso al Análisis](4.ipynb)

---

## ***5.Según tu análisis, Cuales son las horas en las que mas se realizan llamadas, en las que mas se contestan llamadas y en las que hay mas efectividad?***

<span style="color: yellow;">Visualizando los datos, podemos observar que las horas en las que se realizan más llamadas son entre las 10 y las 11 a. m., alcanzando su punto máximo a las 11 a. m.</span>

![horas con mas llamadas](images/PBI5.JPG)

<span style="color: yellow;">Las horas más efectivas en términos de respuesta y contactabilidad son de 13 a 15 horas. Sin embargo, la efectividad en la generación de compromisos de pago muestra su pico entre las 12 y las 13 horas.</span>

[Acceso al Análisis](PowerBI/Assessment%20Vozy.pbix)

---

## ***6.Cuales son los dos días de la semana mas efectivos para realizar las gestiones?***

![días mas efectivos](images/PBI6.JPG)

<span style="color: yellow;">Analizando los datos, podemos visualizar que los días más efectivos en términos de cantidad de llamadas contestadas, contactaciones, cantidad de acuerdos y monto de acuerdos son los martes y los miércoles.</span>

[Acceso al Análisis](PowerBI/Assessment%20Vozy.pbix)

---

## ***7.Porcentualmente cuales son los motivos de cuelgue en las llamadas?***

<span style="color: yellow;">El porcentaje de los motivos de las finalizaciones de las llamadas del mes de septiembre es el siguiente:</span>

![días mas efectivos](images/PBI7.JPG)

- <span style="color: yellow;">34.39%: Scheduled - Llamado que no ha sido respondido y se agenda para un nuevo intento.</span>
- <span style="color: yellow;">24.58%: Sent_to_Channel - Llamado sin responder.</span>
- <span style="color: yellow;">22.34%: Voicemail - Finalización luego del ingreso al correo de voz.</span>
- <span style="color: yellow;">10.99%: USER_HANGUP - Llamada finalizada por el usuario.</span>
- <span style="color: yellow;">7.27%: CALL_ENDED_PROPERLY - Llamada finalizada correctamente.</span>
- <span style="color: yellow;">0.43%: Otro.</span>

[Acceso al Análisis](PowerBI/Assessment%20Vozy.pbix)

---

## ***8.Cuales son los nodos en los que están terminando las llamadas no exitosas, pero que son contestadas.***

<span style="color: yellow;">En el siguiente analisis, se identificaron los nodos en los que están terminando las llamadas no exitosas, pero que son contestadas.

![días mas efectivos](images/PBI8.JPG)

<span style="color: yellow;">Detallo los 3 con la tasa mas alta:

<span style="color: yellow;">Nodo "1_welcome": En este nodo, un porcentaje significativo de llamadas no exitosas son contestadas. Posiblemente este sea un primer contacto.

<span style="color: yellow;">Nodo "2_voicemail": También se observa un número considerable de llamadas no exitosas que son contestadas en este nodo. Son llamadas contestadas por el VoiceMail

<span style="color: yellow;">Nodo "2_contact_yes_VENCIDA": Este grupo de llamadas no exitosas es posible que sea de llamados por recordatorios de vencimiento de propuestas de pago.

[Acceso al Análisis](PowerBI/Assessment%20Vozy.pbix)

---

## **Otras** **Preguntas**

***Teniendo en cuenta tu rol, donde vas a manejar mucha data que plataformas propondrías para hacer el manejo de esta información y poder presentar resultados de manera entendible para el cliente y que sea de fácil manejo?***

---

***En este momento las llamadas no están siendo ejecutadas dentro de la plataforma de Vozy, tenemos un ticket escalado al equipo de operaciones con el mismo, que acciones tomarías para priorizar este caso?***