# Estadística

---

## 1. Introducción a la estadística

La **estadística** es la ciencia que estudia cómo **recoger, organizar, analizar e interpretar datos** para extraer conclusiones y tomar decisiones en situaciones de incertidumbre.

**Objetivos principales:**
1. Describir los datos (**estadística descriptiva**).  
2. Hacer inferencias o predicciones (**estadística inferencial**).

---

## 2. Estudios estadísticos y muestras

### 2.1 Población y muestra
- **Población:** conjunto completo de individuos, objetos o datos de interés.  
- **Muestra:** subconjunto representativo de la población, utilizado cuando no es posible estudiar toda la población.  

**Tipos de muestreo:**
- Aleatorio simple  
- Estratificado  
- Sistemático  
- Por conveniencia (menos recomendable)

### 2.2 Variables estadísticas
- **Cualitativa:** describe categorías (ej. sexo, color).  
- **Cuantitativa:** mide cantidades numéricas.
  - Discreta: valores enteros (ej. número de hijos)  
  - Continua: valores reales dentro de un intervalo (ej. altura, peso)

---

## 3. Tablas y gráficos estadísticos

### 3.1 Tablas de frecuencia
Organizan los datos según valores o intervalos:

| Valor / Clase | Frecuencia absoluta $f_i$ | Frecuencia relativa $h_i = f_i/n$ | Frecuencia acumulada $F_i$ | Frecuencia relativa acumulada $H_i$ |
|---------------|---------------------------|----------------------------------|----------------------------|------------------------------------|

### 3.2 Gráficos
- Barras → variables discretas o cualitativas  
- Histogramas → variables continuas  
- Polígono de frecuencias → conecta los puntos medios del histograma  
- Ojiva → frecuencias acumuladas  
- Pastel → proporción de categorías

---

## 4. Parámetros de posición

**4.1 Media aritmética:**  
$$
\bar{x} = \frac{\sum_{i=1}^{n} x_i}{n}
$$

**4.2 Mediana:**  
- Si $n$ impar: $$M = x_{\frac{n+1}{2}}$$  
- Si $n$ par: $$M = \frac{x_{\frac{n}{2}} + x_{\frac{n}{2}+1}}{2}$$

**4.3 Moda:** valor que más se repite (unimodal, bimodal, multimodal).

**4.4 Cuantiles:**  
- Cuartiles: $Q_1,Q_2,Q_3$  
- Deciles: $D_i$  
- Percentiles: $P_i$

---

## 5. Parámetros de dispersión

**5.1 Rango:**  
$$
R = x_{\max} - x_{\min}
$$

**5.2 Varianza:**  
- Población:  
$$
\sigma^2 = \frac{\sum_{i=1}^{N} (x_i-\mu)^2}{N}
$$  
- Muestra:  
$$
s^2 = \frac{\sum_{i=1}^{n} (x_i-\bar{x})^2}{n-1}
$$

**5.3 Desviación estándar:**  
$$
\sigma = \sqrt{\sigma^2} \quad , \quad s = \sqrt{s^2}
$$

**5.4 Coeficiente de variación:**  
$$
CV = \frac{\sigma}{\mu} \cdot 100\%
$$

---

## 6. Distribuciones bidimensionales

Cuando se estudian **dos variables**:

- Tabla de contingencia → filas = variable X, columnas = variable Y  
- Se calculan **frecuencias conjuntas** y **marginales**.

### 6.1 Diagrama de dispersión
Representa los pares $(x_i, y_i)$ → permite visualizar la relación entre variables.

---

## 7. Correlación lineal

Mide la **intensidad y dirección** de la relación lineal:

$$
r = \frac{\sum_{i=1}^{n} (x_i-\bar{x})(y_i-\bar{y})}{\sqrt{\sum_{i=1}^{n} (x_i-\bar{x})^2 \sum_{i=1}^{n} (y_i-\bar{y})^2}}
$$

- $r \approx 1$ → correlación positiva fuerte  
- $r \approx -1$ → correlación negativa fuerte  
- $r \approx 0$ → no hay correlación lineal

---

## 8. Recta de regresión

Describe la **relación lineal aproximada** para predecir valores de $Y$ a partir de $X$:

- Ecuación:  
$$
y = a + bx
$$

- Pendiente:  
$$
b = \frac{\sum (x_i-\bar{x})(y_i-\bar{y})}{\sum (x_i-\bar{x})^2}
$$

- Intersección:  
$$
a = \bar{y} - b\bar{x}
$$

**Interpretación:**  
- $b$ → cambio esperado en $y$ por unidad de $x$  
- $a$ → valor de $y$ cuando $x=0$

---

## 9. Pasos en un estudio estadístico

1. Recoger datos → definir población/muestra  
2. Organizar datos → tablas y frecuencias  
3. Representar → gráficos  
4. Calcular parámetros de posición → media, mediana, moda  
5. Calcular parámetros de dispersión → rango, varianza, desviación estándar  
6. Analizar relación entre variables → diagrama de dispersión, correlación  
7. Ajustar modelo lineal → recta de regresión  
8. Interpretar resultados y conclusiones

---

## 10. Ejemplos prácticos

**Ejemplo 1 — Media y desviación:**  
Datos: $[2,4,4,4,5,5,7,9]$  
$$
\bar{x} = \frac{2+4+4+4+5+5+7+9}{8} = 5
$$  
$$
s^2 = \frac{(2-5)^2 + (4-5)^2*3 + ...}{7} = 4 \quad , \quad s = 2
$$

**Ejemplo 2 — Correlación:**  
Pares: $(1,2),(2,3),(3,5),(4,4)$  
$$
r \approx 0.84
$$ → correlación positiva fuerte

**Ejemplo 3 — Regresión:**  
Recta: $y=1.75 + 0.7x$ → predecir $y$ para $x=5$:  
$$
y = 1.75 + 0.7*5 = 5.5
$$

