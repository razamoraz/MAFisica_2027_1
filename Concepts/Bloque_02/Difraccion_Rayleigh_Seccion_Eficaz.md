---
title: "Difracción de Rayleigh y Sección Eficaz de Dispersión"
tags: [concept, rayleigh-scattering, cross-section, optics, waves]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Difracción de Rayleigh y Sección Eficaz de Dispersión

## 📌 Idea Central

La dispersión de Rayleigh describe la difracción de ondas electromagnéticas o acústicas por obstáculos o partículas dieléctricas de dimensiones mucho menores que la longitud de onda incidente ($ka = 2\pi a / \lambda \ll 1$). La potencia total dispersada es inversamente proporcional a la cuarta potencia de la longitud de onda ($\sigma \propto \lambda^{-4}$), explicando fundamentalmente el color azul del cielo terrestre.

## 🧮 Ecuaciones Clave

### Sección Eficaz Diferencial ($\frac{d\sigma}{d\Omega}$):
Para una onda no polarizada sobre una partícula polarizable de radio $a$:
$$ \frac{d\sigma}{d\Omega} = a^2 (ka)^4 \left( \frac{n^2 - 1}{n^2 + 2} \right)^2 \frac{1 + \cos^2\theta}{2} $$
donde $n$ es el índice de refracción relativo.

### Sección Eficaz Total ($\sigma_{\text{tot}}$):
Integrando sobre toda la esfera sólida $d\Omega = \sin\theta d\theta d\phi$:
$$ \sigma_{\text{tot}} = \frac{8\pi}{3} k^4 a^6 \left( \frac{n^2 - 1}{n^2 + 2} \right)^2 = \frac{128 \pi^5 a^6}{3 \lambda^4} \left( \frac{n^2 - 1}{n^2 + 2} \right)^2 $$

La dependencia $\sigma \propto \omega^4 \propto \lambda^{-4}$ hace que la luz azul ($\lambda \approx 450\,\text{nm}$) se disperse aproximadamente 9.4 veces más intensamente que la luz roja ($\lambda \approx 700\,\text{nm}$).

## 🔗 Conceptos Relacionados

- **Tratamiento general de ondas**: [[Concepts/Bloque_02/Difraccion_Cilindro_Bessel_Modificadas|Difracción Cilíndrica]]
- **Taller computacional**: `Notebooks/Python/02_Rayleigh_Scattering_Simulation.ipynb`
