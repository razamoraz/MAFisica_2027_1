# 💻 Laboratorios Computacionales y Notebooks (MAF)

Esta carpeta contiene los cuadernos interactivos en **Python** y **Julia** para los talleres computacionales del curso **Matemáticas Avanzadas de la Física (MAF)** en la Facultad de Ciencias, UNAM, diseñados para ejecutarse en **Google Colab** o localmente (JupyterLab / VS Code / Pluto.jl).

---

## 📁 Cuadernos por Bloque Temático

### 🐍 Python (`Notebooks/Python/`)
1. **`01_Bessel_Drums.ipynb`**:
   - Derivación completa de la ecuación de Bessel a partir de la membrana circular vibrante.
   - Visualización interactiva 3D de modos normales con `k3d` y animación con `ipywidgets`.
   - Cálculo numérico de ceros de Bessel $\alpha_{m,n}$ con `scipy.special`.
2. **`02_Rayleigh_Scattering_Simulation.ipynb`**:
   - Simulación de difracción electromagnética y dispersión de Rayleigh.
   - Cálculo de sección eficaz diferencial y visualización de campos cercanos/lejanos en obstáculos cilíndricos.
3. **`03_Mathieu_Stability_Charts.ipynb`**:
   - Cálculo de curvas de transición $a_m(q), b_m(q)$ y diagramas de estabilidad de Ince-Strutt usando métodos espectrales.

### 🔴 Julia (`Notebooks/Julia/`)
- Cuadernos de alto rendimiento para el cálculo de espectros de operadores diferenciales, integración del resolvente en el plano complejo y simulación de ondas en solitones KdV.

---

## 🚀 Cómo ejecutar en Google Colab

Puedes abrir cualquiera de los cuadernos directamente en Google Colab cargando el archivo `.ipynb` desde la interfaz o clonando el repositorio.
