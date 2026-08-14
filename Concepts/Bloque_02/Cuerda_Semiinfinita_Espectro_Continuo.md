---
title: "Cuerda Semiinfinita y Espectro Continuo"
tags: [concept, continuous-spectrum, semi-infinite-domain, wave-scattering]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Cuerda Semiinfinita y Espectro Continuo

## 📌 Idea Central

Al extender el dominio espacial de un sistema oscilatorio de un intervalo finito $[0, L]$ a una región no acotada $[0, \infty)$ o $(-\infty, \infty)$, los valores propios discretos $\lambda_n$ se densifican hasta fusionarse en un **espectro continuo** $\lambda \in [0, \infty)$. Las funciones propias ya no pertenecen a $L^2$ en sentido estricto, sino que se normalizan a la delta de Dirac como **funciones propias generalizadas** (ondas viajeras e incidentes/reflejadas).

## 🧮 Ecuaciones Clave

Para la cuerda semiinfinita $x \in [0, \infty)$ con extremo fijo $u(0,t) = 0$:
$$ \frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2} $$

Las funciones propias espaciales continuas parametrizadas por el número de onda $k \ge 0$ son:
$$ \phi(x; k) = \sin(kx) $$

Ortogonalidad en el continuo (normalización delta):
$$ \int_0^\infty \sin(kx) \sin(k'x) dx = \frac{\pi}{2} \delta(k - k') $$

La superposición general se convierte en una integral de Fourier seno:
$$ u(x,t) = \int_0^\infty \sin(kx) \left[ A(k) \cos(kct) + B(k) \sin(kct) \right] dk $$

## 🔗 Conceptos Relacionados

- **Límite desde el discreto**: [[Concepts/Bloque_01/Cuerda_Vibrante_Separacion_Variables|Cuerda Finita]] $\to$ [[Concepts/Bloque_02/Transformada_Fourier_Continuo|Transformada de Fourier]]
- **Teoría Espectral Cuántica**: [[Concepts/Bloque_03/Pozo_Potencial_Estados_Ligados_Libres|Estados del Continuo en Pozos]]
