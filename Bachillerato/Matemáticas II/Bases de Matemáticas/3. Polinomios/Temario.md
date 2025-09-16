# **Polinomios**

## 1. Introducción a los polinomios
Un **polinomio** es una expresión algebraica formada por la suma o resta de monomios:

$P(x) = a_n x^n + a_{n-1} x^{n-1} + \dots + a_1 x + a_0$

- $a_i$ = coeficientes (números reales)  
- $x$ = variable  
- $n$ = grado del polinomio (mayor exponente)  

**Ejemplo:** $P(x) = 3x^4 - 5x^3 + 2x - 7$ → grado 4, 4 términos

**Clasificación según número de términos:**  
- Monomio: 1 término ($5x^3$)  
- Binomio: 2 términos ($x+2$)  
- Trinomio: 3 términos ($x^2 + x + 1$)  
- Polinomio general: más de 3 términos  

**Términos semejantes:** mismos exponentes de la variable.  
**Ejemplo:** $3x^2 + 5x - 2x^2 +4 = x^2 +5x +4$

---

## 2. Operaciones con polinomios

### 2.1 Suma y resta
Se suman o restan los **términos semejantes**.  

**Ejemplo suma:** $(2x^3 + 3x^2 - x +4) + (x^3 - x^2 +5x -1) = 3x^3 + 2x^2 +4x +3$  

**Ejemplo resta:** $(3x^3 -2x^2 +x -5) - (x^3 +4x^2 -2x +1) = 2x^3 -6x^2 +3x -6$

### 2.2 Multiplicación
Multiplicar cada término de un polinomio por todos los términos del otro.  

**Ejemplo:** $(x+2)(x^2+3x+4) = x^3 +5x^2 +10x +8$

---

## 3. Productos notables y potencia de un binomio

| Producto notable | Fórmula | Ejemplo |
|-----------------|---------|---------|
| Cuadrado de un binomio | $(a+b)^2 = a^2 +2ab + b^2$ | $(x+3)^2 = x^2 +6x +9$ |
| Diferencia de cuadrados | $a^2 - b^2 = (a-b)(a+b)$ | $x^2-9 = (x-3)(x+3)$ |
| Cubo de un binomio | $(a+b)^3 = a^3 +3a^2b +3ab^2 + b^3$ | $(x+2)^3 = x^3 +6x^2 +12x +8$ |
| Cubo de una diferencia | $(a-b)^3 = a^3 -3a^2b +3ab^2 - b^3$ | $(x-1)^3 = x^3 -3x^2 +3x -1$ |
| Producto de binomios | $(x+a)(x+b) = x^2 + (a+b)x + ab$ | $(x+2)(x+3) = x^2 +5x +6$ |

---

## 4. División de polinomios

### 4.1 División larga
Se utiliza para dividir $P(x)$ entre $D(x)$ de igual o menor grado:  

$P(x) = D(x) \cdot Q(x) + R(x)$  

**Pasos:**
1. Ordenar polinomios por grado descendente  
2. Dividir primer término del dividendo entre primer término del divisor → primer término del cociente  
3. Multiplicar divisor por ese término y restar del dividendo  
4. Bajar siguiente término y repetir hasta que grado del resto < grado divisor  

**Ejemplo:** dividir $x^3 +2x^2 -x -2$ entre $x-1$  
- $\frac{x^3}{x} = x^2$ → multiplicar $(x-1)x^2 = x^3 - x^2$ → restar: $3x^2 - x$  
- $\frac{3x^2}{x} = 3x$ → multiplicar $(x-1)3x = 3x^2 -3x$ → restar: $2x$  
- Bajar $-2$: $2x -2$ → $\frac{2x}{x}=2$ → multiplicar $(x-1)2=2x-2$ → restar: $0$  

**Resultado:** $Q(x) = x^2 +3x +2$, $R(x)=0$

### 4.2 Método de Ruffini
Divide $P(x)$ entre $(x-a)$ de forma rápida:  

**Pasos:**
1. Escribir coeficientes de $P(x)$  
2. Llevar primer coeficiente hacia abajo  
3. Multiplicar por $a$ y sumar al siguiente coeficiente  
4. Repetir hasta el último → resto

**Ejemplo:** $x^3 -6x^2 +11x -6$ entre $x-1$ ($a=1$)

| Coeficientes | 1 | -6 | 11 | -6 |
|--------------|---|----|----|----|
| Llevar abajo | 1 |    |    |    |
| Multiplicar  |   | 1  | -5 | 6  |
| Sumar        | 1 | -5 | 6  | 0  |

- Cociente: $x^2 -5x +6$, resto: 0 → $x-1$ es factor  

**Ejemplo adicional:** $2x^3 +3x^2 -5x -6$ entre $x+2$ ($a=-2$)

| Coeficientes | 2 | 3 | -5 | -6 |
|--------------|---|---|----|----|
| Llevar abajo | 2 |   |    |    |
| Multiplicar  |   | -4 | 2 | 6  |
| Sumar        | 2 | -1 | -3 | 0 |

- Cociente: $2x^2 - x -3$, resto: 0 → $x+2$ es factor

---

## 5. Teorema del Resto y raíces de un polinomio

### 5.1 Teorema del Resto
Si se divide $P(x)$ entre $(x-a)$, el **resto** es $P(a)$:  

$P(x) = (x-a) \cdot Q(x) + R \implies R = P(a)$

- Si $P(a) = 0$ → resto = 0 → $(x-a)$ es factor

**Ejemplo:** $P(x) = x^3 -6x^2 +11x -6$, dividir entre $x-1$  

$P(1)=1-6+11-6=0$ → $x-1$ es factor

### 5.2 Raíces o ceros
- Raíz: $r$ tal que $P(r)=0$  
- Cada raíz $r$ → $(x-r)$ es factor lineal  
- Un polinomio de grado $n$ puede tener como máximo $n$ raíces reales

**Ejemplo:** $P(x)=x^3 -6x^2 +11x -6$  
- Posibles raíces: divisores de $-6$: $\pm1, \pm2, \pm3, \pm6$  
- Verificación: $P(1)=0$, $P(2)=0$, $P(3)=0$  
- Factorización completa: $P(x)=(x-1)(x-2)(x-3)$

### 5.3 Relación con Ruffini
- Último número en Ruffini = resto = $P(a)$  
- Si resto = 0 → $a$ es raíz → $(x-a)$ factor

### 5.4 Estrategia para encontrar raíces
1. Probar divisores del término independiente  
2. Evaluar con Teorema del Resto  
3. Dividir el polinomio por el factor encontrado  
4. Repetir hasta factorizar completamente

**Ejemplo completo:** $P(x) = x^3 -6x^2 +11x -6 = (x-1)(x-2)(x-3)$

---

## 6. Factorización de polinomios
- Factor común: $ax + ay = a(x+y)$  
- Agrupación: $(x^3+x^2) + (x+1) = x^2(x+1)+1(x+1)=(x+1)(x^2+1)$  
- Productos notables: $x^2-9=(x-3)(x+3)$  
- Usando raíces conocidas: si $r$ es raíz → $P(x)=(x-r)Q(x)$  

**Ejemplo:** $x^3-6x^2+11x-6 = (x-1)(x-2)(x-3)$

---

## 7. Fracciones algebraicas
- Cociente de polinomios: $\frac{P(x)}{Q(x)}$  
- Simplificación: factorizar y cancelar factores comunes  
- Suma y resta: mínimo común denominador  
- Multiplicación: $\frac{P}{Q} \cdot \frac{R}{S} = \frac{PR}{QS}$  
- División: $\frac{P}{Q} \div \frac{R}{S} = \frac{P \cdot S}{Q \cdot R}$  

**Ejemplo:**  
$\frac{x^2-1}{x^2+2x+1} = \frac{(x-1)(x+1)}{(x+1)^2} = \frac{x-1}{x+1}$

