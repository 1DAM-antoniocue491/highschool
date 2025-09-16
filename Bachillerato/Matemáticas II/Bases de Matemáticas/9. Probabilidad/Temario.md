# 🎲 Tema: Probabilidad — Desarrollo completo

---

## 1. Experimentos aleatorios y sucesos

### 1.1 Experimento aleatorio
Un **experimento aleatorio** es un proceso que produce un resultado incierto, aunque sus posibles resultados sean conocidos.  

**Ejemplos:**  
- Lanzar un dado  
- Tirar una moneda  
- Sacar una carta de una baraja  

### 1.2 Espacio muestral
El **espacio muestral** $S$ es el conjunto de todos los resultados posibles del experimento.  

**Ejemplos:**  
- Lanzar una moneda: $$S = \{\text{cara}, \text{cruz}\}$$  
- Lanzar un dado: $$S = \{1,2,3,4,5,6\}$$  
- Sacar una carta: $$S = \{A♠, 2♠, ..., K♣\}$$

### 1.3 Sucesos o eventos
Un **suceso** es un subconjunto de $S$.  
- **Simple:** contiene un solo resultado (ej. "sacar un 3").  
- **Compuesto:** contiene varios resultados (ej. "sacar un número par").  

Se denotan con letras mayúsculas: $$A, B, C$$.

---

## 2. Operaciones con sucesos

- **Unión:** $$A \cup B = \text{"ocurre A o B o ambos"}$$  
- **Intersección:** $$A \cap B = \text{"ocurre A y B"}$$  
- **Complemento:** $$\bar{A} = \text{"A no ocurre"}$$  
- **Diferencia:** $$A - B = A \cap \bar{B}$$

---

## 3. Probabilidad de un suceso

Si todos los resultados son **equiprobables**, la probabilidad de un suceso $A$ es:  
$$
P(A) = \frac{n(A)}{n(S)}
$$

**Propiedades:**  
1. $$0 \le P(A) \le 1$$  
2. $$P(S) = 1$$  
3. $$P(\bar{A}) = 1 - P(A)$$  
4. $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

**Ejemplo:** lanzar un dado, suceso $$A = \{\text{número par}\}$$  
$$
P(A) = \frac{3}{6} = 0.5
$$

---

## 4. Probabilidades de sucesos combinados

- **Mutuamente excluyentes:** no pueden ocurrir a la vez.  
$$
A \cap B = \emptyset \quad \Rightarrow \quad P(A \cup B) = P(A) + P(B)
$$

- **Independientes:** ocurrencia de uno no afecta al otro.  
$$
P(A \cap B) = P(A) \cdot P(B)
$$

- **Dependientes:** ocurrencia de uno afecta al otro.  
$$
P(A \cap B) = P(A) \cdot P(B|A)
$$

---

## 5. Probabilidad condicionada

Probabilidad de que ocurra $A$ dado que $B$ ya ocurrió:  
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}, \quad P(B) \neq 0
$$

**Ejemplo:** lanzar un dado  
- $$A = \{2,4,6\}$$  
- $$B = \{4,5,6\}$$  
$$
P(A|B) = \frac{P(A \cap B)}{P(B)} = \frac{2/6}{3/6} = \frac{2}{3}
$$

---

## 6. Teorema de la probabilidad total

Si $B_1, ..., B_n$ son sucesos **mutuamente excluyentes** y **exhaustivos**, entonces para cualquier suceso $A$:  
$$
P(A) = \sum_{i=1}^{n} P(A|B_i) \cdot P(B_i)
$$

**Ejemplo:** urna con dos compartimentos  
- $B_1$ = sacar del primer compartimento  
- $B_2$ = sacar del segundo  
- $A$ = sacar bola roja  
$$
P(A) = P(A|B_1)P(B_1) + P(A|B_2)P(B_2)
$$

---

## 7. Probabilidad y combinatoria

- **Combinaciones:** elegir $k$ elementos de $n$ sin importar el orden:  
$$
C_n^k = \binom{n}{k} = \frac{n!}{k!(n-k)!}
$$

- **Permutaciones:** ordenar $n$ elementos:  
$$
P_n = n!
$$

**Ejemplo:** lanzar 3 monedas, probabilidad de obtener exactamente 2 caras:  
$$
C_3^2 / 2^3 = 3/8
$$

