---
title: "Series de Fourier-Bessel"
tags: [concept, fourier-bessel, circular-membranes, orthogonality]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Series de Fourier-Bessel

## 📌 Idea Central

La serie de Fourier-Bessel es el análogo en simetría radial de las series de Fourier trigonométricas. Permite expandir cualquier función definida en un disco o sector circular $r \in [0, a]$ en una base ortogonal ponderada formada por funciones de Bessel $\{J_\nu(\alpha_{\nu, m} r / a)\}$.

## 🧮 Ecuaciones Clave

Para una función $f(r) \in L^2_r([0, a])$ con $f(a) = 0$:
$$ f(r) = \sum_{m=1}^\infty c_m J_\nu\left( \frac{\alpha_{\nu, m} r}{a} \right) $$
donde $\alpha_{\nu, m}$ es el $m$-ésimo cero positivo de $J_\nu(x)$.

### Relación de Ortogonalidad con Peso $w(r) = r$:
$$ \int_0^a r J_\nu\left( \frac{\alpha_{\nu, m} r}{a} \right) J_\nu\left( \frac{\alpha_{\nu, k} r}{a} \right) dr = \frac{a^2}{2} \left[ J_{\nu+1}(\alpha_{\nu, m}) \right]^2 \delta_{mk} $$

### Coeficientes de Fourier-Bessel:
$$ c_m = \frac{2}{a^2 \left[ J_{\nu+1}(\alpha_{\nu, m}) \right]^2} \int_0^a r f(r) J_\nu\left( \frac{\alpha_{\nu, m} r}{a} \right) dr $$

Para membranas sectoriales de ángulo $\alpha_0$, el orden $\nu$ toma valores fraccionarios $\nu = \frac{n\pi}{\alpha_0}$, reflejando la singularidad geométrica en las esquinas del dominio.

## 🔗 Conceptos Relacionados

- **Base teórica**: [[Concepts/Bloque_01/Problema_Sturm_Liouville|Teoría de Sturm-Liouville]], [[Concepts/Bloque_01/Funciones_Bessel|Funciones de Bessel]]
- **Simulación computacional**: `Notebooks/Python/01_Fourier_Bessel_Series.ipynb`
