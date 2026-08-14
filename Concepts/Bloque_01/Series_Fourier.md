---
title: "Series de Fourier y Ortogonalidad"
tags: [concept, fourier-series, orthogonality, functional-analysis]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Series de Fourier y Ortogonalidad

## 📌 Idea Central

Una serie de Fourier descompone cualquier función periódica continua a trozos $f(x) \in L^2([-L, L])$ en una suma infinita de funciones trigonométricas armónicas ortogonales. Constituye el prototipo fundamental de desarrollo espectral para operadores diferenciales con espectro discreto.

## 🧮 Ecuaciones Clave

Para una función con periodo $2L$:
$$ f(x) \sim \frac{a_0}{2} + \sum_{n=1}^\infty \left[ a_n \cos\left(\frac{n\pi x}{L}\right) + b_n \sin\left(\frac{n\pi x}{L}\right) \right] $$

Los coeficientes de Fourier se determinan mediante el producto interno y la relación de ortogonalidad:
$$ \int_{-L}^{L} \cos\left(\frac{n\pi x}{L}\right) \cos\left(\frac{m\pi x}{L}\right) dx = L \delta_{nm} $$
$$ a_n = \frac{1}{L} \int_{-L}^{L} f(x) \cos\left(\frac{n\pi x}{L}\right) dx, \quad b_n = \frac{1}{L} \int_{-L}^{L} f(x) \sin\left(\frac{n\pi x}{L}\right) dx $$

Forma compleja exponencial:
$$ f(x) = \sum_{n=-\infty}^{\infty} c_n e^{i \frac{n\pi x}{L}}, \quad c_n = \frac{1}{2L} \int_{-L}^{L} f(x) e^{-i \frac{n\pi x}{L}} dx $$

Identidad de Parseval (conservación de energía en el espacio de Hilbert):
$$ \frac{1}{2L} \int_{-L}^{L} |f(x)|^2 dx = \sum_{n=-\infty}^{\infty} |c_n|^2 $$

## 🔗 Conceptos Relacionados

- **Marco General**: [[Concepts/Bloque_01/Problema_Sturm_Liouville|Problema de Sturm-Liouville]]
- **Análogo Cilíndrico**: [[Concepts/Bloque_01/Series_Fourier_Bessel|Series de Fourier-Bessel]]
- **Límite Continuo ($L \to \infty$)**: [[Concepts/Bloque_02/Transformada_Fourier_Continuo|Transformada de Fourier]]
