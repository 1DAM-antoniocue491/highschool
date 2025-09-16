# Números Reales
## 1. ¿Qué son los números reales?

Los **números reales** engloban todos los números que se pueden representar en la recta numérica. Se componen de dos bloques principales:

- **Números racionales** ($\mathbb{Q}$): se pueden escribir como fracción $\displaystyle \frac{p}{q}$ con $p,q\in\mathbb{Z}$ y $q\neq 0$.  
  Ejemplos: $\displaystyle \frac{3}{4},\; -2,\; 0.75,\; 0.\overline{3}$ (decimal periódico).

- **Números irracionales**: no se pueden escribir como fracción; su desarrollo decimal no es periódico y no termina.  
  Ejemplos: $\sqrt{2},\; \pi,\; e$.

Por tanto: $\displaystyle \mathbb{R}=\mathbb{Q}\cup\{\text{irracionales}\}$.

---

## 2. Recta numérica y clasificación

Los reales se colocan sobre la recta numérica.  

Ejemplos de clasificación:

- $2$ es entero → racional.  
- $0.333\ldots = 0.\overline{3}$ → racional.  
- $\sqrt{2}\approx 1.4142135\ldots$ → irracional.

---

## 3. Intervalos

Se usan para indicar subconjuntos de $\mathbb{R}$.

- **Abierto:** $(a,b)=\{x\in\mathbb{R}: a<x<b\}$.  
- **Cerrado:** $[a,b]=\{x\in\mathbb{R}: a\le x\le b\}$.  
- **Semiabiertos:** $[a,b)\quad\text{o}\quad(a,b]$.  
- **Infinitos:** $(-\infty,a),\ (a,\infty)$. (No se usa $[-\infty,\cdot]$ como intervalo cerrado en $-\infty$.)

Ejemplo: $[0,1]$ contiene $0$ y $1$; $(0,1)$ no.

---

## 4. Potencias (exponentes)

Si $a$ es un número y $n$ entero:

- $a^0=1\quad(\text{si }a\neq 0)$.  
- $a^1=a$.  
- $a^m\cdot a^n=a^{m+n}$.  
- $(a^m)^n=a^{mn}$.  
- $(ab)^n=a^n b^n$.  
- $a^{-n}=\dfrac{1}{a^n}\quad(\text{si }a\neq0)$.

**Ejemplo:** $2^3\cdot 2^{-1}=2^{3-1}=2^2=4$.

**Fracciones y potencias:** $\left(\dfrac{2}{3}\right)^2=\dfrac{4}{9}$.

---

## 5. Potencias con exponentes fraccionarios — relación con radicales

Si $m,n\in\mathbb{Z}$, $n>0$, entonces $a^{\frac{m}{n}}=\sqrt[n]{a^m}=\bigl(\sqrt[n]{a}\bigr)^m$, siempre que esté bien definida (por ejemplo, $a\ge 0$ si $n$ es par para la raíz real principal).

**Ejemplo:** $8^{\frac{2}{3}}=(\sqrt[3]{8})^2=2^2=4$.

---

## 6. Radicales

- **Notación**: $\sqrt[n]{a}$ es la raíz $n$-ésima de $a$.  
	>- índice: $n$ (si no aparece se entiende $n=2$).  
	>- radicando: $a$.
- **Raíz principal**: $\sqrt[n]{a}$ se toma no negativa si $n$ es par y $a\ge 0$.  
- Para $n$ par: $\sqrt[n]{a^n}=|a|$.  
	 **Ejemplo**: $\sqrt{(-3)^2}=\sqrt{9}=3=|{-3}|$.
- Para $n$ impar: $\sqrt[n]{a^n}=a$.

**Ejemplos:** $\sqrt{9}=3,\qquad \sqrt[3]{-8}=-2$.

---

## 7. Simplificar radicales (extraer factores)

Idea: factorizar el radicando en potencias perfectas del índice.

**Ejemplo 1:** $\sqrt{18}$  
$18=9\cdot 2,\quad 9$ es cuadrado perfecto.  
$\sqrt{18}=\sqrt{9\cdot 2}=\sqrt{9}\,\sqrt{2}=3\sqrt{2}$.

**Ejemplo 2:** $\sqrt[3]{54}$  
$54=27\cdot 2,\quad 27=3^3$.  
$\sqrt[3]{54}=\sqrt[3]{27\cdot 2}=3\sqrt[3]{2}$.

**Regla:** si $a=b^n\cdot r$ entonces $\sqrt[n]{a}=b\sqrt[n]{r}$.

---

## 8. Operaciones con radicales

### Suma y resta
Sólo se pueden combinar directamente radicales **semejantes** (mismo índice y mismo radicando).

Ejemplo: $3\sqrt{2}+5\sqrt{2}=8\sqrt{2}$.  
Pero $\sqrt{2}+\sqrt{3}$ no se simplifica.

**Truco:** simplifica primero: $\sqrt{18}+\sqrt{72}=3\sqrt{2}+6\sqrt{2}=9\sqrt{2}$.

### Producto
$\sqrt[n]{a}\cdot\sqrt[n]{b}=\sqrt[n]{ab}$ (Ej.: $\sqrt{2}\cdot\sqrt{8}=\sqrt{16}=4$).

### Cociente
$\dfrac{\sqrt[n]{a}}{\sqrt[n]{b}}=\sqrt[n]{\dfrac{a}{b}}\quad(b>0)$ (Ej.: $\dfrac{\sqrt{50}}{\sqrt{2}}=\sqrt{25}=5$).

### Potencias de radicales
$(\sqrt[n]{a})^m=a^{m/n}$ (Ej.: $(\sqrt{3})^4=3^{4/2}=3^2=9$).

### Radical de radical
$\sqrt[m]{\sqrt[n]{a}}=\sqrt[mn]{a}$.

---

## 9. Radicales con índices distintos

Para operar con índices distintos, usa exponentes fraccionarios y un común denominador: $\sqrt[a]{x}=x^{1/a},\qquad \sqrt[b]{x}=x^{1/b}$.

**Ejemplo:** $\sqrt[3]{2}=2^{1/3}=2^{2/6}=(2^{1/6})^2$, mientras que $\sqrt[6]{2}=2^{1/6}$. No son semejantes directamente sin transformar exponentes.

---

## 10. Racionalizar denominadores

Objetivo: quitar radicales del denominador.

- **Caso simple:** $\dfrac{a}{\sqrt{b}}\;\longrightarrow\;\dfrac{a}{\sqrt{b}}\cdot\dfrac{\sqrt{b}}{\sqrt{b}}=\dfrac{a\sqrt{b}}{b}$.  
  Ejemplo: $\dfrac{3}{\sqrt{2}}=\dfrac{3\sqrt{2}}{2}$.

- **Caso binomial (usar el conjugado):**  
  $\dfrac{1}{\sqrt{2}+\sqrt{3}}\cdot\dfrac{\sqrt{2}-\sqrt{3}}{\sqrt{2}-\sqrt{3}}=\dfrac{\sqrt{2}-\sqrt{3}}{2-3}=\dfrac{\sqrt{2}-\sqrt{3}}{-1}=\sqrt{3}-\sqrt{2}$.
