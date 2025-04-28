# LAB2_202373504-3

Nombres:
    Lucas Ansieta M. Rol: 202373504-3. Paralelo 200.
    Bastián Garcés C. Rol: 202373510-8. Paralelo 200.

Entornos de desarrollo: Logisim (Windows).

Instrucciones de ejecución:

    Abrir mapa.circ en Logisim.
    Ir al circuito main.
    Seleccionar la herramienta de "mano".
    Hacer clic en los pines de entrada (A, B, C, D) para establecer la combinación binaria (0000 a 1111).
    Observar el símbolo resultante en el Display de 7 Segmentos.

Consideraciones para la ejecución:

    Usar versión compatible de Logisim.
    Asegurar simulación activa.

Justificación de Decisiones o Supuestos

    Interpretación de Entradas y Salidas: Se asumió que la entrada de 4 bits (A, B, C, D en Logisim) representa el número binario de la habitación (0 a- 15), siendo el bit más significativo el de mayor peso (por ejemplo, A es el MSB). La salida de 7 bits corresponde a los segmentos del display (a a g) según la nomenclatura de la Figura 2, donde un '1' indica que el segmento debe estar encendido.

    Mapeo Habitación -> Símbolo: La correspondencia exacta entre el número de habitación, el paciente/acción y el símbolo a mostrar en el display se extrajo directamente de la Tabla de Pacientes (Sección 2.1.1) y las figuras del diccionario de símbolos (Figuras 3 y 4). Este mapeo fue la base para construir la Tabla de Verdad completa.

    Construcción de la Tabla de Verdad: Se generó una Tabla de Verdad que cubre las 16 posibles combinaciones de entrada (0000 a 1111), y para cada una, se determinó el patrón de 7 bits de salida (los estados ON/OFF de los segmentos a-g) necesario para formar el símbolo correspondiente según el diccionario. Esta tabla es la especificación funcional completa del circuito.

    Minimización de Funciones: Para obtener la implementación lógica más simple y eficiente (minimizando el número de compuertas), se aplicó el método de Mapas de Karnaugh a la Tabla de Verdad para cada una de las 7 salidas (cada segmento).

    Implementación en Logisim: El circuito se implementó en Logisim utilizando la estructura de Suma de Productos (SOP) resultante de la minimización, empleando compuertas lógicas básicas (AND, OR, NOT).

