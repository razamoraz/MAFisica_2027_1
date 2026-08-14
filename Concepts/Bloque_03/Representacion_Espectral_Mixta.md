---
title: "Representación Espectral Mixta"
tags: [concept, spectral-theory, completeness, bound-states, continuous-spectrum]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Representación Espectral Mixta

## 📌 Idea Central

La resolución de la identidad (relación de completitud) para operadores diferenciales lineales en dominios infinitos con potenciales localizados no se agota con una serie discreta ni con una sola integral de Fourier, sino que requiere la suma simultánea sobre los estados ligados discretos más la integración sobre todos los modos del espectro continuo.

## 🧮 Ecuaciones Clave

Para un operador con $N_b$ estados ligados $\{\psi_n(x)\}$ y un conjunto completo de funciones de dispersión $\{\psi_k(x)\}$:

### Relación de Completitud / Cierre:
$$ \sum_{n=1}^{N_b} \psi_n(x) \psi_n^*(x') + \int_{-\infty}^{\infty} \psi_k(x) \psi_k^*(x') \frac{dk}{2\pi} = \delta(x - x') $$

### Expansión de Cualquier Estado Arbitrario $f(x) \in L^2(\mathbb{R})$:
$$ f(x) = \sum_{n=1}^{N_b} c_n \psi_n(x) + \int_{-\infty}^{\infty} c(k) \psi_k(x) \frac{dk}{2\pi} $$
donde:
$$ c_n = \int_{-\infty}^{\infty} \psi_n^*(x) f(x) dx, \quad c(k) = \int_{-\infty}^{\infty} \psi_k^*(x) f(x) dx $$

### Conservación de la Norma (Teorema de Parseval Generalizado):
$$ \int_{-\infty}^{\infty} |f(x)|^2 dx = \sum_{n=1}^{N_b} |c_n|^2 + \int_{-\infty}^{\infty} |c(k)|^2 \frac{dk}{2\pi} $$

## 🔗 Conceptos Relacionados

- **Fundamento**: [[Concepts/Bloque_03/Pozo_Potencial_Estados_Ligados_Libres|Estados Ligados y Libres]]
- **Green y Resolvente**: [[Concepts/Bloque_03/Resonancias_Polos_Resolvente|Polos del Resolvente]]
