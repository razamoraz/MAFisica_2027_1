---
title: "Resonancias, Amortiguamiento por Radiación y Polos del Resolvente"
tags: [concept, resonances, resolvent-operator, complex-plane, radiation-damping]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Resonancias, Amortiguamiento por Radiación y Polos del Resolvente

## 📌 Idea Central

Las resonancias físicas (estados metaestables o cuasiligados con tiempo de vida finito) corresponden formalmente a **polos en el plano complejo de frecuencias o momentos $(\omega, k)$ del operador resolvente** $\mathcal{R}(z) = (\mathcal{L} - z)^{-1}$ o de la matriz de dispersión $S(k)$. La parte real del polo define la frecuencia resonante del sistema, mientras que la parte imaginaria determina la tasa de amortiguamiento por radiación hacia el continuo.

## 🧮 Ecuaciones Clave

### Operador Resolvente y Función de Green:
$$ (\mathcal{L} - z I) G(x, x'; z) = \delta(x - x') $$

### Posición del Polo en el Semi-Plano Inferior:
$$ z_R = E_R - i \frac{\Gamma}{2} \quad \text{o} \quad \omega_R = \omega_0 - i \gamma_R $$
donde:
- $\omega_0$: Frecuencia propia de oscilación de la resonancia.
- $\gamma_R = \frac{\Gamma}{2\hbar}$: Tasa de decaimiento por emisión de radiación hacia el continuo.
- Tiempo de vida característico: $\tau = 1/\gamma_R$.

### Forma de Línea de Breit-Wigner / Lorentziana:
La sección eficaz de dispersión o respuesta en frecuencia exhibe el perfil característico:
$$ \sigma(\omega) \propto \frac{1}{(\omega - \omega_0)^2 + \gamma_R^2} $$

## 🔗 Conceptos Relacionados

- **Acoplamiento elástico**: [[Concepts/Bloque_03/Ondas_Elasticas_Acopladas|Ondas Elásticas Acopladas]]
- **Inversión de Fourier/Laplace**: [[Concepts/Bloque_05/Inversion_Bromwich_Velocidad_Grupo_Senal|Contorno de Bromwich]]
