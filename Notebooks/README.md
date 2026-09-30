# 💻 Laboratorios Computacionales y Notebooks

Esta carpeta contiene los materiales y simulaciones en **Python** y **Julia** para las prácticas numéricas del curso de **Matemáticas Avanzadas de la Física (2027-1)**.

Están diseñados para ejecutarse tanto en la nube mediante **Google Colab** (con un solo clic) como en entornos locales (JupyterLab / Notebooks / VS Code).

---

## 🚀 Cuadernos Disponibles y Acceso Directo

| # | Cuaderno / Tema | Descripción | Google Colab |
| :-: | :--- | :--- | :---: |
| **01** | [`01_Bessel_Drums.ipynb`](https://github.com/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/01_Bessel_Drums.ipynb) | **El Tambor de Bessel — Vibraciones de una Membrana Circular**: Derivación de la ecuación de Bessel en coordenadas polares, cálculo numérico de ceros $\alpha_{m,n}$ con `scipy.special`, visualización interactiva 3D de modos normales $(m,n)$ y animación con `k3d`/`ipywidgets` (*Tema 1, Sesiones 4–6; Arfken Cap. 11, Lebedev Cap. 7*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/01_Bessel_Drums.ipynb) |
| **02** | `02_Rayleigh_Scattering_Simulation.ipynb` *(En desarrollo)* | **Dispersión de Rayleigh y Difracción**: Simulación de difracción electromagnética por un cilindro dieléctrico, cálculo de sección eficaz diferencial $d\sigma/d\Omega$ y visualización de campos cercanos/lejanos (*Tema 2, Sesión 15*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/02_Rayleigh_Scattering_Simulation.ipynb) |
| **03** | `03_Mathieu_Stability_Charts.ipynb` *(En desarrollo)* | **Ecuación de Mathieu y Diagramas de Estabilidad**: Cálculo numérico de curvas de transición $a_m(q), b_m(q)$ y diagramas de estabilidad de Ince-Strutt (lenguas de Arnold) usando métodos espectrales (*Tema 6, Sesión 31*). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/razamoraz/MAFisica_2027_1/blob/main/Notebooks/Python/03_Mathieu_Stability_Charts.ipynb) |

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
