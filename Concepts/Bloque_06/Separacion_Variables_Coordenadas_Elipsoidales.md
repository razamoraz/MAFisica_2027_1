---
title: "Separación de Variables en Coordenadas Elipsoidales y Problemas de Potencial"
tags: [concept, ellipsoidal-coordinates, potential-theory, mathieu-functions, pde]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Separación de Variables en Coordenadas Elipsoidales y Problemas de Potencial

## 📌 Idea Central

La resolución de la ecuación de Laplace $\nabla^2 V = 0$ y de la ecuación de Helmholtz $\nabla^2 \psi + k^2 \psi = 0$ en geometrías con fronteras elípticas (guías de onda elípticas, membranas elípticas o conductores elipsoidales cargados) requiere el uso de coordenadas cilíndricas elípticas $(\mu, \nu, z)$ o coordenadas elipsoidales $(\xi, \eta, \zeta)$, desembocando naturalmente en funciones de Mathieu ordinarias y modificadas.

## 🧮 Ecuaciones Clave

### Coordenadas Cilíndricas Elípticas:
$$ x = d \cosh\mu \cos\nu, \quad y = d \sinh\mu \sin\nu, \quad z = z $$
donde $2d$ es la distancia focal inter-focos.

El Laplaciano en el plano transversal se expresa como:
$$ \nabla_\perp^2 \psi = \frac{1}{d^2(\cosh^2\mu - \cos^2\nu)} \left( \frac{\partial^2\psi}{\partial \mu^2} + \frac{\partial^2\psi}{\partial \nu^2} \right) $$

Para la ecuación de Helmholtz $\nabla_\perp^2 \psi + k^2 \psi = 0$, proponiendo $\psi(\mu,\nu) = M(\mu)N(\nu)$ con $q = \frac{k^2 d^2}{4}$:
1. **Ecuación angular (Mathieu periódica)**:
   $$ \frac{d^2 N}{d\nu^2} + (a - 2q\cos(2\nu))N = 0 \implies N(\nu) = \text{ce}_m(\nu, q) \text{ o } \text{se}_m(\nu, q) $$
2. **Ecuación radial (Mathieu modificada)**:
   $$ \frac{d^2 M}{d\mu^2} - (a - 2q\cosh(2\mu))M = 0 \implies M(\mu) = \text{Ce}_m(\mu, q) \text{ o } \text{Se}_m(\mu, q) $$

## 🔗 Conceptos Relacionados

- **Teoría de Mathieu**: [[Concepts/Bloque_06/Ecuacion_Mathieu_Estabilidad|Ecuación de Mathieu y Estabilidad]]
- **Otros sistemas coordenados**: [[Concepts/Bloque_01/Funciones_Bessel|Coordenadas Cilíndricas (Bessel)]], [[Concepts/Bloque_04/Polinomios_Legendre|Coordenadas Esféricas (Legendre)]]
