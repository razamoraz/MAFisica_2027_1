# 💻 Laboratorios Computacionales y Notebooks

Esta carpeta contiene los materiales y simulaciones en **Python** y **Julia** para las prácticas numéricas del curso de **Matemáticas Avanzadas de la Física (2027-1)**.

Están diseñados para ejecutarse tanto en la nube mediante **Google Colab** (con un solo clic) como en entornos locales (JupyterLab / Notebooks / VS Code).

---

## 🚀 Cuadernos Disponibles y Acceso Directo

| # | Cuaderno / Tema | Descripción | Google Colab |
| :-: | :--- | :--- | :---: |
| **01** | [`01_Bessel_Drums.ipynb`](https://github.com/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/01_Bessel_Drums.ipynb) | **El Tambor de Bessel — Vibraciones de una Membrana Circular**: Derivación de la ecuación de Bessel en coordenadas polares, cálculo numérico de ceros $\alpha_{m,n}$ con `scipy.special`, visualización interactiva 3D de modos normales $(m,n)$ y animación con `k3d`/`ipywidgets` (*Tema 1, Sesiones 4–6; Arfken Cap. 11, Lebedev Cap. 7*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/01_Bessel_Drums.ipynb) |
| **02** | [`02_Sturm_Liouville.ipynb`](https://github.com/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/02_Sturm_Liouville.ipynb) | **Teoría de Sturm–Liouville y Familias Ortogonales — De Fourier a las Funciones Especiales**: Operador canónico autoadjunto, Fourier como caso fundamental ($p=1, q=0, w=1$), gran tabla de funciones especiales (Legendre, Chebyshev I/II, Hermite, Laguerre, Jacobi, Gegenbauer, Bessel), verificación numérica de ortogonalidad con matrices de Gram y widget interactivo de series generalizadas (*Tema 1, Sesión 3; Arfken Cap. 9*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/02_Sturm_Liouville.ipynb) |
| **03** | [`03_SL_Quantum.ipynb`](https://github.com/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/03_SL_Quantum.ipynb) | **Sturm–Liouville en Mecánica Cuántica — Oscilador Armónico y Átomo Hidrogenoide**: Problemas singulares de Sturm–Liouville, Polinomios de Hermite y Laguerre asociados, comprobación simbólica con SymPy y visualizaciones 3D en WebGL (*Tema 1, Sesión 5*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/03_SL_Quantum.ipynb) |
| **04** | [`04_Membrana_Rectangular_Examen.ipynb`](https://github.com/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/04_Membrana_Rectangular_Examen.ipynb) | **Vibraciones de una Membrana Rectangular — Solución Completa del Examen Parcial**: Separación de variables, formulación canónica de Sturm–Liouville, cálculo de frecuencias propias $\omega_{mn} = c\pi\sqrt{m^2+n^2}$, base ortonormal 2D, expansión de la condición inicial plana $u_0=1$, fenómeno de Gibbs y visualizaciones 2D de atlas modal, paridad y evolución temporal (*Tema 1, Sesión 7/8*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/04_Membrana_Rectangular_Examen.ipynb) |

---

## 🛠️ Configuración y Ejecución en Local (usando `make`)

Para reproducir y ejecutar los cuadernos en tu computadora con todas las dependencias científicas (`numpy`, `scipy`, `matplotlib`, `jupyter`), sigue estos pasos:

### 1. Clonar el repositorio
```bash
git clone https://github.com/razamoraz/MAFisica_2027_1.git
cd MAFisica_2027_1
```

### 2. Configurar el entorno virtual con `make setup`
Ejecuta el siguiente comando en la terminal:
```bash
make setup
```
Este comando automáticamente:
- Crea un entorno virtual aislado en `.venv`.
- Actualiza `pip` e instala todas las dependencias científicas requeridas especificadas en `requirements.txt`.
- Inicializa el archivo `.env` de configuración si no existe.

### 3. Iniciar Jupyter
Para abrir la interfaz interactiva en tu navegador:
```bash
# Para iniciar Jupyter Notebook clásico:
make jupyter

# O para iniciar JupyterLab:
make lab
```

### 4. Validar la ejecución de todos los cuadernos
Puedes verificar que todos los cuadernos de Python se ejecuten correctamente sin errores con:
```bash
make test-notebooks
```

### 5. Uso manual alternativo (sin `make`)
Si prefieres activar el entorno virtual directamente:
```bash
source .venv/bin/activate
jupyter notebook Notebooks/
```
Para desactivar el entorno al terminar:
```bash
deactivate
```
