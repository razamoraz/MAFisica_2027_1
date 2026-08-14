---
title: "Inversión por Contorno de Bromwich, Velocidad de Señal y Precursores"
tags: [concept, bromwich-contour, complex-inversion, signal-velocity, precursors]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Inversión por Contorno de Bromwich, Velocidad de Señal y Precursores

## 📌 Idea Central

La inversión de la transformada de Laplace en medios dispersivos o complejos requiere evaluar la **integral de inversión de Bromwich** (Mellin-Bromwich) a lo largo de una línea vertical en el plano complejo a la derecha de todas las singularidades. En medios dispersivos (donde $k(\omega)$ no es lineal), el frente de onda desarrolla oscilaciones transitorias de alta y baja frecuencia conocidas como **precursores de Sommerfeld y Brillouin**, mientras que la energía principal viaja a la **velocidad de grupo y de señal**.

## 🧮 Ecuaciones Clave

### Integral de Inversión de Bromwich:
$$ f(t) = \frac{1}{2\pi i} \int_{\gamma - i\infty}^{\gamma + i\infty} F(s) e^{st} ds, \quad \gamma > \gamma_0 $$

Cerrando el contorno hacia la izquierda mediante el Lema de Jordan, la integral se reduce a la suma de residuos en los polos y la integración a lo largo de cortes de ramificación:
$$ f(t) = \sum_{k} \operatorname{Res}\left( F(s) e^{st}, s_k \right) + \frac{1}{2\pi i} \oint_{\text{cortes}} F(s) e^{st} ds $$

### Velocidad de Fase, Grupo y Señal:
- **Velocidad de fase**: $v_p = \frac{\omega}{k(\omega)}$
- **Velocidad de grupo**: $v_g = \frac{d\omega}{dk}$
- **Precursores (Sommerfeld & Brillouin)**: Surgen de la evaluación asintótica por punto silla del contorno de Bromwich para $t \approx x/c$ antes del arribo de la señal principal.

## 🔗 Conceptos Relacionados

- **Operador Resolvente**: [[Concepts/Bloque_03/Resonancias_Polos_Resolvente|Polos del Resolvente]]
- **Transformada de Laplace**: [[Concepts/Bloque_05/Transformada_Laplace_Ondas|Transformada de Laplace en EDPs]]
