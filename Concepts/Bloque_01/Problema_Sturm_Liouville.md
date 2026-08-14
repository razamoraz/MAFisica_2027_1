---
title: "Problema General de Sturm-Liouville"
tags: [concept, sturm-liouville, self-adjoint, eigenvalues]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Problema General de Sturm-Liouville

## 📌 Idea Central

La teoría de Sturm-Liouville es el pilar central del análisis espectral de ecuaciones diferenciales ordinarias lineales de segundo orden autoadjuntas. Garantiza que los valores propios $\lambda_n$ son reales, forman una sucesión monótona creciente no acotada, y sus funciones propias $\{y_n(x)\}$ forman una base ortogonal completa en el espacio de Hilbert ponderado $L^2_w([a,b])$.

## 🧮 Ecuaciones Clave

La forma autoadjunta de Sturm-Liouville para el operador diferencial $\mathcal{L}$ es:
$$ \mathcal{L} y = \frac{d}{dx}\left[ p(x) \frac{dy}{dx} \right] + q(x) y = -\lambda w(x) y $$
donde $p(x) > 0, w(x) > 0$ en el intervalo $[a,b]$.

Condiciones de frontera generales regulares de tipo Robin:
$$ \alpha_1 y(a) + \alpha_2 y'(a) = 0, \quad \beta_1 y(b) + \beta_2 y'(b) = 0 $$

### Teoremas Fundamentales:
1. **Realidad**: Todos los valores propios $\lambda_n \in \mathbb{R}$.
2. **Ortogonalidad con peso $w(x)$**:
   $$ \langle y_n, y_m \rangle_w = \int_a^b y_n(x) y_m(x) w(x) dx = N_n \delta_{nm} $$
3. **Completitud y Relación de Cierre**:
   $$ \sum_{n=1}^\infty \frac{y_n(x) y_n(x')}{N_n} = \frac{\delta(x - x')}{w(x)} $$

## 🔗 Conceptos Relacionados

- **Ejemplos**:
  - $p=1, q=0, w=1 \implies$ [[Concepts/Bloque_01/Series_Fourier|Series de Fourier]]
  - $p(x)=x, q(x)=-\nu^2/x, w(x)=x \implies$ [[Concepts/Bloque_01/Funciones_Bessel|Ecuación de Bessel]]
  - $p(x)=1-x^2, q(x)=0, w(x)=1 \implies$ [[Concepts/Bloque_04/Polinomios_Legendre|Ecuación de Legendre]]
- **Inversión**: [[Concepts/Bloque_01/Funcion_Green_1D|Funciones de Green 1D]]
