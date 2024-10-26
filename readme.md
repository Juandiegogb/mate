Para convertir este ejercicio en formato Markdown con notación matemática, aquí tienes la respuesta detallada:

---

## Solución

### Integral Definida o Indefinida

Para evaluar una integral, primero debemos saber si es **definida** o **indefinida**:

1. **Integral Indefinida**:
   - Una integral indefinida tiene la forma:
     \[
     \int f(x) \, dx
     \]
     Aquí, estamos buscando la **antiderivada** de \( f(x) \), es decir, una función \( F(x) \) tal que \( F'(x) = f(x) \).
   - El resultado se expresa como \( F(x) + C \), donde \( C \) es la **constante de integración**.

   Ejemplo:
   \[
   \int x^2 \, dx = \frac{x^3}{3} + C
   \]

2. **Integral Definida**:
   - Una integral definida tiene límites de integración:
     \[
     \int_{a}^{b} f(x) \, dx
     \]
     En este caso, calculamos la **diferencia del valor de la antiderivada \( F(x) \)** evaluada en \( b \) y en \( a \).
   - El resultado es un número, y representa el **área bajo la curva** de \( f(x) \) entre \( x = a \) y \( x = b \).

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

---

### Ejercicio: Suma de Riemann y Límite

Dado el siguiente límite:

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

Sabemos que \( \frac{i}{n} \) representa un punto dentro del intervalo \([0, 1]\), por lo que podemos hacer las siguientes asociaciones:

- \( x_i = \frac{i}{n} \), que es el punto en el intervalo \([0, 1]\).
- \( \Delta x = \frac{1}{n} \), ya que estamos dividiendo el intervalo \([0, 1]\) en \( n \) partes.

Por lo tanto, la suma se puede escribir como:
\[
\sum_{i=1}^{n} \left( \frac{i}{n} \right)^3 \cdot \frac{1}{n}
\]

### Paso 3: Expresar como una integral

Cuando \( n \to \infty \), la suma de Riemann se convierte en la integral de \( f(x) = x^3 \) en el intervalo \([0, 1]\). Es decir:

\[
\lim_{n \to \infty} \sum_{i=1}^{n} \left( \frac{i}{n} \right)^3 \cdot \frac{1}{n} = \int_0^1 x^3 \, dx
\]

### Paso 4: Calcular la integral

La integral de \( x^3 \) es:

\[
\int_0^1 x^3 \, dx = \left[ \frac{x^4}{4} \right]_0^1 = \frac{1^4}{4} - \frac{0^4}{4} = \frac{1}{4}
\]

### Respuesta final

El valor del límite es \( \frac{1}{4} \).
