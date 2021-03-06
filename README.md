# TT2

Este repositorio contiene los archivos de la interfaz de usuario, creada en python 3.9, así como los programas de Algoritmo Genético y Enjambre de Partículas.
Tambien contiene la versión de prueba del calculo de Hipervolumen. A continuación se describiran cada uno de los programas ya mencionados.

## GUI
Nombre del archivo: GUI_TT_MIOPTION.py <br>
La implementación de la GUI fue realizada con la biblioteca de PySimpleGUI, la cual fue seleccionada por su simplicidad de uso.
La interfaz gráfica permite al usuario seleccionar el sistema a sintonizar, ingresar los parámetros dinámicos característicos de cada sistema, así como sleccionar el algoritmo metaheurístico deseado, posteriormente se deberán ingresar los parámetros necesarios de cada algoritmo, según sea el caso.
Al aceptar la ejeción del algoritmo seleccionado, se presentará la aproximación al frente de Pareto junto con una tabla que presenta el conjunto de soluciones inmejorables obtenidas por el algoritmo evolutivo.
Por último se puede seleccionar cualquier conjunto de ganancias y simular el comportamiento dinámico del péndulo seleccionado presionando el botón de simular, la simulación mostrará dos pestañas, una con la animación del comportamiento esperado y otra con las gráficas de posición, velocidad y señal de alimentación.

Librerias requeridas: <br>

* drawnow versión 0.72.5
* ipython versión 8.0.1
* matplotlib versión 3.4.3
* mplcursors versión 0.5.1
* numpy versión 1.21.2
* PySimpleGUI versión 4.56.0
* PySimpleGUIQt versión 0.35.0
* scipy versión 1.7.1

## Algoritmo Genético

Nombre de los archivos:<br>

* MOGA_PD_ARCHIVE.py
* MOGA_PI_ARCHIVE.py
* MOGA_PS_ARCHIVE.py

Ests programas contienen el Algoritmo Genétco aplicado a los 3 sistemas, en el primero, aplicado al péndulo doble, el segundo aplicado al péndulo invertido y el último aplicado al péndulo simple. Todos estos programas dan como resultado la aproximación al frente de Pareto, así como una versión preliminar del cálculo de Hipervolumen.

Las bibliotecas requeridas: <br>

* matplotlib versión 3.4.3
* numpy versión 1.21.2

## Enjambre de Partículas

Nombre de los archivos:

* MOPSO_FrentePareto.py
* MOPSO_PD_ARCHIVE.py
* MOPSO_PI_ARCHIVE.py

De igual manera, cada programa corresponde a una versión preliminar del calculo de Hipervolumen aplicado al péndulo simple, doble e invertido respectivamente.
Las librerias requeridas: <br>

* matplotlib versión 3.4.3
* numpy versión 1.21.2

## Hipervolumen

Los resultados de las ejecuciones de HIPERVOLUMEN, así como los programas usados para obtenerlos se encuentran en dentro de la carpeta Hipervolumen.
Dentro de esta carpeta se encuentran 3 carpetas, las cuales se enlistas a continuación:<br>

* pendulo-doble
* pendulo-invertido
* pendulo-simple

Dentro de cada carpeta se encunetran los programas ejecutados, es decir, se encuntra un programa por cada algoritmo (Evolución Diferencial, Algotimo Gnético y Algoritmo de Enjambre de Partículas), así como los resultados obtenidos de las ejeciones del calculo de Hipervolumen.
Los archivos de resultados se encuentra en formato txt, mismos que fueron usados para la prueba de Wilcoxon.
Esta prueba nos brindo una manera adecuada de realizar la comparación de manera adecuada entre algoritmos.
