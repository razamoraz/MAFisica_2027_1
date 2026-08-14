---
title: "Difracción Cilíndrica y Funciones de Bessel Modificadas"
tags: [concept, modified-bessel, diffraction, electromagnetic-scattering]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Difracción Cilíndrica y Funciones de Bessel Modificadas

## 📌 Idea Central

La dispersión de una onda plana incidente sobre un obstáculo cilíndrico infinito de radio $a$ se resuelve descomponiendo la onda incidente en armónicos cilíndricos y aplicando condiciones de frontera en la superficie. En regiones con difusión o decaimiento evanescente, surgen las **funciones de Bessel modificadas** $I_\nu(x)$ y $K_\nu(x)$.

## 🧮 Ecuaciones Clave

### Expansión de Jacobi-Anger (Onda Plana en Armónicos Cilíndricos):
$$ e^{ikx} = e^{ikr\cos\theta} = \sum_{m=-\infty}^{\infty} i^m J_m(kr) e^{im\theta} = J_0(kr) + 2\sum_{m=1}^\infty i^m J_m(kr)\cos(m\theta) $$

### Campo Total Dispersado por un Cilindro Conductor Perfecto:
$$ \psi_{\text{tot}}(r,\theta) = \psi_{\text{inc}} + \psi_{\text{scat}} = \sum_{m=-\infty}^\infty i^m \left[ J_m(kr) - \frac{J_m(ka)}{H_m^{(1)}(ka)} H_m^{(1)}(kr) \right] e^{im\theta} $$

### Funciones de Bessel Modificadas:
Para el argumento imaginario $z = ix$:
$$ I_\nu(x) = i^{-\nu} J_\nu(ix) \quad (\text{crecimiento exponencial } \sim \frac{e^x}{\sqrt{2\pi x}}) $$
$$ K_\nu(x) = \frac{\pi}{2} i^{\nu+1} H_\nu^{(1)}(ix) \quad (\text{decaimiento exponencial } \sim \sqrt{\frac{\pi}{2x}} e^{-x}) $$

## 🔗 Conceptos Relacionados

- **Límite de longitud de onda larga**: [[Concepts/Bloque_02/Difraccion_Rayleigh_Seccion_Eficaz|Dispersión de Rayleigh]]
- **Condición de contorno**: [[Concepts/Bloque_01/Funciones_Bessel|Funciones de Bessel]]
