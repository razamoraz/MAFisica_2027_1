---
title: "Funciones de Green 1D y Distribuciones"
tags: [concept, green-functions, inverse-operators, delta-dirac]
primary_sources:
  - "[[Sources/Books/Arfken_1966]]"
---

# Funciones de Green 1D y Distribuciones

## 📌 Idea Central

La función de Green $G(x, x')$ representa la respuesta impulsional de un sistema físico lineal gobernado por un operador diferencial $\mathcal{L}$ ante una fuente puntual modelada por la delta de Dirac $\delta(x - x')$. Provee la representación integral explícita del operador inverso $\mathcal{L}^{-1}$.

## 🧮 Ecuaciones Clave

Para el problema de contorno no homogéneo:
$$ \mathcal{L} u(x) = f(x), \quad x \in [a, b] $$
con condiciones de frontera homogéneas, la función de Green satisface:
$$ \mathcal{L} G(x, x') = \delta(x - x') $$

La solución viene dada directamente por convolución:
$$ u(x) = \int_a^b G(x, x') f(x') dx' $$

### Propiedades de la Función de Green en 1D:
1. **Continuidad en $x = x'$**:
   $$ G(x'^+, x') - G(x'^-, x') = 0 $$
2. **Salto en la primera derivada**:
   $$ \left. \frac{dG}{dx} \right|_{x=x'^+} - \left. \frac{dG}{dx} \right|_{x=x'^-} = \frac{1}{p(x')} $$
3. **Simetría y reciprocidad** (para operadores autoadjuntos):
   $$ G(x, x') = G(x', x) $$

### Representación Espectral Bilineal:
$$ G(x, x') = \sum_{n=1}^\infty \frac{y_n(x) y_n(x')}{\lambda_n N_n} $$

## 🔗 Conceptos Relacionados

- **Operador diferencial**: [[Concepts/Bloque_01/Problema_Sturm_Liouville|Problema de Sturm-Liouville]]
- **Resolvente en el plano complejo**: [[Concepts/Bloque_03/Resonancias_Polos_Resolvente|Polos del Operador Resolvente]]
