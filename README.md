# inform-tica-m-dica-actividad
Interpretación de los siete indicadores
1. Número total de pacientes
La base reúne 20 pacientes. Cada persona aparece una sola vez, identificada con un código del P001 al P020. Este es el punto de partida del análisis: permite saber con cuántos registros se cuenta y calcular los porcentajes de las demás variables. Como se trata de un ejercicio con pocos datos ficticios, los resultados describen únicamente a este grupo; no deben generalizarse a un hospital real.
2. Edad promedio
La edad promedio es de 43 años, con edades que van desde los 19 hasta los 72 años. Esto muestra que se incluyeron adultos jóvenes y personas mayores, por lo que no todos los pacientes están en la misma etapa de la vida. Sin embargo, el promedio por sí solo no describe la situación de cada persona: hay edades bastante diferentes dentro del grupo.
3. Distribución por sexo
Se registraron 10 pacientes de sexo femenino (50 %) y 10 de sexo masculino (50 %). En esta base existe un equilibrio exacto entre ambas categorías. Este resultado ayuda a describir la composición del grupo, pero no permite afirmar que esa misma proporción se presente en las consultas de una institución de salud real.
4. Temperatura corporal promedio
La temperatura promedio es de 37,15 °C (valor original: 37,145 °C). La más baja fue de 36,4 °C y la más alta de 38,5 °C. Aunque el promedio se encuentra cercano a una temperatura corporal habitual, hay pacientes con valores más elevados, como P005 y P007. Esto recuerda que un promedio puede ocultar diferencias importantes entre personas. Una medición aislada no basta para establecer un diagnóstico.
5. Frecuencia cardíaca promedio
La frecuencia cardíaca promedio es de 86,05 latidos por minuto (lpm). Los registros van de 70 a 110 lpm. Por ejemplo, P009 tiene el valor más alto (110 lpm). Estos datos permiten observar variaciones entre pacientes, pero deben leerse junto con el motivo de consulta y otras circunstancias; no es correcto concluir que alguien está enfermo solamente por el número registrado.
6. Saturación de oxígeno promedio
La saturación promedio es de 97 %, calculada solo con los 19 pacientes que sí tienen este dato. El valor más bajo registrado fue 91 % (P009) y el más alto, 99 %. El registro de P009 merece atención dentro de la lectura descriptiva porque también corresponde a una consulta por dificultad respiratoria, pero el ejercicio no permite confirmar causas ni formular diagnósticos adicionales. El paciente P016 no tiene saturación registrada: su celda se dejó vacía y no se reemplazó por cero ni por un valor estimado.
7. Estado de atención
De los 20 registros, 9 pacientes tienen la atención finalizada (45 %), 7 aparecen en atención (35 %) y 4 están pendientes (20 %). Es decir, 11 pacientes (55 %) no figuran con atención finalizada en el momento representado por la base. Este indicador sirve para entender cómo se distribuyen los estados de los casos, pero no informa cuánto tiempo lleva cada paciente esperando ni por qué algunos siguen pendientes.
Inconsistencias encontradas y decisiones de limpieza
Al recibir los registros, la información no venía escrita de una sola manera. Era posible entenderla, pero habría sido difícil ordenarla, filtrarla o compararla sin una limpieza previa.
- Fechas con formatos diferentes: aparecían expresiones como 20/10/2026, 2026-10-22, 22/10/26, 2026/10/23 y «21 de octubre de 2026». Todas se normalizaron al formato AAAA-MM-DD, conservando la fecha original de cada consulta.
- Sexo expresado con distintas palabras: se utilizaron «mujer», «femenino», «F», «hombre», «masculino» y «M». Se unificaron a F y M para facilitar el conteo, sin alterar el dato recibido.
- Estados de atención redactados de formas distintas: por ejemplo, «Atención finalizada» y «Finalizada». Se dejaron únicamente las categorías Finalizada, En atención y Pendiente.
- Signos vitales con abreviaturas, separadores y unidades variadas: se encontraron T, «Temp.», «temperatura», FC, «pulso», SpO₂, «oxígeno» y «saturación». Además, algunos decimales estaban escritos con punto y otros con coma. Se organizaron en columnas específicas y como valores numéricos, con unidades indicadas en los encabezados.
- Un dato ausente: en P016 no se registró la saturación de oxígeno. La celda quedó en blanco. En consecuencia, el promedio de saturación utiliza 19 observaciones, no 20. Rellenar el espacio con cero o con un número supuesto habría distorsionado el análisis.
Estas diferencias son principalmente inconsistencias de formato y estandarización, no pruebas de que los pacientes estén mal registrados clínicamente. Tampoco se identificó información suficiente para verificar diagnósticos reales, pues todos los diagnósticos del ejercicio son simulados.
Reflexión sobre la privacidad clínica (100–150 palabras)
Cuando trabajamos con información clínica, es fácil concentrarnos en las cifras y olvidar que cada registro representa la historia de una persona. Por eso, proteger los datos no es solo cumplir una norma: también es una forma de respeto. Aunque este ejercicio utiliza pacientes ficticios, en una situación real evitaría compartir nombres, documentos, direcciones o cualquier detalle que permitiera identificar a alguien. Además, daría acceso a los archivos únicamente a las personas autorizadas y los guardaría de manera segura. Si tuviera que presentar resultados, preferiría utilizar cifras generales en vez de exponer historias individuales. También revisaría cuidadosamente los datos, porque un error o una información faltante puede cambiar lo que entendemos de un paciente. Este ejercicio me recuerda que organizar información de salud exige responsabilidad, discreción y cuidado por la confianza que las personas depositan en quienes manejan sus datos.





Descripción del trabajo realizado

Organización y análisis de una base de datos hospitalaria

1. Objetivo del trabajo

El objetivo de este trabajo fue aprender a organizar y analizar la información de 20 pacientes ficticios, utilizando Excel como herramienta principal. A partir de unos registros que estaban escritos de diferentes maneras, buscamos crear una base de datos más clara, ordenada y fácil de comprender.

Además de organizar la información, la idea fue aprender a interpretar los datos, identificar posibles errores o información incompleta y representar algunos resultados mediante gráficos. Este ejercicio nos permitió entender lo importante que es llevar un buen registro de los pacientes, ya que una información bien organizada facilita su revisión y ayuda a comprender mejor los datos relacionados con la atención en salud.

2. Diccionario de datos

Para organizar la información, utilizamos diez columnas. Cada una nos permitió registrar un dato específico de los pacientes y evitar que toda la información quedara mezclada.

Columna

¿Qué información contiene?

Código

Es el número que identifica a cada paciente, por ejemplo, P001.

Edad

Indica cuántos años tiene el paciente.

Sexo

Permite identificar si es femenino (F) o masculino (M).

Fecha de consulta

Señala el día en que el paciente recibió atención.

Motivo de consulta

Explica la razón por la que el paciente acudió al servicio de salud.

Temperatura (°C)

Registra la temperatura corporal del paciente.

Frecuencia cardíaca (lpm)

Indica cuántas veces late el corazón en un minuto.

Saturación de oxígeno (%)

Muestra el porcentaje de oxígeno registrado en la sangre.

Diagnóstico simulado

Presenta la condición de salud asignada al paciente dentro del ejercicio.

Estado de atención

Permite saber si la atención está pendiente, en proceso o finalizada.

Este diccionario nos ayudó a comprender qué significaba cada dato y por qué era importante ubicarlo correctamente dentro de la tabla.

3. Proceso de limpieza y organización de los datos

Antes de comenzar con el análisis, fue necesario revisar los 20 registros, porque algunos datos estaban escritos de diferentes formas. Por ejemplo, las fechas aparecían en distintos formatos, el sexo se encontraba como mujer, femenino, hombre o masculino y algunos valores de temperatura utilizaban puntos en lugar de comas.

Lo primero que hicimos fue organizar cada información en su columna correspondiente. Después, unificamos las fechas para que todas tuvieran el mismo formato, utilizamos las letras F y M para identificar el sexo y dejamos los estados de atención con los mismos nombres.

También revisamos los valores de temperatura, frecuencia cardíaca y saturación de oxígeno para que pudieran utilizarse en los cálculos de Excel.

Durante esta revisión encontramos que el paciente P016 no tenía registrada la saturación de oxígeno. Decidimos dejar ese espacio vacío, ya que no sería correcto inventar un valor solamente para completar la tabla.

Este proceso nos permitió comprender que limpiar una base de datos no significa cambiar la información, sino organizarla, corregir las diferencias en la forma de escribirla y respetar los datos originales.

4. Archivos entregados

Como resultado de esta actividad, se prepararon dos archivos:

Base_Datos_Hospital.xlsx

En este archivo de Excel se organizaron los datos de los 20 pacientes ficticios. Contiene una hoja llamada Pacientes, donde se encuentra la información ordenada, y otra llamada Análisis, destinada a presentar los resultados y facilitar su interpretación.

También se trabajó con gráficos para observar de manera más sencilla algunas características de los pacientes, como su distribución por sexo, el estado de atención y la frecuencia cardíaca.

analisis.md

En este archivo se presentan las interpretaciones de los resultados obtenidos, las inconsistencias encontradas en los registros y una reflexión sobre la importancia de proteger la información clínica.

Estos dos archivos permiten mostrar tanto la organización de los datos como lo que logramos comprender a partir de ellos.

5. Declaración de datos ficticios

Es importante aclarar que los 20 pacientes utilizados en este trabajo son completamente ficticios. Sus edades, motivos de consulta, signos vitales, diagnósticos y estados de atención fueron proporcionados únicamente para realizar una actividad académica.

Esto significa que no trabajamos con historias clínicas reales ni con información personal de pacientes verdaderos.

Aunque se trata de un ejercicio, nos permitió reconocer la responsabilidad que implica manejar información relacionada con la salud de las personas. Entendimos que los datos clínicos deben tratarse con cuidado, respeto y confidencialidad, porque detrás de cada historia clínica real hay una persona que tiene derecho a que su información sea protegida.

En conclusión, esta actividad no solo nos ayudó a practicar el uso de Excel, sino también a comprender la importancia de ser organizados, responsables y cuidadosos al trabajar con información en el área de la salud.
