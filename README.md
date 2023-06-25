# 10APLICATIVOS_MEDIDAS_JUNIO


Medidas definitivas  finales  con OZM tomadas el 6 de junio de 2023 

Comenzaron el dia 2023-06-09 a las 09:34:38+02:00 y terminaron el dia 2023-06-09  a las 13:36:19+02:00 en el Laboratorio de Electrotecnia de la  Escuela de Ingenieria Industrial de la Universidad de Almeria. Tambien se cosideran medidas unitarias del dia 6 del 6.Las Medidas  se realizan con 3  OpenZMeter  Trifásicos  (cada uno con 4 canales de medida)  conformando asi en total  11 canales de medida  que se distribuyen en los 10 aplicativos, mas el agregado.


En este respositorio se analizaran todas la medidas electricas  por medio de  3 OpenPowerMeter (OzM)  con soporte de 4 canales medidor ( en total 12 canales de medidas electricas),  conformando asi en total  11 canales utiles de los cuales 10 son paa aplicativos, uno  al agregado, y un ultimo vacante realizandose todas las meididas estos durante 4 horas a la maxima frecuencias de muestreo. 

Todo el proceso se realiza  en los cuadernos adjuntos a este repositorio fundamentalemnte versando en el analisis de las medidas de 10 aplicativos incluyendo transitorios  hasta el orden 150 de tension, corriente y potencia. 

Las medidas corresponden a W, VAR, VA,f, VLN,PF y A, mas los transititoros  hasta el orden 150 de W, V y A,   todas con un marca de tiempo (Timestamp) de 13 dígitos tipo UNIX Epox.

 
  
Para el  entrenamiento se  han definido tres periodos:

 - TRAIN(start="2023-06-09 09:34:00", end="2023-06-09 12:54:00")

 - VAL:(start="2023-06-09 12:55:00", end="2023-06-09 13:36:00")
 
 - TEST: (start="2023-06-06 11:19:19", end="2023-06-06 11:40:28")
 

Estos datos se entrenaron, tanto con el algoritmo CO, como el algoritmo FHMM.


Los aplicativos  usados en el experimento son los siguintes:

 1 -Main
 
2 - Electric Furnace ( Horno)

3- Microwave (Microonda)

4 - Television

5 - Bulb ( bombilla)

6 - Vacuum Cleaner ( Aspiradora)

7- Electric Space Heater ( Radiador de aceite)

8 - Electric Shower Heater  (Calentador de agua)

9 - Fan  ( Ventilador)

10 - Fridge  ( refrigerador)

11 -  Freezer (congelador)



## RESULTADOS FINALES
La rápida expansión de NILM y el desarrollo de diferentes algoritmos, han hecho que sea esencial proporcionar una evaluación de rendimiento mediante el uso de métricas de desempeño. Las métricas de evaluación, comparan los resultados de la desagregaciónn (predicciones) de los modelos entrenados con los datos del set de validación (mediciones reales de cada proceso). NILMTK cuenta con el cálculo de métricas de evaluación mediante el uso del MeterGroup para la validación de los resultados mediante el set de validación entes y lo mas variadas posibles. 

