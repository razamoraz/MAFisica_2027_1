---
title: "Ondas Elásticas Acopladas y Medios Vibrantes"
tags: [concept, elastic-waves, coupled-oscillators, continuous-media]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Ondas Elásticas Acopladas y Medios Vibrantes

## 📌 Idea Central

El estudio del acoplamiento entre estructuras mecánicas localizadas (vigas, masas concentradas u osciladores) y medios elásticos continuos semiinfinitos o infinitos describe fenómenos de dispersión de energía, atrapamiento de modos y amortiguamiento por radiación sin disipación térmica interna.

## 🧮 Ecuaciones Clave

Para una cuerda continua acoplada a un oscilador de masa $M$ y resorte $K$ en $x = 0$:
$$ \rho \frac{\partial^2 u}{\partial t^2} = T_0 \frac{\partial^2 u}{\partial x^2} - \left( M\frac{\partial^2 u}{\partial t^2} + Ku \right) \delta(x) $$

Condición de salto dinámico en $x = 0$:
$$ T_0 \left[ \left. \frac{\partial u}{\partial x} \right|_{0^+} - \left. \frac{\partial u}{\partial x} \right|_{0^-} \right] = M \frac{\partial^2 u(0,t)}{\partial t^2} + K u(0,t) $$

### Matriz de Dispersión y Coeficiente de Transmisión:
Para ondas monocromáticas $u(x,t) = e^{-i\omega t}\psi(x)$:
$$ T(\omega) = \frac{2 T_0 k}{2 T_0 k + i (M\omega^2 - K)}, \quad k = \frac{\omega}{c} $$

Cuando $\omega^2 \approx K/M$, ocurre una **resonancia** donde la estructura concentrada absorbe y reemite ondas coherentemente hacia el continuo.

## 🔗 Conceptos Relacionados

- **Atrapamiento y Polos**: [[Concepts/Bloque_03/Resonancias_Polos_Resolvente|Polos del Operador Resolvente]]
- **Green 1D**: [[Concepts/Bloque_01/Funcion_Green_1D|Funciones de Green 1D]]
