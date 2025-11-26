[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=ClaudiaX14/PracticaFinal_MSF)

# Práctica Final: Sistema respiratorio con bronquitis.

## Información de la estudiantes

Claudia X. Castro [22212252]; L22212252@tectijuana.edu.mx

Yuliana J. Navarrete [21212170]; L21212170@tectijuana.edu.mx

Daniela Castillo [22212251]; L22212251@tectijuana.edu.mx

Lugo Valenzuela Liliana Fernanda [21212165]; L21212165@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos

1. Convertir el diagrama mecánico al diagrama eléctrico.
2. Calcular la función de transferencia aplicando el principio de superposición.
3. Calcular el error en estado estacionario y la estabilidad en lazo abierto.
4. Emular y simular la respuesta del circuito en Simulink/Simscape a la señal impulso unitario.
5. Sintonizar las ganancias de un controlador PID para eliminar el error entre la entrada y la salida del sistema control-caso.
6. Obtener la respuesta en lazo abierto y en lazo cerrado con el controlador PID en Spyder/Python con la función de transferencia.

## Descripción detallada del sistema

El modelo eléctrico utilizado representa la mecánica del sistema respiratorio mediante una analogía basada en resistencias, inductores y capacitores. La entrada del sistema, Ve(t), corresponde a una señal tipo impulso, empleada para simular un esfuerzo inspiratorio breve generado por el diafragma.
Esta señal se aplica antes del inductor L, el cual representa la inercia del aire en las vías respiratorias centrales; este componente modela el hecho de que los cambios en la presión no producen variaciones instantáneas en el flujo debido a la masa del aire en movimiento.
Después del inductor, el flujo atraviesa la resistencia Re, que representa la oposición al paso del aire en la tráquea y bronquios principales. Posteriormente se encuentran los elementos que representan la zona bronquial y alveolar:
la resistencia Ra, asociada a la oposición al flujo en los bronquios más pequeños, y el capacitor Ca, que modela la capacidad de expansión de los alvéolos.

De forma complementaria, el capacitor Cn representa la capacidad del tejido respiratorio periférico para almacenar parte del volumen inspirado.
La salida del sistema, Vs(t), corresponde a la tensión medida después de Ra y Ca, y se interpreta como la presión alveolar resultante.

Modelo sano (control)
En el modelo correspondiente a un individuo sano, las resistencias mantienen valores bajos y los capacitores presentan una capacidad elevada, lo que refleja vías respiratorias desobstruidas y alvéolos que se expanden con facilidad.
 Esto permite que el flujo de aire avance sin dificultad hacia los alvéolos, generando una respuesta de salida Vs(t) más rápida y de mayor amplitud.

 Modelo con bronquitis (caso)
En el modelo patológico, la bronquitis se representa mediante un aumento significativo en la resistencia Ra debido a inflamación y acumulación de moco en los bronquios más pequeños.
 Al mismo tiempo, el capacitor Ca toma un valor menor, lo cual representa una disminución en la capacidad de expansión alveolar.
Como consecuencia:
una mayor porción de la presión de entrada Ve(t) se disipa antes de llegar a los alvéolos, el capacitor Ca se carga más lentamente, y la ventilación se vuelve menos eficiente, lo que produce una salida Vs(t)de menor amplitud y con un retardo más notable en comparación con el modelo sano.


Palabras clave: Musculo; Esqueleto; Controlador PI; Tratamiento; Control


## Referencias

\[1] National Heart, Lung and Blood Institute (NHLBI), “Bronquitis,” NHLBI, 12-ene-2023. [En línea]. Disponible: https://www.nhlbi.nih.gov/es/salud/bronquitis. [Accedido: 25-nov-2025]. 
