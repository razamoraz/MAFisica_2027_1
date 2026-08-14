---
title: "Potenciales Reflexión Cero y Solitones (KdV)"
tags: [concept, solitons, reflectionless-potentials, kdv-equation, nonlinear-waves]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Potenciales Reflexión Cero y Solitones (KdV)

## 📌 Idea Central

Los potenciales de reflexión cero (como los potenciales de Pöschl-Teller $V(x) = -N(N+1)\operatorname{sech}^2(x)$) son aquellos en los que el coeficiente de reflexión $R(k) = 0$ para todas las energías del espectro continuo. En la física no lineal, estos potenciales corresponden exactamente a las soluciones de **ondas solitarias (solitones)** de la ecuación de Korteweg-de Vries (KdV) a través del método de la transformada de dispersión inversa (IST).

## 🧮 Ecuaciones Clave

### Potencial de Pöschl-Teller 1D:
$$ V(x) = -\frac{\hbar^2 \kappa^2}{m} N(N+1)\operatorname{sech}^2(\kappa x) $$
- Admite exactamente $N$ estados ligados.
- Para cualquier onda incidente $k > 0$, el coeficiente de reflexión es idénticamente nulo:
  $$ R(k) = 0, \quad |T(k)| = 1 $$

### Conexión con la Ecuación Korteweg-de Vries (KdV):
$$ \frac{\partial u}{\partial t} - 6 u \frac{\partial u}{\partial x} + \frac{\partial^3 u}{\partial x^3} = 0 $$

Solución de 1-solitón propagándose a velocidad $v = 4\kappa^2$:
$$ u(x,t) = -2\kappa^2 \operatorname{sech}^2\left[ \kappa(x - 4\kappa^2 t - x_0) \right] $$

El valor propio del estado ligado cuántico $\lambda = -\kappa^2$ permanece invariante en el tiempo (integral de movimiento de Lax).

## 🔗 Conceptos Relacionados

- **Teoría Espectral**: [[Concepts/Bloque_03/Pozo_Potencial_Estados_Ligados_Libres|Pozos de Potencial]]
- **Acoplamiento clásico**: [[Concepts/Bloque_03/Ondas_Elasticas_Acopladas|Ondas Elásticas Acopladas]]
