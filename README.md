# QM2515
Programas de la materia Intruducción a la Quimiometría.
# Programa #1: Calcula el pH de una Solución
Dada la concentración de iones H+.

En este código, primero importo la biblioteca `math` para utilizar funciones matemáticas, en particular el logaritmo base 10, necesario para calcular el pH. Defino la función `calcular_pH`, que recibe la concentración de iones H+ y verifica que sea un valor positivo, retornando un mensaje de error si no lo es, y calculando el pH en caso contrario.

Solicito al usuario la concentración de iones H+ a través de un input, convirtiendo la entrada a número flotante. Luego, calculo el pH con la función previamente definida y muestro el resultado con dos decimales, proporcionando así una respuesta clara y precisa al usuario.

# Programa #2: Determina los Moles de Cualquier Compuesto

Desarrollé un programa que pudiera calcular la cantidad de moles de un compuesto químico dado, basándome en su masa y masa molar. Para ello, diseñé una función que realiza este cálculo dividiendo la masa del compuesto entre su masa molar, y añadí una comprobación para asegurarme de que la masa molar no fuera un valor cero o negativo. En la parte principal del programa, creé una interfaz de usuario sencilla que pide el nombre del compuesto, su masa y su masa molar, y luego muestra la cantidad de moles calculada. Implementé también un manejo de errores para capturar cualquier entrada inválida, como valores no numéricos o masas molares incorrectas. Aseguré que el programa solo se ejecutara de manera directa.

# Programa #3: Calcula la Concentración de Cualquier Compuesto (Moles/Litros)

Hice un programa para calcular cuánto de un compuesto hay en una solución. Primero, creé una parte que hace el cálculo dividiendo los moles del compuesto entre los litros de la solución, pero me aseguré de que los litros no fueran cero para evitar errores. Luego, en la parte principal, el programa le pide al usuario que diga cómo se llama el compuesto, la cantidad de moles y el volumen de la solución, y después usa esa información para decir cuánto compuesto hay en cada litro de solución. Si el usuario se equivoca y pone algo que no debería, el programa le dice que hubo un error. Al final, me aseguré de que el programa solo funcione cuando lo ejecutas directamente y probé que todo estuviera funcionando bien.

# Programa #4: Calcula el Rendimiento Porcentual de una Reacción

A partir de los rendimientos reales y teóricos.

Desarrollé un programa sencillo para ayudar a calcular el rendimiento porcentual en reacciones químicas, una medida que compara la cantidad de producto que realmente se obtuvo con la cantidad máxima que se podría haber obtenido. Para hacer esto, creé una función que realiza el cálculo dividiendo el rendimiento real entre el rendimiento teórico y multiplicando por 100. Me aseguré de incluir una verificación para evitar dividir por cero en caso de que el rendimiento teórico fuera cero. En la parte principal del programa, se le pide al usuario que ingrese los valores del rendimiento real y teórico, y luego se utiliza la función para calcular y mostrar el rendimiento porcentual. Si el usuario introduce algo incorrecto, como un texto en lugar de un número, el programa le informa del error. Todo esto asegura que el programa sea fácil de usar y proporcione resultados precisos.

# Programa #5: Calcula el pH de una Solución Tampón

Para ayudar a calcular el pH de soluciones tampón, creé un programa basado en la ecuación de Henderson-Hasselbalch, una fórmula fundamental en química que relaciona el pH de una solución con las concentraciones de un ácido débil y su base conjugada. La ecuación es:

pH = pKa + log(Base conjugada / Ácido débil)

Donde `pKa` es una constante específica del ácido débil en cuestión. Esta fórmula es especialmente útil para soluciones tampón porque permite predecir cómo cambiará el pH al agregar pequeñas cantidades de ácido o base. En el programa, utilicé la librería `math` de Python para realizar el cálculo del logaritmo necesario en la fórmula. El programa está estructurado para ser interactivo, solicitando al usuario que introduzca el pKa, así como las concentraciones del ácido débil y su base conjugada, para luego mostrar el pH calculado. Además, incluí medidas para manejar posibles errores. En resumen, este programa permite calcular el pH de soluciones tampón, aprovechando la utilidad y precisión de la ecuación de Henderson-Hasselbalch.

# Programa #6: Predice si un Compuesto Será Soluble o Insoluble Usando su Valor de Kps

Para analizar la solubilidad de un compuesto en una solución específica, desarrollé un programa en Python que calcula el producto de solubilidad, (Q), y lo compara con la constante de producto de solubilidad, (Ksp). El programa es sencillo y fácil de seguir. Inicialmente, solicita al usuario que introduzca el valor de (Ksp), una constante conocida para cada compuesto. Posteriormente, pide las concentraciones de dos iones distintos en la solución, así como sus coeficientes estequiométricos en la reacción de disociación.

La función `calcular_Q` toma estas concentraciones y coeficientes, calculando el producto de solubilidad, (Q), elevando cada concentración a su respectivo coeficiente y multiplicando los resultados. Este valor de (Q) nos proporciona una visión clara de la interacción entre los iones en la solución.

<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?\Large&space;Q=[\text{Ion}_1]^{\text{coef}_1}\cdot[\text{Ion}_2]^{\text{coef}_2}" title="\Large Q=[\text{Ion}_1]^{\text{coef}_1}\cdot[\text{Ion}_2]^{\text{coef}_2}" />
</p>

Tras calcular (Q), el programa lo compara con (Ksp). Si Q > Ksp, se espera que la solución esté sobresaturada y que pueda formarse un precipitado. Si Q = Ksp, la solución se considera saturada pero aún soluble. Finalmente, si Q < Ksp, la solución se considera insaturada y completamente soluble.

# Programa #7: Predice los Grados de Insaturación en Compuestos Orgánicos
El programa propio que decidí crear sirve para calcular el número de insaturaciones (DBE) en una molécula orgánica.

![Ecuación de Grados de Insaturación](https://latex.codecogs.com/svg.latex?DBE=C+\frac{N}{2}+1-\frac{H}{2}-\frac{X}{2})

donde \( C \) representa los átomos de carbono, \( N \) los de nitrógeno, \( H \) los de hidrógeno y \( X \) los de halógenos. El programa inicia solicitando al usuario que introduzca la cantidad de cada tipo de átomo en la molécula. Luego, utiliza una función que aplica la fórmula para calcular el número de insaturaciones. Finalmente, muestra el resultado al usuario. Si se introduce un valor no entero, el programa notifica al usuario para que ingrese un valor válido.Este programa proporciona una herramienta sencilla para entender mejor la estructura de las moléculas orgánicas a través de su grado de insaturación.

# Programa #8. A: Calcula el Seno y el Coseno de un Ángulo Sin Usar el Módulo Math

Cree un programa para calcular el seno y el coseno de un ángulo sin utilizar el módulo `math` de Python, optando en su lugar por las series de Taylor, una herramienta matemática que permite aproximar funciones a través de una suma de términos polinómicos.

Para ello, creé funciones que calculan el factorial de un número, el seno y el coseno de un ángulo en radianes. La serie de Taylor fue la técnica elegida porque proporciona una manera de aproximar funciones trigonométricas mediante una serie infinita de términos polinómicos, lo cual es especialmente útil cuando no se dispone de funciones trigonométricas directas como las del módulo `math`.

En el programa, el usuario introduce un ángulo en grados, que luego se convierte a radianes para ser compatible con las series de Taylor. Posteriormente, se calculan y muestran el seno y el coseno del ángulo utilizando las funciones previamente definidas. La elección de usar 10 términos en las series fue un balance entre precisión y simplicidad, aunque este número puede ajustarse según las necesidades específicas.

# Programa #8. B: Calcula el Seno y el Coseno de un Ángulo Usando el Módulo Math

Elaboré un programa utilizando Python para calcular el seno y el coseno de un ángulo, aprovechando las funciones integradas en el módulo `math`. Inicialmente, importé este módulo para acceder a sus herramientas matemáticas avanzadas. El usuario es solicitado a ingresar un ángulo en grados, que posteriormente es convertido a radianes utilizando la constante π, también obtenida del módulo `math`. Acto seguido, el programa hace uso de las funciones `sin` y `cos` para calcular el seno y el coseno del ángulo dado, respectivamente. Para finalizar, los resultados son presentados al usuario, redondeados a cuatro decimales para una mejor visualización. Este método resulta ser más eficiente y preciso, ya que se basa en funciones ya optimizadas y de alta precisión proporcionadas por el módulo `math` de Python.

# Comparación de Resultados

Para realizar una comparación efectiva entre los resultados de los códigos, es esencial ejecutar ambos utilizando el mismo ángulo y analizar cuidadosamente los valores obtenidos. En la mayoría de los casos, especialmente con ángulos pequeños y un número adecuado de términos en las series de Taylor, los resultados tienden a ser muy similares. Sin embargo, es importante tener en cuenta que las series de Taylor son aproximaciones y, por lo tanto, pueden presentar diferencias notables, especialmente con ángulos más grandes o con un número reducido de términos en la serie. Esto se debe a las limitaciones inherentes a la precisión de los cálculos computacionales y a la naturaleza de las series de Taylor. Por otro lado, el módulo math de Python emplea métodos optimizados y precisos para calcular funciones trigonométricas, proporcionando resultados más exactos y confiables. En resumen, aunque para la mayoría de los ángulos los resultados del seno y el coseno serán muy cercanos o presentarán variaciones mínimas, es crucial tener en cuenta estas consideraciones al comparar los resultados obtenidos mediante diferentes métodos.

# Programa #9: Determina Cuando el Seno y el Coseno de un Ángulo son Iguales

Finalmente, creé un código en Python que permite comparar el seno y el coseno de un ángulo específico. El programa inicia convirtiendo el ángulo ingresado de grados a radianes mediante la función `radians` del módulo `math`. Posteriormente, procede a calcular tanto el seno como el coseno del ángulo en cuestión. Para abordar la limitada precisión de los cálculos con punto flotante, establecí una tolerancia de 1 x 10^-8. Si la diferencia absoluta entre el seno y el coseno resulta ser menor que esta tolerancia, el programa interpreta los valores como aproximadamente iguales y comunica este resultado al usuario. En caso contrario, el programa proporciona los valores específicos del seno y el coseno. La interacción con el usuario es sencilla: se le pide que introduzca el ángulo deseado y el programa se encarga del resto.


