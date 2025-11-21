# Valuacion_Bonos
Valuación de Bonos

#  Análisis Cuantitativo de Bonos: Precio, Duración, Convexidad y Curvas de Rendimiento




---

##  Estructura del Proyecto

###  1 — Precio y Duración de Bonos**
**Conceptos cubiertos:**
- Precio de un bono con cupones.
- Duración de Macaulay y Duración Modificada.
- Efecto del YTM sobre el precio (Price–Yield Curve).
- Aproximación del precio con duración.
- Ejercicios prácticos y gráficas.

**Funciones implementadas:**
- `bond_price()`
- `macaulay_duration()`
- `modified_duration()`
- `price_using_duration_approx()`

---

### 2 — Convexidad e Inmunización**
**Conceptos cubiertos:**
- Convexidad y aproximación cuadrática del precio.
- Comparación:
  - Precio directo
  - Aproximación por duración
  - Aproximación por duración + convexidad
- Construcción de un portafolio inmunizado:
  - Igualación de valor presente
  - Igualación de duración
- Resolución con álgebra lineal (`numpy.linalg.solve`).

**Funciones implementadas:**
- `convexity()`
- `price_duration_only()`
- `price_duration_convexity()`
- `immunize_two_bonds()`

Gráficas incluidas:
- Curvas de error entre aproximaciones
- Portafolio inmunizado vs pasivo objetivo

---

### 3 — Curvas de Rendimiento y Bootstrapping**
**Conceptos cubiertos:**
- Tasas spot (zero–coupon).
- Factores de descuento `DF(T)`.
- Tasas forward implícitas.
- Reconstrucción de curva spot con **bootstrapping**.
- Ajuste paramétrico usando **Nelson–Siegel**:
  - Cálculo de β₀, β₁, β₂, λ
  - Curva ajustada vs curva bootstrapped.
- Visualización de la curva y forwards.

**Funciones implementadas:**
- `bond_price_from_spot_curve()`
- `bootstrap_spot_from_bond_prices()`
- `nelson_siegel()`
- `forward_rate_1y()`

Gráficas incluidas:
- Curva spot verdadera vs curva bootstrapped
- Curva Nelson–Siegel ajustada
- Factores de descuento
- Forward 1-year curve

---



