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


Se dispone de
Dataset original: BBDD_Hospitalización.csv
Notebook Preprocesamiento de datos: ProyectoIntegrador1M6
Dataset procesado (Usado en el segundo notebook 'ProyectoIntegrador1BM': BBDD_HospitalizaciónB.csv
Notebook Modelo Machine Learning: ProyectoIntegrador1BM6

Se identifica que los atributos 'Fiebre' 'PSA', son los mas determinantes para poder clasificar a un paciente como hospitalizado o no dentro del 
estudio realizado

![atributos](https://github.com/harlantonguino/HospitalizacionML/assets/9009541/cded8738-e04a-42f4-8eb0-797c4413152e)

Finalmente al validar las metricas obtenidas (Accuracy: 0.991 (+/- 0.006)) con el modelo propuesto se decide no evaluar otros modelos alternativos 

![matrix de confusion](https://github.com/harlantonguino/HospitalizacionML/assets/9009541/75bfdcd5-e68c-47bd-bfb4-384e30856383)

Cabve resaltar que el preprocesamiento de los datos es fundamental para obtener un buen performance en el modelo final

