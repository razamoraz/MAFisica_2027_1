---
title: "Conducción de Calor en una Esfera y Geofísica"
tags: [concept, heat-equation, spherical-harmonics, geophysics]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
  - "[[Sources/Books/Lebedev_1970]]"
---

# Conducción de Calor en una Esfera y Geofísica

## 📌 Idea Central

La ecuación de conducción de calor en una esfera sólida de radio $R$ (modelo canónico para el enfriamiento y calentamiento de la Tierra y cuerpos planetarios) se resuelve mediante separación de variables en coordenadas esféricas $(r, \theta, \phi)$, combinando funciones esféricas de Bessel para la parte radial con polinomios de Legendre para la parte angular.

## 🧮 Ecuaciones Clave

Ecuación de difusión térmica con difusividad térmica $\kappa$:
$$ \frac{\partial T}{\partial t} = \kappa \nabla^2 T = \kappa \left[ \frac{1}{r^2}\frac{\partial}{\partial r}\left(r^2 \frac{\partial T}{\partial r}\right) + \frac{1}{r^2\sin\theta}\frac{\partial}{\partial \theta}\left(\sin\theta \frac{\partial T}{\partial \theta}\right) + \frac{1}{r^2\sin^2\theta}\frac{\partial^2 T}{\partial \phi^2} \right] $$

Para simetría azimutal ($\partial/\partial \phi = 0$), proponiendo $T(r,\theta,t) = R(r)\Theta(\theta)\mathcal{T}(t)$:
$$ \mathcal{T}(t) = e^{-\kappa \lambda^2 t} $$
$$ \Theta(\theta) = P_n(\cos\theta) \quad (\text{Polinomio de Legendre de grado } n) $$
$$ R(r) = j_n(\lambda r) = \sqrt{\frac{\pi}{2\lambda r}} J_{n+1/2}(\lambda r) \quad (\text{Función esférica de Bessel}) $$

Solución general:
$$ T(r,\theta,t) = \sum_{n=0}^\infty \sum_{m=1}^\infty A_{nm} j_n\left(\frac{\alpha_{n,m} r}{R}\right) P_n(\cos\theta) e^{-\kappa \left(\frac{\alpha_{n,m}}{R}\right)^2 t} $$

## 🔗 Conceptos Relacionados

- **Parte angular**: [[Concepts/Bloque_04/Polinomios_Legendre|Polinomios de Legendre]]
- **Parte radial**: [[Concepts/Bloque_01/Funciones_Bessel|Funciones de Bessel]]
