# **Ecuaciones y Sistemas**

---

## **1. Introducción**
Una **ecuación** es una igualdad con una o más incógnitas que se cumple para ciertos valores de esas incógnitas.  
Resolver una ecuación significa **encontrar todos los valores de la incógnita** que hacen verdadera la igualdad.

Un **sistema de ecuaciones** es un conjunto de dos o más ecuaciones que comparten las mismas incógnitas. Resolver el sistema significa **encontrar todos los valores que satisfacen todas las ecuaciones al mismo tiempo**.

---

## **2. Ecuaciones de primer grado**
$ax + b = 0, \quad a \neq 0$

**Pasos para resolver:**
1. Pasar el término independiente: $ax = -b$  
2. Dividir entre $a$: $x = -\frac{b}{a}$

**Ejemplo:**  
$3x+5=0 \implies x=-\frac{5}{3}$

---

## **3. Ecuaciones de segundo grado**
$ax^2 + bx + c = 0, \quad a \neq 0$

### **3.1 Fórmula general**
$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

**Ejemplo:**  
$x^2 -5x +6 = 0 \implies x=2,3$

### **3.2 Factorización**
$x^2 -5x +6 = (x-2)(x-3) =0$

### **3.3 Discriminante**
- $\Delta = b^2-4ac$  
- $\Delta>0$: dos soluciones reales distintas  
- $\Delta=0$: solución real única  
- $\Delta<0$: soluciones complejas

---

## **4. Ecuaciones de grado mayor que 2**
Ecuaciones cúbicas ($x^3$), cuárticas ($x^4$) o superiores.

### **Estrategias**
1. Factor común  
2. Agrupación  
3. Uso de raíces enteras/racionales  
4. Sustitución para reducir a cuadrática

**Ejemplo:**  
$x^3 -6x^2 +11x -6 =0$  
- Probar raíces: 1,2,3  
- Factorización: $(x-1)(x-2)(x-3)=0$  
- Soluciones: $x=1,2,3$

---

## **5. Ecuaciones racionales**
Ecuaciones con fracciones algebraicas: $\frac{P(x)}{Q(x)}=0$

**Pasos:**
1. Determinar el dominio ($Q(x)\neq 0$)  
2. Multiplicar por el MCD para eliminar denominadores  
3. Resolver la ecuación resultante  
4. Comprobar soluciones dentro del dominio

**Ejemplo 1:** $\frac{x-2}{x+1}=0 \implies x=2$  

**Ejemplo 2:** $\frac{1}{x-1} + \frac{2}{x+2}=0$  
- MCD: $(x-1)(x+2)$  
- Multiplicar: $(x+2)+2(x-1)=0 \implies x=0$  
- Dominio: $x\neq1,-2$ → solución válida

---

## **6. Ecuaciones exponenciales**
$a^{f(x)} = a^{g(x)}, \quad a>0, a\neq1$

**Pasos:**
1. Igualar exponentes si base igual: $f(x)=g(x)$  
2. Resolver la ecuación resultante  
3. Si bases diferentes, usar logaritmos: $b^{f(x)}=c \implies f(x)=\log_b c$

**Ejemplos:**
- Base igual: $2^{3x-1}=2^{x+3} \implies x=2$  
- Base distinta: $3^x=5 \implies x=\log_3 5$

---

## **7. Sistemas de ecuaciones lineales (2x2)**

$$
\begin{cases}
a_1 x + b_1 y = c_1 \\
a_2 x + b_2 y = c_2
\end{cases}
$$

### **Métodos**
1. **Sustitución**: despejar una variable y sustituir  
2. **Igualación**: despejar la misma variable y igualar expresiones  
3. **Reducción/Combinación**: sumar/restar ecuaciones para eliminar variable  
4. **Determinantes (Cramer)**

**Ejemplo:**  
$$
\begin{cases}x+y=5 \\ 2x-y=1\end{cases} \implies x=2, y=3
$$

---

## **8. Sistemas de ecuaciones no lineales**

Contienen al menos una ecuación no lineal.

### **Estrategias**
1. Sustitución  
2. Reducción / combinación  
3. Factorización  
4. Logaritmos para exponenciales

**Ejemplo:**  
$$
\begin{cases}y=2x+1 \\ x^2+y^2=25\end{cases}
$$
- Sustituir: $x^2+(2x+1)^2=25 \implies 5x^2 +4x -24=0$  
- Soluciones: $(2,5), (-12/5,-19/5)$

