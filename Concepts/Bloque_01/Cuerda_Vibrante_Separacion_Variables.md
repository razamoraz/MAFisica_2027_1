---
title: "Ecuación de la Cuerda Vibrante y Separación de Variables"
tags: [concept, pde, wave-equation, separation-of-variables]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Ecuación de la Cuerda Vibrante y Separación de Variables

## 📌 Idea Central

La ecuación de onda unidimensional modela la propagación de perturbaciones transversales en una cuerda tensa con densidad lineal $\rho$ y tensión $T_0$. Mediante la técnica de **separación de variables**, la ecuación en derivadas parciales (EDP) se desacopla en un conjunto de ecuaciones diferenciales ordinarias (EDOs) cuyos valores propios determinan las frecuencias armónicas naturales del sistema.

## 🧮 Ecuaciones Clave

La ecuación diferencial para el desplazamiento transversal $u(x,t)$ en $x \in [0, L]$ es:
$$ \frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}, \quad c = \sqrt{\frac{T_0}{\rho}} $$

Con condiciones de frontera de Dirichlet homogéneas (extremos fijos):
$$ u(0, t) = 0, \quad u(L, t) = 0 $$

Proponiendo una solución separable $u(x,t) = X(x)T(t)$:
$$ \frac{X''(x)}{X(x)} = \frac{T''(t)}{c^2 T(t)} = -\lambda^2 $$

Lo que conduce al problema de valores propios espacial:
$$ X''(x) + \lambda^2 X(x) = 0 \implies X_n(x) = \sin\left(\frac{n\pi x}{L}\right), \quad \lambda_n = \frac{n\pi}{L}, \quad n = 1, 2, \dots $$

La solución general como superposición lineal es:
$$ u(x,t) = \sum_{n=1}^\infty \sin\left(\frac{n\pi x}{L}\right) \left[ A_n \cos(\omega_n t) + B_n \sin(\omega_n t) \right], \quad \omega_n = \frac{n\pi c}{L} $$

## 🔗 Conceptos Relacionados

- **Fundamento de**: [[Concepts/Bloque_01/Series_Fourier|Series de Fourier]], [[Concepts/Bloque_01/Problema_Sturm_Liouville|Problema de Sturm-Liouville]]
- **Generalización en 2D**: [[Concepts/Bloque_01/Funciones_Bessel|Membranas circulares y Funciones de Bessel]]
- **Límite continuo**: [[Concepts/Bloque_02/Cuerda_Semiinfinita_Espectro_Continuo|Cuerda semiinfinita y espectro continuo]]
