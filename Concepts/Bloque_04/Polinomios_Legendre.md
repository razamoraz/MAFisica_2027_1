---
title: "Polinomios y Funciones de Legendre"
tags: [concept, legendre-polynomials, spherical-harmonics, special-functions]
primary_sources:
  - "[[Sources/Books/Lebedev_1970]]"
  - "[[Sources/Books/Arfken_1966]]"
---

# Polinomios y Funciones de Legendre

## 📌 Idea Central

Los polinomios de Legendre $P_n(x)$ son las soluciones regulares acotadas en $x \in [-1, 1]$ (donde $x = \cos\theta$) de la ecuación diferencial de Legendre. Forman la base ortogonal fundamental para la descripción de campos gravitacionales, electrostáticos y térmicos con simetría esférica.

## 🧮 Ecuaciones Clave

### Ecuación Diferencial de Legendre:
$$ (1 - x^2)\frac{d^2 y}{dx^2} - 2x \frac{dy}{dx} + n(n+1)y = 0, \quad x \in [-1, 1] $$

### Fórmula de Rodrigues:
$$ P_n(x) = \frac{1}{2^n n!} \frac{d^n}{dx^n} \left[ (x^2 - 1)^n \right] $$

Primeros polinomios:
$$ P_0(x) = 1, \quad P_1(x) = x, \quad P_2(x) = \frac{1}{2}(3x^2 - 1), \quad P_3(x) = \frac{1}{2}(5x^3 - 3x) $$

### Relación de Ortogonalidad:
$$ \int_{-1}^{1} P_n(x) P_m(x) dx = \frac{2}{2n + 1} \delta_{nm} $$

### Relaciones de Recurrencia de Bonnet:
$$ (2n + 1)x P_n(x) = (n + 1)P_{n+1}(x) + n P_{n-1}(x) $$
$$ P'_{n+1}(x) - P'_{n-1}(x) = (2n + 1)P_n(x) $$

### Función Generatriz (Potencial Electrostático Multipolo):
$$ \frac{1}{\sqrt{1 - 2xt + t^2}} = \sum_{n=0}^\infty P_n(x) t^n, \quad |t| < 1 $$

## 🔗 Conceptos Relacionados

- **Aplicación física**: [[Concepts/Bloque_04/Conduccion_Calor_Esfera|Conducción de Calor en Esfera]]
- **Teoría Sturm-Liouville**: [[Concepts/Bloque_01/Problema_Sturm_Liouville|Operadores de Sturm-Liouville]]
