# Funciones y modelos funcionales

---

## 1. Introducción: ¿qué es una función?
Una **función** es una regla que a cada valor de una variable independiente $x$ (del **dominio**) le asigna **uno y solo un** valor $y=f(x)$ (del **recorrido** o **imagen**).

- Notación: $f: D \to \mathbb{R}$, $x \mapsto f(x)$.
- **Dominio**: conjunto de $x$ para los que $f(x)$ está definida.
- **Recorrido (rango)**: conjunto de valores que toma $f(x)$.
- **Ejemplo:** $f(x)=x^2$ tiene dominio $\mathbb{R}$ y recorrido $[0,\infty)$.

---

## 2. Características generales de una función

**2.1 Dominio y recorrido**  
- Determinar el dominio: eliminar divisores cero, raíces pares con radicando negativo, logaritmos con argumento $\le 0$, etc.  
- Calcular el recorrido mediante análisis (factorización, vértices, límites, etc.)

**2.2 Intersecciones**
- **Corte con el eje $x$ (ceros / raíces):** resolver $f(x)=0$.  
- **Corte con el eje $y$:** $f(0)$ (si existe).

**2.3 Paridad y periodicidad**
- **Par:** $f(-x)=f(x)$ → simetría respecto al eje $y$.  
- **Impar:** $f(-x)=-f(x)$ → simetría respecto al origen.  
- **Periódica:** existe $T>0$ tal que $f(x+T)=f(x)$ para todo $x$ (ej. funciones trigonométricas).

**2.4 Continuidad y discontinuidades**
- **Continuidad** en $a$: $\lim_{x\to a} f(x)=f(a)$.  
- Discontinuidades: salto, asintótica (por ejemplo vertical en racionales), removible (hueco).

**2.5 Crecimiento/monotonía**
- **Creciente** en un intervalo si $x_1<x_2 \implies f(x_1)\le f(x_2)$ (estricto si $<$).  
- **Decreciente** análogo.

**2.6 Tendencia y tasa de variación**
- **Tasa de variación media** entre $x=a$ y $x=b$:
  $$
  \frac{\Delta f}{\Delta x} = \frac{f(b)-f(a)}{b-a}.
  $$
  Ejemplo: para $f(x)=x^2$ entre $1$ y $3$: $\frac{9-1}{2}=4$.
- **Tasa de variación instantánea** (concepto de derivada): límite
  $$
  f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}.
  $$
  (Si no usas cálculo formal, basta con la interpretación: pendiente instantánea).

---

## 3. Operaciones con funciones

Dadas $f,g$ con dominios adecuados:

- **Suma:** $(f+g)(x)=f(x)+g(x)$  
- **Resta:** $(f-g)(x)=f(x)-g(x)$  
- **Producto:** $(f\cdot g)(x)=f(x)\,g(x)$  
- **Cociente:** $\left(\dfrac{f}{g}\right)(x)=\dfrac{f(x)}{g(x)}$ (si $g(x)\neq 0$)  
- **Composición:** $(f\circ g)(x)=f(g(x))$ — ojo al dominio: $x$ debe pertenecer al dominio de $g$ y $g(x)$ al dominio de $f$.
- **Función inversa:** $f^{-1}$ existe sólo si $f$ es biyectiva (inyectiva + sobreyectiva). Si $f$ es estrictamente monotónica y continua en su dominio es inyectiva; para encontrar $f^{-1}$ se resuelve $y=f(x)$ despejando $x$ en función de $y$.

**Ejemplo de composición:**  
$f(x)=\sqrt{x+1}$ y $g(x)=2x$.  
$(f\circ g)(x)=f(2x)=\sqrt{2x+1}$; dominio: $2x+1\ge0\Rightarrow x\ge -\frac12$.

---

## 4. Funciones polinómicas

**Definición:** $p(x)=a_n x^n + \dots + a_1 x + a_0$, $a_n\neq 0$, grado $n$.

**Propiedades:**
- Dominio: $\mathbb{R}$.  
- Comportamiento extremo (end behavior): determinado por $a_n$ y $n$ par/impar:
  - Si $n$ par: mismos signos al infinito ($+\infty$ o $-\infty$ según $a_n$).
  - Si $n$ impar: signo opuesto en $+\infty$ y $-\infty$.
- **Ceros y multiplicidad:** si $(x-r)^m$ es factor, $r$ es raíz de multiplicidad $m$; si $m$ es par el gráfico "toca" la abscisa; si impar la cruza.
- **Número máximo de raíces reales:** $n$.
- **Derivadas** (si conoces cálculo) ayudan a localizar extremos y puntos de inflexión.

**Ejemplo: cuadrática**
- $f(x)=ax^2+bx+c$.
- Vértice: $x_v = -\frac{b}{2a}$, $y_v=f(x_v)$.  
- Eje de simetría: $x=x_v$.
- Si $a>0$ abre hacia arriba (mínimo), si $a<0$ abre hacia abajo (máximo).

**Ejemplo resuelto:** $f(x)=x^3-3x^2-9x+27$ → factoriza (buscar raíces) etc.

---

## 5. Funciones racionales

**Definición:** $R(x)=\dfrac{P(x)}{Q(x)}$ con $P,Q$ polinomios y $Q\not\equiv0$.

**Aspectos clave:**

- **Dominio:** $\{x\in\mathbb{R}: Q(x)\neq 0\}$.  
- **Holes (agujeros) y asíntotas verticales:**  
  - Si un factor $(x-a)$ cancela en numerador y denominador → hueco en $x=a$ (discontinuidad removible).  
  - Si factor no se cancela → asíntota vertical en $x=a$.
- **Asíntotas horizontales/oblicuas:**  
  - Compare grados $n=\deg P$, $m=\deg Q$:
    - $n<m$: asíntota horizontal $y=0$.
    - $n=m$: asíntota horizontal $y=\frac{\text{coeficiente líder }P}{\text{coeficiente líder }Q}$.
    - $n=m+1$: asíntota oblicua / lineal (obténla dividiendo polinomios).
    - $n>m+1$: asíntota de grado mayor (polinomio de grado $n-m$).
- **Signo:** se analiza por intervalos considerando ceros y polos.

**Ejemplo:**  
$R(x)=\dfrac{x^2-1}{x-1}$. Simplificar: $R(x)=\dfrac{(x-1)(x+1)}{x-1} = x+1$ para $x\ne1$. Hay un hueco en $x=1$; la función coincide con la recta $y=x+1$ salvo en $x=1$.

**Ejemplo de asíntota oblicua:**  
$\dfrac{2x^2+3x+1}{x-1}$ → división: $2x+5 + \dfrac{6}{x-1}$ → asíntota oblicua $y=2x+5$.

---

## 6. Funciones exponenciales

**Forma básica:** $f(x)=a^{x}$ con base $a>0$, $a\neq1$.

**Propiedades:**
- Dominio: $\mathbb{R}$. Recorrido: $(0,\infty)$.  
- Si $a>1$ → crecimiento exponencial (crece al aumentar $x$).  
- Si $0<a<1$ → decrecimiento exponencial (decaimiento).
- **Ley de potencias:** $a^{x+y}=a^x a^y$, $a^{-x}=1/a^x$.
- **Constante $e\approx 2.7182818$**: función $e^x$ tiene propiedades especiales (derivada igual a la función misma en cálculo).

**Modelos exponenciales (aplicaciones):**
- Crecimiento poblacional (modelo simple): $N(t)=N_0 e^{rt}$.
- Decaimiento radioactivo: $A(t)=A_0 e^{-kt}$.
- Interés compuesto continuo: $A=P e^{rt}$.

**Ajuste de datos (linealización):**
- Para ajustar $y=A\cdot b^x$, aplicar logaritmo: $\ln y = \ln A + x \ln b$ → recta en escala semilog.

---

## 7. Funciones definidas a trozos (por tramos)

**Definición:** función cuya expresión cambia según el intervalo de $x$.

**Ejemplo clásico: valor absoluto**
$$
|x| = \begin{cases}
-x & x<0,\\
0 & x=0,\\
x & x>0.
\end{cases}
$$

**Puntos a comprobar:**
- **Continuidad** en los puntos límite entre tramos: comprobar límites laterales y valor de la función.  
- **Derivabilidad** (si procede): la derivada lateral debe coincidir para ser derivable.

**Ejemplo práctico:**  
$$
f(x)=\begin{cases}
x^2 & x\le 1,\\
2x+1 & x>1.
\end{cases}
$$
- Verificar continuidad en $x=1$: $f(1^-)=1$, $f(1^+)=3$ → discontinuidad de salto → no continua.

---

## 8. Tendencia y tasa de variación media (ampliación práctica)

**Interpretación física:** la tasa de variación media es el promedio de la variación de la magnitud por unidad de tiempo (o por unidad de variable).

**Ejemplo numérico completo:**
$f(t)=100(1.05)^t$ (inversión con interés compuesto anual del 5%).  
Tasa media entre $t=0$ y $t=3$:
$$
\frac{f(3)-f(0)}{3-0} = \frac{100(1.05)^3 - 100}{3} \approx \frac{115.7625 -100}{3} \approx 5.25417\ \text{(unidades por año)}.
$$

---

## 9. Modelos funcionales: elegir y ajustar modelos

**Modelos comunes y cuándo usarlos:**

- **Lineal:** $y=mx+b$ → relación proporcional + desplazamiento; buena primera aproximación; tasa de cambio constante.
- **Polinómico (ej. cuadrático):** $y=ax^2+bx+c$ → curvatura (máximos/mínimos), trayectorias con aceleración constante.
- **Exponencial:** $y=Ae^{kx}$ → crecimiento/decadencia multiplicativo.
- **Potencia (ley de potencias):** $y=Ax^b$ → relaciones de escala, alometría; log-log lineariza: $\ln y=\ln A + b\ln x$.
- **Logístico:** $y=\dfrac{L}{1+e^{-k(x-x_0)}}$ → crecimiento con saturación (capacidad máxima $L$), usado en poblaciones y difusión.
- **Trigonometricas:** $y=A\sin(\omega x+\phi)+C$ → fenómenos periódicos.

**Pasos para modelar datos reales:**
1. **Plot de dispersión**: ver forma (lineal, curvo, crecimiento, saturación).  
2. **Probar transformaciones**:
   - Semilog (log en $y$) → si recta entonces exponencial.
   - Log-log (log en $x$ e $y$) → si recta entonces potencia.
3. **Ajuste por mínimos cuadrados / regresión** (si tienes herramientas).  
4. **Comprobar residuos**: deberían distribuirse aleatoriamente (sin patrón).  
5. **Interpretación de parámetros**: ej. en $y=Ae^{kx}$, $k$ es tasa de crecimiento instantánea; $A$ valor inicial.  
6. **Validación**: usar parte de los datos para test; cuidado con extrapolación.

**Consejos prácticos:**
- No sobreajustes (evitar polinomios de grado excesivo sólo porque ajustan datos).
- Preferir modelos simples y explicables.
- Reportar unidades y escala.

---

## 10. Inversas, composición y condiciones (resumen práctico)

- Para que $f^{-1}$ exista: $f$ debe ser **inyectiva**. Un método práctico: restringir dominio de funciones no-inyectivas (ej. $\sqrt{x}$ es inversa de $x^2$ si dominio restringido a $x\ge0$).
- Composición: $(f\circ g)^{-1} = g^{-1}\circ f^{-1}$ (si ambas inversas existen).
- Atención a dominios al componer o invertir.

---

## 11. Ejemplos resueltos (varios)

### Ejemplo A — Tasa media
$f(x)=x^2+2x$, entre $x=1$ y $x=4$:
$$
\frac{f(4)-f(1)}{4-1} = \frac{(16+8)-(1+2)}{3}=\frac{24-3}{3}=7.
$$

### Ejemplo B — Composición e inversa
$f(x)=2x+1, \ g(x)=x^2$ (dominio $\mathbb{R}$).  
$(f\circ g)(x)=f(x^2)=2x^2+1$.  
$f^{-1}(y)=\frac{y-1}{2}$ (existe porque $f$ es lineal inyectiva). $g^{-1}$ no existe globalmente (no inyectiva), pero restricta a $x\ge0$ tiene $g^{-1}(y)=\sqrt{y}$.

### Ejemplo C — Racional con asíntota
$R(x)=\dfrac{2x^2+3x+1}{x-1}$. División:  
$2x^2+3x+1 = (x-1)(2x+5) +6$.  
Por tanto $R(x)=2x+5 + \dfrac{6}{x-1}$. Asíntota oblicua: $y=2x+5$; asíntota vertical: $x=1$.

### Ejemplo D — Ajuste exponencial (linealización)
Datos: $(x,y)=(0,2),(1,4),(2,8)$ → parece $y=2\cdot 2^x$. Tomando ln: $\ln y = \ln 2 + x \ln 2$ → recta con pendiente $\ln 2$.
