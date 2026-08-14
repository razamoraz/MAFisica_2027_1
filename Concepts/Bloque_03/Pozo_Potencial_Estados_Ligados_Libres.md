---
title: "Pozo de Potencial: Estados Ligados vs Estados Libres"
tags: [concept, quantum-mechanics, potential-wells, bound-states, continuous-spectrum]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Pozo de Potencial: Estados Ligados vs Estados Libres

## 📌 Idea Central

En sistemas cuánticos y clásicos no acotados con potenciales localizados $V(x) \to 0$ cuando $|x| \to \infty$, el operador Hamiltoniano / Sturm-Liouville $\hat{H} = -\frac{d^2}{dx^2} + V(x)$ presenta una estructura espectral dual:
1. **Espectro Discreto ($E < 0$)**: Número finito de estados ligados normalizables $\psi_n \in L^2(\mathbb{R})$.
2. **Espectro Continuo ($E > 0$)**: Continuo de estados libres / dispersados $\psi_k(x)$ no integrables en $L^2$.

## 🧮 Ecuaciones Clave

Ecuación estacionaria de Schrödinger 1D:
$$ -\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V(x)\psi(x) = E\psi(x) $$

Para un pozo finito de profundidad $V_0$ y ancho $2a$:
- Para $E = -\frac{\hbar^2\kappa^2}{2m} < 0$:
  $$ \psi(x) \propto e^{-\kappa |x|} \quad (|x| > a), \quad \kappa = \frac{\sqrt{2m|E|}}{\hbar} $$
- Para $E = \frac{\hbar^2 k^2}{2m} > 0$:
  $$ \psi(x) \sim \begin{cases} e^{ikx} + R(k) e^{-ikx}, & x \to -\infty \\ T(k) e^{ikx}, & x \to +\infty \end{cases} $$
  donde $R(k)$ y $T(k)$ son los coeficientes de reflexión y transmisión.

Conservación de flujo de probabilidad:
$$ |R(k)|^2 + |T(k)|^2 = 1 $$

## 🔗 Conceptos Relacionados

- **Completitud global**: [[Concepts/Bloque_03/Representacion_Espectral_Mixta|Representación Espectral Mixta]]
- **Casos especiales sin reflexión**: [[Concepts/Bloque_03/Potenciales_Reflexion_Cero_Solitones|Potenciales Reflexión Cero]]
- **Polos de dispersión**: [[Concepts/Bloque_03/Resonancias_Polos_Resolvente|Polos del Resolvente]]
