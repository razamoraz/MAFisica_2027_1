---
title: "Funciones de Bessel"
tags: [concept, bessel-functions, cylindrical-harmonics, special-functions]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Funciones de Bessel

## 📌 Idea Central

Las funciones de Bessel (o funciones cilíndricas) surgen al resolver la ecuación de Helmholtz $\nabla^2 \psi + k^2 \psi = 0$ mediante separación de variables en coordenadas cilíndricas $(r, \theta, z)$ o polares $(r, \theta)$. Describen modos normales de vibración en membranas circulares, propagación en guías de ondas cilíndricas y difracción óptica y acústica.

## 🧮 Ecuaciones Clave

Ecuación diferencial de Bessel de orden $\nu$:
$$ x^2 \frac{d^2 y}{dx^2} + x \frac{dy}{dx} + (x^2 - \nu^2)y = 0 $$

Solución general:
$$ y(x) = C_1 J_\nu(x) + C_2 Y_\nu(x) $$

- **$J_\nu(x)$ (Primera especie)**: Solución regular en el origen ($x \to 0$):
  $$ J_\nu(x) = \sum_{m=0}^\infty \frac{(-1)^m}{m!\,\Gamma(m+\nu+1)} \left(\frac{x}{2}\right)^{2m+\nu} $$
- **$Y_\nu(x)$ (Segunda especie o Neumann)**: Solución singular en el origen ($Y_\nu(x) \to -\infty$ cuando $x \to 0$).

### Relaciones de Recurrencia:
$$ J_{\nu-1}(x) + J_{\nu+1}(x) = \frac{2\nu}{x} J_\nu(x) $$
$$ J_{\nu-1}(x) - J_{\nu+1}(x) = 2 J'_\nu(x) $$
$$ \frac{d}{dx}\left[ x^\nu J_\nu(x) \right] = x^\nu J_{\nu-1}(x) $$

### Ceros y Propiedades Nodales:
Si $\alpha_{\nu, m}$ denota el $m$-ésimo cero positivo de $J_\nu(x)$ ($J_\nu(\alpha_{\nu,m}) = 0$), los ceros están entrelazados:
$$ 0 < \alpha_{\nu, 1} < \alpha_{\nu+1, 1} < \alpha_{\nu, 2} < \alpha_{\nu+1, 2} < \dots $$

## 🔗 Conceptos Relacionados

- **Desarrollo en serie**: [[Concepts/Bloque_01/Series_Fourier_Bessel|Series de Fourier-Bessel]]
- **Asintótica y complejo**: [[Concepts/Bloque_02/Asintotica_Bessel_Integrales_Complejas|Representación Asintótica de Bessel]]
- **Bessel Modificadas**: [[Concepts/Bloque_02/Difraccion_Cilindro_Bessel_Modificadas|Funciones $I_\nu$ y $K_\nu$ en Difracción]]
