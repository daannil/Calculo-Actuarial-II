# Calculo-Actuarial-II
López Lazcano Renata Daniela
## Resumen: Cálculo Actuarial II - Unidad I
*Preliminares probabilísticos y entorno computacional reproducible*

---

### 1. Problema actuarial
* **Incertidumbre**
* **Tiempo**
* **Dinero**
* **Obligación actuarial**
  * Evento incierto
  * Monto del pago
  * Momento del pago
* **Valor actuarial**
  * E[valor presente aleatorio]

### 2. Entorno computacional
* GitHub
* Git
* Python
* Visual Studio Code
* Entorno virtual `.venv`
* `requirements.txt`
* `README.md`
* **Repositorio reproducible**
  * `data/` (`raw/`, `processed/`)
  * `notebooks/`
  * `src/`
  * `tests/`
  * `figures/`
  * `reports/`
  * `.github/workflows/`

### 3. Python básico
* Variables y tipos numéricos
* Funciones
* NumPy, Pandas, Matplotlib, SciPy
* Semillas para reproducibilidad

### 4. Lenguaje de probabilidad
* Experimento, Espacio muestral (Ω), Resultado, Evento, σ-álgebra
* **Espacio de probabilidad:** (Ω, F, P)
* **Operaciones con eventos:** A ∪ B, A ∩ B, Aᶜ, A \ B
* **Probabilidad condicional:** P(A|B) = P(A ∩ B) / P(B)
* **Ley de probabilidad total:** P(A) = Σ P(A|Bⱼ)P(Bⱼ)
* **Teorema de Bayes:** Actualiza probabilidades con nueva información
* **Independencia:** P(A ∩ B) = P(A)P(B)

### 5. Variables aleatorias
* **Definición:** X: Ω → ℝ
* **Discretas:** p_X(x) = P(X=x)
* **Continuas:** f_X(x)
* **Función de distribución:** F_X(x) = P(X ≤ x)
* **Indicadores:** 1 si ocurre A, 0 si no ocurre A

### 6. Esperanza, varianza y dependencia
* **Esperanza:** E[X] (Promedio esperado del modelo)
* **Linealidad:** E[Σ Xⱼ] = Σ E[Xⱼ]
* **Varianza:** Var(X) = E[X²] - (E[X])²
* **Desviación estándar:** σ_X = √(Var(X))
* **Covarianza:** Cov(X,Y) = E[XY] - E[X]E[Y]
* **Esperanza condicional:** E[X] = E[E[X|Y]]

### 7. Cuantiles y pérdidas
* **Cuantil:** Describe una posición de la distribución
* **Deducible:** Y = (X - d)⁺
* **Límite:** Y = min(X, u)

### 8. Distribuciones discretas
* **Bernoulli:** 0 (no ocurre), 1 (ocurre), E[X]=p, Var(X)=p(1-p)
* **Binomial:** Número de éxitos en n ensayos (E[N]=np)
* **Poisson:** Conteo de eventos (E[N]=λ, revisar equidispersión)
* **Geométrica:** Ensayos hasta el primer éxito (E[N]=1/p, falta de memoria)

### 9. Distribuciones continuas
* Uniforme
* Exponencial (modelo de tiempos de espera)
* Gamma
* Normal (simétrica; útil para aproximaciones)

### 10. Riesgo agregado
* **Suma de pérdidas:** S = X₁ + ... + Xₙ
* **Modelo colectivo:** S = Σ Xⱼ (N: frecuencia, Xⱼ: severidad)
* **Si N ~ Poisson(λ):** E[S] = λμ, Var(S) = λ(σ² + μ²)

### 11. Ley de los grandes números
* Al aumentar n, la media muestral tiende a μ
* Simulación y frecuencia observada
* **Importante:** Una cartera grande **NO** elimina el riesgo sistemático

### 12. Datos reales de México
* **INEGI:** Estadísticas de Defunciones Registradas (EDR)
* Diferenciar: Conteo, Tasa bruta, Probabilidad individual (Tasa bruta ≠ q_x)
* **Microdatos:** Revisar primero el diccionario de datos
* **Flujo correcto:** Descargar → Guardar originales → Inspeccionar → Recodificar con código → Crear procesados → Comparar con cifras oficiales

### 13. Ejemplos de probabilidad actuarial
* Al menos una reclamación, exactamente k eventos
* Probabilidad de excedencia y tiempo de espera
* Deducible con exponencial y costo agregado Compound Poisson

### 14. Errores que deben evitarse
* Densidad ≠ probabilidad puntual
* Tasa agregada ≠ probabilidad individual
* No asumir independencia sin justificarla ni elegir Poisson solo por ser conteo
* Esperanza ≠ resultado que necesariamente ocurrirá
* No redondear pronto, no modificar datos crudos, no subir datos sensibles
* **Python calcula; la explicación debe ser matemática y actuarial**

### 15. Práctica de la Unidad I
* **Parte A:** Repositorio (GitHub, Git, Python, VS Code, GitHub Actions)
* **Parte B:** Notebook (Bernoulli, Binomial, Poisson, Exponencial, LLN)
* **Parte C:** Datos mexicanos (EDR 2015–2024)
* **Parte D:** Entrega reproducible

### 16. Ejercicios propuestos
* Probabilidad, variables aleatorias, distribuciones, pérdidas, riesgo agregado y datos reales.

### 17. Al terminar la unidad
* Comprender probabilidad actuarial, manejar variables aleatorias, calcular momentos, identificar distribuciones, modelar pérdidas, usar Python y Git/GitHub para análisis reproducibles.


