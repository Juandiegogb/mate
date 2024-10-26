Para evaluar una integral, primero debemos saber si es **definida** o **indefinida**:

1. **Integral Indefinida**:
   - Una integral indefinida tiene la forma:
     \[
     \int f(x) \, dx
     \]
     Aquí, estamos buscando la **antiderivada** de \(f(x)\), es decir, una función \(F(x)\) tal que \(F'(x) = f(x)\).
   - El resultado se expresa como \(F(x) + C\), donde \(C\) es la **constante de integración**.

   Ejemplo:
   \[
   \int x^2 \, dx = \frac{x^3}{3} + C
   \]

2. **Integral Definida**:
   - Una integral definida tiene límites de integración:
     \[
     \int_{a}^{b} f(x) \, dx
     \]
     En este caso, calculamos la **diferencia del valor de la antiderivada \(F(x)\)** evaluada en \(b\) y en \(a\).
   - El resultado es un número, y representa el **área bajo la curva** de \(f(x)\) entre \(x = a\) y \(x = b\).

   Ejemplo:
   \[
   \int_{1}^{3} x^2 \, dx = \left[ \frac{x^3}{3} \right]_{1}^{3} = \frac{3^3}{3} - \frac{1^3}{3} = \frac{27}{3} - \frac{1}{3} = \frac{26}{3}
   \]

### Pasos Generales para Evaluar Integrales

1. **Simplifica la función integrando** si es posible, por ejemplo, usando identidades o propiedades algebraicas.
2. **Identifica una técnica adecuada de integración**, como:
   - Integración básica (antiderivadas directas).
   - Integración por partes.
   - Sustitución.
   - Integración por fracciones parciales.
   - Integración por trinomios cuadráticos y otros métodos avanzados.
3. **Aplica la técnica de integración** para obtener la antiderivada o el valor final si es una integral definida.
4. **Evalúa los límites de integración** (si es definida) en la antiderivada y resta los valores en los puntos de los límites.

Si tienes una integral específica o necesitas ayuda con algún método de integración en particular, ¡puedo ayudarte a resolverla!

El ejercicio que tienes busca evaluar el límite reconociendo una suma de Riemann.

El enunciado dice:

\[
\lim_{n \to \infty} \sum_{i=1}^{n} \frac{i^3}{n^4}
\]

### Paso 1: Relacionar con una suma de Riemann

Una suma de Riemann tiene la forma general:

\[
\sum_{i=1}^{n} f(x_i) \Delta x
\]

Donde:

- \( f(x_i) \) es la función que evaluamos en los puntos de la partición.
- \( \Delta x \) es el ancho de los intervalos.

Para relacionar la suma con una integral, necesitamos identificar los elementos de la suma de Riemann.

### Paso 2: Reescribir la suma

Sabemos que \( i/n \) representa un punto dentro del intervalo \([0, 1]\), por lo que podemos hacer las siguientes asociaciones:

- \( x_i = \frac{i}{n} \), que es el punto en el intervalo \([0, 1]\).
- \( \Delta x = \frac{1}{n} \), ya que estamos dividiendo el intervalo \([0, 1]\) en \(n\) partes.

Por lo tanto, la suma se puede escribir como:
\[
\sum_{i=1}^{n} \left( \frac{i}{n} \right)^3 \cdot \frac{1}{n}
\]

### Paso 3: Expresar como una integral

Cuando \(n \to \infty\), la suma de Riemann se convierte en la integral de \( f(x) = x^3 \) en el intervalo \([0, 1]\). Es decir:

\[
\lim_{n \to \infty} \sum_{i=1}^{n} \left( \frac{i}{n} \right)^3 \cdot \frac{1}{n} = \int_0^1 x^3 \, dx
\]

### Paso 4: Calcular la integral

La integral de \(x^3\) es:

\[
\int_0^1 x^3 \, dx = \left[ \frac{x^4}{4} \right]_0^1 = \frac{1^4}{4} - \frac{0^4}{4} = \frac{1}{4}
\]

### Respuesta final

El valor del límite es \( \frac{1}{4} \).

Para calcular el valor promedio de una función \( f(t) \) en un intervalo \([a, b]\), usamos la fórmula:

\[
f_{\text{prom}} = \frac{1}{b - a} \int_{a}^{b} f(t) \, dt
\]

En tu caso, la función es \( f(t) = e^{\sin t} \cos t \) y el intervalo es \([0, \pi/2]\). Por lo tanto:

\[
f_{\text{prom}} = \frac{1}{\frac{\pi}{2} - 0} \int_{0}^{\frac{\pi}{2}} e^{\sin t} \cos t \, dt
\]

Simplificando el factor:

\[
f_{\text{prom}} = \frac{2}{\pi} \int_{0}^{\frac{\pi}{2}} e^{\sin t} \cos t \, dt
\]

### Evaluación de la integral

Observamos que la integral \(\int_{0}^{\frac{\pi}{2}} e^{\sin t} \cos t \, dt\) se puede simplificar haciendo un cambio de variable:

1. Sea \( u = \sin t \).
2. Entonces, \( du = \cos t \, dt \).

Cuando \( t = 0 \), \( u = 0 \), y cuando \( t = \frac{\pi}{2} \), \( u = 1 \).

Entonces, la integral se transforma en:

\[
\int_{0}^{\frac{\pi}{2}} e^{\sin t} \cos t \, dt = \int_{0}^{1} e^u \, du
\]

La antiderivada de \( e^u \) es \( e^u \), así que:

\[
\int_{0}^{1} e^u \, du = \left[ e^u \right]_0^1 = e^1 - e^0 = e - 1
\]

### Sustituyendo en el valor promedio

Ahora sustituimos el resultado de la integral:

\[
f_{\text{prom}} = \frac{2}{\pi} (e - 1)
\]

### Respuesta final

El valor promedio de la función \( f(t) = e^{\sin t} \cos t \) en el intervalo \([0, \pi/2]\) es:

\[
f_{\text{prom}} = \frac{2}{\pi} (e - 1)
\]

Para resolver este ejercicio, sigamos los pasos indicados:

### Paso 1: Identificar las curvas y el intervalo

Las funciones dadas son:

- \( y = e^x \)
- \( y = x^2 - 1 \)

El intervalo de integración está definido entre \( x = -1 \) y \( x = 1 \).

### Paso 2: Graficar las funciones y determinar la región encerrada

1. La función \( y = e^x \) es una función exponencial creciente.
2. La función \( y = x^2 - 1 \) es una parábola que abre hacia arriba y está desplazada hacia abajo en 1 unidad.

Al graficarlas, observaremos que la función \( y = e^x \) está por encima de \( y = x^2 - 1 \) en el intervalo \([-1, 1]\).

### Paso 3: Plantear la integral para el área de la región

Para encontrar el área entre las dos curvas en el intervalo \([-1, 1]\), restamos la función inferior de la función superior e integramos en el intervalo:

\[
\text{Área} = \int_{-1}^{1} \left( e^x - (x^2 - 1) \right) \, dx
\]

Simplificamos la expresión dentro de la integral:

\[
\text{Área} = \int_{-1}^{1} \left( e^x - x^2 + 1 \right) \, dx
\]

### Paso 4: Resolver la integral

Ahora, evaluamos cada término de la integral:

\[
\text{Área} = \int_{-1}^{1} e^x \, dx - \int_{-1}^{1} x^2 \, dx + \int_{-1}^{1} 1 \, dx
\]

1. **Integral de \( e^x \):**
   \[
   \int_{-1}^{1} e^x \, dx = \left[ e^x \right]_{-1}^{1} = e^1 - e^{-1} = e - \frac{1}{e}
   \]

2. **Integral de \( x^2 \):**
   \[
   \int_{-1}^{1} x^2 \, dx = \left[ \frac{x^3}{3} \right]_{-1}^{1} = \frac{1}{3} - \frac{(-1)^3}{3} = \frac{1}{3} + \frac{1}{3} = \frac{2}{3}
   \]

3. **Integral de \( 1 \):**
   \[
   \int_{-1}^{1} 1 \, dx = \left[ x \right]_{-1}^{1} = 1 - (-1) = 2
   \]

### Paso 5: Sustituir y simplificar

Finalmente, sumamos los resultados de cada término:

\[
\text{Área} = \left( e - \frac{1}{e} \right) - \frac{2}{3} + 2
\]

### Respuesta final

El área de la región encerrada es:

\[
\text{Área} = e - \frac{1}{e} + \frac{4}{3}
\]


**¡Claro! Aquí está la respuesta en español:**

**Ejercicio 17-20:**

Expresa cada uno de los siguientes límites como una integral definida sobre el intervalo dado.

**17.**

```
lim(n→∞) Σ(i=1 to n) [x_i * ln(1 + x_i^2) * Δx]
```

**Intervalo:**

```
[2, 6]
```

