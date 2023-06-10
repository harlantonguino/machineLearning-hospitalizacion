# HospitalizacionML
Machine Learning en Medicina: Al aplicar Machine Learning en Medicina se pueden usar las herramientas informáticas, con el fin de conseguir 
información a partir de los datos, por ejemplo, de historias clínicas o registros de prestadores de servicios de salud. De esta manera, se 
pueden emitir diagnósticos predicitivos, evaluar la efectividad de estrategias de intervención y anticipar comportamientos en escenarios 
relacionados con la atención.

Se desea saber las características más importantes que tienen los pacientes de cierto tipo de enfermedad que terminan en hospitalización. 
Fue definido como caso aquel paciente que fue sometido a biopsia prostática y que en un periodo máximo de 30 días posteriores al procedimiento 
presentó fiebre, infección urinaria o sepsis; requiriendo manejo médico ambulatorio u hospitalizado para la resolución de la complicación y 
como control al paciente que fue sometido a biopsia prostática y que no presentó complicaciones infecciosas en el período de 30 días posteriores
al procedimiento. Dado que tienen en su base de datos algunos datos referentes a los pacientes y resultados de exámenes diagnósticos, de pacientes
hospitalizados y no hospitalizados, nos han entregado esta información.  

Se ha recopilado `Antecedentes del paciente`, `Morbilidad asociada al paciente` y `Antecedentes relacionados con la toma de la biopsia`y 
`Complicaciones infecciosas`. En la siguiente tabla, se encuentra un diccionario de datos asociado:

![image](https://user-images.githubusercontent.com/118769777/220240501-8c21461d-2de5-495b-954e-10fb9bf38014.png)


Se disponibiliza:<br>
1. Dataset original: BBDD_Hospitalización.csv<br>
2. Notebook Preprocesamiento de datos (normalizacion, limpieza): ProyectoIntegrador1M6<br>
3. Dataset procesado (usado en el segundo notebook 'ProyectoIntegrador1BM'): BBDD_HospitalizaciónB.csv<br>
4. Notebook Modelo Machine Learning (modelamiento, evaluacion): ProyectoIntegrador1BM6<br>

<br>
<br>
Se identifica que los atributos 'Fiebre' 'PSA', son los mas determinantes para poder clasificar a un paciente como hospitalizado o no dentro del 
estudio realizado<br>

![atributos](https://github.com/harlantonguino/HospitalizacionML/assets/9009541/cded8738-e04a-42f4-8eb0-797c4413152e)

Se identifica la exahustividad (recall) como la metrica objetivo con la cual validasremos nuestro modelo debido a que por la naturaleza del problema 
se busca minimizar los falsos negativos, considerando que seria mas grave predecir un paciente como NO Hospitalizado y que en realidad SI sea Hospitalizado<br>

Finalmente al validar la exahustividad (Recall: 1)) con el modelo propuesto y obtener un valor satisfactorio para dicha metrica se decide no evaluar otros modelos alternativos<br>

![matrix de confusion](https://github.com/harlantonguino/HospitalizacionML/assets/9009541/75bfdcd5-e68c-47bd-bfb4-384e30856383)

Cabve resaltar que el preprocesamiento de los datos es fundamental para obtener un buen performance en el modelo final

