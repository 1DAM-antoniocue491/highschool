# **Inecuaciones**

---

## **1. Introducción a las inecuaciones**
Una **inecuación** es una desigualdad matemática que contiene una o más incógnitas.  
Se diferencia de una ecuación en que representa una **relación de orden**:

- Mayor que: $>$  
- Mayor o igual que: $\geq$  
- Menor que: $<$  
- Menor o igual que: $\leq$  

**Ejemplo:**  
$$
x+3 > 5 \implies x > 2
$$

---

## **2. Reglas fundamentales**
Al resolver inecuaciones, aplicamos reglas similares a las ecuaciones, salvo una excepción importante:

- Si multiplicamos o dividimos **ambos lados por un número negativo**, se **invierte el signo de la desigualdad**.

**Ejemplo:**  
$$
-2x > 6 \implies x < -3
$$

---

## **3. Inecuaciones de primer grado con una incógnita**
Son de la forma:
$$
ax+b > 0, \quad ax+b < 0, \quad ax+b \geq 0, \quad ax+b \leq 0
$$

### **Ejemplo 1**
$$
2x - 5 \leq 7 \implies 2x \leq 12 \implies x \leq 6
$$

### **Ejemplo 2 (con signo negativo)**
$$
-3x + 4 > 10 \implies -3x > 6 \implies x < -2
$$

**Representación gráfica:**  
La solución se representa en la recta real mediante intervalos abiertos $(\ )$ o cerrados $[\ ]$ según corresponda.

---

## **4. Inecuaciones de grado mayor o igual que 2**
Incluyen polinomios cuadráticos, cúbicos o de grado superior.

### **Método de intervalos**
1. Pasar todo a un lado: $P(x) \geq 0$  
2. Factorizar $P(x)$  
3. Calcular las raíces  
4. Estudiar el signo del polinomio en cada intervalo  
5. Escoger los intervalos que cumplen la condición

---

### **Ejemplo 1: cuadrática**
$$
x^2 - 5x + 6 > 0
$$

1. Factorización: $(x-2)(x-3) > 0$  
2. Raíces: $x=2,3$  
3. Intervalos: $(-\infty,2), (2,3), (3,\infty)$  
4. Signos:  
   - $x=1$: $(1-2)(1-3)=(-)(-) >0$ ✔  
   - $x=2.5$: $(+)(-) <0$ ✘  
   - $x=4$: $(+)(+) >0$ ✔  

**Solución:** $(-\infty,2) \cup (3,\infty)$

---

### **Ejemplo 2: cúbica**
$$
x^3 - x^2 -6x \leq 0
$$

1. Factor común: $x(x^2 - x -6) \leq 0$  
2. Factorizar: $x(x-3)(x+2) \leq 0$  
3. Raíces: $x=-2, 0, 3$  
4. Intervalos: $(-\infty,-2), (-2,0), (0,3), (3,\infty)$  
5. Signos:  
   - $x=-3$: $(-)(-)(-)=-$ ✔  
   - $x=-1$: $(-)(-)(+)=+$ ✘  
   - $x=1$: $(+)(-)(+)= -$ ✔  
   - $x=4$: $(+)(+)(+)=+$ ✘  

**Solución:** $(-\infty,-2] \cup [0,3]$

---

## **5. Otras inecuaciones con una incógnita**

### **5.1 Inecuaciones racionales**
De la forma:
$$
\frac{P(x)}{Q(x)} > 0
$$

**Ejemplo:**
$$
\frac{x-1}{x+2} \leq 0
$$

1. Numerador: $x=1$  
2. Denominador: $x=-2$ (excluido)  
3. Intervalos: $(-\infty,-2), (-2,1), (1,\infty)$  
4. Signos:  
   - $x=-3$: $( - )/( - )=+$ ✘  
   - $x=0$: $( - )/( + )=-$ ✔  
   - $x=2$: $(+)/(+)=+$ ✘  

**Solución:** $(-2,1]$

---

### **5.2 Inecuaciones con valor absoluto**
$$
|x| < a \iff -a < x < a
$$
$$
|x| > a \iff x < -a \ \text{o}\ x > a
$$

**Ejemplo:**  
$$
|x-3| \leq 5 \implies -5 \leq x-3 \leq 5 \implies -2 \leq x \leq 8
$$

---

### **5.3 Inecuaciones irracionales**
Contienen raíces cuadradas.

**Ejemplo:**  
$$
\sqrt{x-1} \leq 3
$$

1. Dominio: $x-1 \geq 0 \implies x \geq 1$  
2. Resolver: $x-1 \leq 9 \implies x \leq 10$  
3. Solución: $1 \leq x \leq 10$

---

## **6. Representación gráfica**
- Intervalo abierto: $(a,b)$  
- Intervalo cerrado: $[a,b]$  
- Semi-abierto: $(a,b]$ o $[a,b)$  

**Convenciones:**  
- Punto **relleno** → valor incluido ($\leq$, $\geq$)  
- Punto **hueco** → valor excluido ($<$, $>$)  

