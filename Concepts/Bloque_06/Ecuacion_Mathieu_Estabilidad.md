---
title: "Ecuación de Mathieu y Diagramas de Estabilidad"
tags: [concept, mathieu-equation, parametric-resonance, stability-diagrams, floquet-theory]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Ecuación de Mathieu y Diagramas de Estabilidad

## 📌 Idea Central

La ecuación de Mathieu es el prototipo canónico de una ecuación diferencial lineal de segundo orden con coeficientes periódicos (teoría de Floquet / Bloch). Modela la **resonancia paramétrica** (péndulo con pivote vibrante, trampas iónicas de Paul, condensados de Bose-Einstein en redes ópticas periódicas) y la propagación de ondas en geometrías elípticas.

## 🧮 Ecuaciones Clave

### Ecuación Canónica de Mathieu:
$$ \frac{d^2 y}{dz^2} + (a - 2q \cos(2z))y = 0 $$
donde $a$ es el parámetro característico y $q$ es la amplitud de la modulación paramétrica.

### Teorema de Floquet:
Toda solución puede escribirse en la forma:
$$ y(z) = e^{\mu z} \phi(z), \quad \phi(z + \pi) = \phi(z) $$
donde $\mu$ es el exponente característico de Floquet.

- **Zona Estable**: $\mu = i\beta$ es puramente imaginario $\implies$ Soluciones acotadas y cuasiperiódicas.
- **Zona Inestable (Resonancia Paramétrica)**: $\text{Re}(\mu) \neq 0 \implies$ Soluciones que crecen exponencialmente hacia el infinito ($y(z) \sim e^{|\text{Re}(\mu)| z}$).

### Curvas de Transición (Diagrama de Ince-Strutt):
Las fronteras entre estabilidad e inestabilidad corresponden a las soluciones periódicas de orden entero:
- Funciones de Mathieu cosenoidales: $\text{ce}_m(z, q)$ correspondientes a las curvas $a_m(q)$.
- Funciones de Mathieu senoidales: $\text{se}_m(z, q)$ correspondientes a las curvas $b_m(q)$.

## 🔗 Conceptos Relacionados

- **Geometría elíptica**: [[Concepts/Bloque_06/Separacion_Variables_Coordenadas_Elipsoidales|Coordenadas Elipsoidales]]
- **Estabilidad de osciladores**: [[Concepts/Bloque_03/Ondas_Elasticas_Acopladas|Ondas Acopladas]]
