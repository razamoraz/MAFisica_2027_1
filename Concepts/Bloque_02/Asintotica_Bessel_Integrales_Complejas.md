---
title: "Asintótica de Bessel y Representación Integral en el Plano Complejo"
tags: [concept, bessel-asymptotics, complex-analysis, contour-integrals]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Asintótica de Bessel y Representación Integral en el Plano Complejo

## 📌 Idea Central

Para distancias grandes ($kr \gg 1$), las ondas cilíndricas descritas por funciones de Bessel se comportan localmente como ondas planas moduladas por una envolvente de caída geométrica $1/\sqrt{r}$. Estas propiedades se deducen rigurosamente a partir de representaciones integrales de contorno en el plano complejo usando el **método de la fase estacionaria** y el **método de descenso más pronunciado** (*steepest descent*).

## 🧮 Ecuaciones Clave

### Representación Integral de Sommerfeld / Hankel:
$$ J_\nu(z) = \frac{1}{2\pi} \int_{-\pi}^\pi e^{i(z \sin\theta - \nu\theta)} d\theta \quad (\nu \in \mathbb{Z}) $$
$$ H_\nu^{(1)}(z) = \frac{1}{i\pi} \int_{-\infty}^{\infty + i\pi} e^{z \sinh t - \nu t} dt $$

### Comportamiento Asintótico ($x \to \infty$):
$$ J_\nu(x) \sim \sqrt{\frac{2}{\pi x}} \cos\left( x - \frac{\nu\pi}{2} - \frac{\pi}{4} \right) $$
$$ Y_\nu(x) \sim \sqrt{\frac{2}{\pi x}} \sin\left( x - \frac{\nu\pi}{2} - \frac{\pi}{4} \right) $$
$$ H_\nu^{(1)}(x) = J_\nu(x) + i Y_\nu(x) \sim \sqrt{\frac{2}{\pi x}} e^{i\left( x - \frac{\nu\pi}{2} - \frac{\pi}{4} \right)} $$

La función de Hankel $H_\nu^{(1)}(kr)$ satisface exactamente la **condición de radiación de Sommerfeld** para ondas cilíndricas salientes $e^{i(kr - \omega t)}$.

## 🔗 Conceptos Relacionados

- **Teoría de difracción**: [[Concepts/Bloque_02/Difraccion_Cilindro_Bessel_Modificadas|Difracción por Cilindro]]
- **Dispersión clásica**: [[Concepts/Bloque_02/Difraccion_Rayleigh_Seccion_Eficaz|Difracción de Rayleigh]]
