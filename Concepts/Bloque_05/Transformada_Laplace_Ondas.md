---
title: "Transformada de Laplace en EDPs y Propagación de Ondas"
tags: [concept, laplace-transform, wavefronts, pde-initial-values]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Transformada de Laplace en EDPs y Propagación de Ondas

## 📌 Idea Central

La transformada unilateral de Laplace es la herramienta analítica estándar para resolver problemas de valor inicial y de contorno (PVI-PVC) en ecuaciones diferenciales en derivadas parciales. Convierte derivadas temporales directamente en términos algebraicos incorporando automáticamente las condiciones iniciales en $t = 0$. En problemas hiperbólicos (ondas), preserva la causalidad estricta y la velocidad finita de propagación del frente de onda.

## 🧮 Ecuaciones Clave

### Definición y Propiedad Fundamental de Derivada:
$$ \mathcal{L}\{f(t)\}(s) = F(s) = \int_0^\infty f(t) e^{-st} dt, \quad \text{Re}(s) > \gamma_0 $$
$$ \mathcal{L}\left\{\frac{\partial^2 u}{\partial t^2}\right\} = s^2 U(x,s) - s u(x,0) - \left.\frac{\partial u}{\partial t}\right|_{t=0} $$

Para la cuerda semiinfinita en reposo excitada en el origen $u(0,t) = f(t)$:
$$ \frac{d^2 U}{dx^2} - \frac{s^2}{c^2} U(x,s) = 0 \implies U(x,s) = F(s) e^{-\frac{s}{c}x} $$

Aplicando la propiedad de desplazamiento temporal:
$$ u(x,t) = \mathcal{L}^{-1}\left\{ F(s) e^{-s(x/c)} \right\} = f\left(t - \frac{x}{c}\right) \Theta\left(t - \frac{x}{c}\right) $$
donde $\Theta$ es la función escalón unitario de Heaviside, demostrando que la perturbación viaja a velocidad finita $c$ sin precursores acausales.

## 🔗 Conceptos Relacionados

- **Inversión compleja**: [[Concepts/Bloque_05/Inversion_Bromwich_Velocidad_Grupo_Senal|Contorno de Bromwich]]
- **Comparación con Fourier**: [[Concepts/Bloque_02/Transformada_Fourier_Continuo|Transformada de Fourier]]
