---
title: "Transformada de Fourier como Límite del Espectro Discreto"
tags: [concept, fourier-transform, continuous-spectrum, spectral-theory]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Transformada de Fourier como Límite del Espectro Discreto

## 📌 Idea Central

La transformada de Fourier es la extensión natural de las series de Fourier al tomar el límite de longitud de caja $L \to \infty$. Representa la descomposición espectral de funciones en términos de ondas planas $e^{ikx}$, correspondientes al espectro continuo del operador momentum / Laplaciano en todo $\mathbb{R}$.

## 🧮 Ecuaciones Clave

Tomando el límite $L \to \infty$ en la serie compleja $f(x) = \sum_n c_n e^{i k_n x}$ con $\Delta k = \pi / L$:
$$ \mathcal{F}\{f\}(k) = \tilde{f}(k) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} f(x) e^{-ikx} dx $$

Transformada inversa de Fourier:
$$ f(x) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \tilde{f}(k) e^{ikx} dk $$

### Relación de Cierre y Teorema de Plancherel:
$$ \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik(x-x')} dk = \delta(x - x') $$
$$ \int_{-\infty}^\infty |f(x)|^2 dx = \int_{-\infty}^\infty |\tilde{f}(k)|^2 dk $$

## 🔗 Conceptos Relacionados

- **Origen discreto**: [[Concepts/Bloque_01/Series_Fourier|Series de Fourier]]
- **Generalización a problemas con estados ligados**: [[Concepts/Bloque_03/Representacion_Espectral_Mixta|Representación Espectral Mixta]]
