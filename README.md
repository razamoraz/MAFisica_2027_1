# 📐 Matemáticas Avanzadas de la Física (MAF) — Facultad de Ciencias, UNAM

A version-controlled, Obsidian-compatible course vault and learning system for **Matemáticas Avanzadas de la Física (MAF)** at **Facultad de Ciencias, UNAM (Semestre 2027-1)**, created and maintained by **Dr. Roberto Antonio Zamora Zamora**.

---

## 🌟 Overview & Architecture

This repository hosts the lecture notes, interactive knowledge graph, computational notebooks, syllabus, and project guides for the 33-session course in Mathematical Physics.

It integrates three foundational pillars:

1. **Obsidian Knowledge Vault (Public & Git-Tracked)**:
   - Atomic concept notes (`Concepts/`), lecture logs for 33 sessions (`Lectures/`), Map of Content (`MoC/MAF_MoC.md`), project guidelines (`Projects/`), and syllabus definition (`Syllabus.md`).
   - Rich Markdown frontmatter, LaTeX equation rendering (`$$...$$`), and Obsidian wikilinks (`[[Concept]]`).

2. **Public Static Web Interface via Quartz 5 (Automated Web Deployment)**:
   - Publishes the interactive vault to **GitHub Pages** (`https://razamoraz.github.io/MAFisica_2027_1/`).
   - Includes full-text search, visual graph view, backlinks, popover previews, and KaTeX rendering.

3. **Private PDF Indexing RAG Pipeline (Local & Private)**:
   - Python tools (`scripts/convert_and_index.py`, `scripts/query_local.py`) to convert textbook PDFs (Arfken, Lebedev) into searchable vector chunks via **LanceDB** for deep offline semantic retrieval without committing copyrighted PDFs.

---

## 📁 Repository Structure

```
.
├── Syllabus.md                         # Official Course Syllabus (Temario, 33 Sesiones, Evaluación 50/40/10)
├── index.md                            # Quartz static site homepage
├── Concepts/                           # Atomic concept notes by block
│   ├── Bloque_01/                      # Cuerda finita, Fourier, Bessel & Sturm-Liouville
│   ├── Bloque_02/                      # Dispersión, espectro continuo & difracción
│   ├── Bloque_03/                      # Espectro mixto, pozos cuánticos & resonancias
│   ├── Bloque_04/                      # Conducción de calor en esfera & Legendre
│   ├── Bloque_05/                      # Transformada de Laplace & frentes de onda
│   └── Bloque_06/                      # Ecuación de Mathieu & coordenadas elipsoidales
├── Lectures/                           # Chronological notes for all 33 sessions
│   ├── Sesion_01_Presentacion_Cuerda_Vibrante.md
│   ├── ...
│   └── Sesion_33_Cierre_Evaluacion_Proyectos.md
├── MoC/                                # Map of Content master index
│   └── MAF_MoC.md
├── Notebooks/                          # Google Colab notebooks for numerical methods
│   ├── Python/                         # Fourier-Bessel series, Rayleigh scattering, Mathieu charts
│   └── Julia/                          # High-performance spectral methods
├── Projects/                           # Final project guidelines & proposal templates
│   ├── Final_Project_Guide.md          # 40% Final Project Guide (7-15 min video + oral defense)
│   └── Paper_Proposal_Template.md      # Paper selection proposal template
├── Sources/                            # Metadata for textbooks and references
│   └── Books/
│       ├── Arfken_1966.md
│       └── Lebedev_1970.md
├── Templates/                          # Obsidian note templates
├── scripts/                            # Local Python RAG indexing & CLI query tools
├── .github/workflows/deploy.yml        # Quartz GitHub Pages deployment
├── quartz.config.yaml                  # Quartz configuration file
├── Makefile                            # Development shortcuts
└── README.md
```

---

## 🚀 Getting Started

### 1. Local Web Preview (Quartz)
Ensure Node.js 22+ is installed, then run:

```bash
# Install Node dependencies
npm install

# Preview site locally on http://localhost:8080
make site-dev

# Build static HTML production bundle into public/
make site-build
```

### 2. Private PDF RAG & Markdown Pipeline (Optional)
Convert local textbook PDFs into Markdown (`./output/<book>.md`) and build an offline LanceDB vector index:

```bash
# 1. Initialize Python environment & dependencies
make setup

# 2. Place PDFs in ./sample_pdfs/ (or set PDF_DIR in .env)

# 3a. Fast text mode (PyMuPDF)
make index

# 3b. Full LaTeX math OCR mode (Marker)
make index-marker

# 4. Search local vector index
make query
```

---

## 💯 Course Evaluation Framework (MAF 2027-1)

- **50% Exámenes Parciales (3 exámenes)**: Evaluaciones individuales al finalizar Bloques 1, 2 y 3. **+1 punto extra por examen** al entregar un formulario manuscrito (1 cuartilla).
- **40% Proyecto Final**: Análisis teórico o reproducción numérica de un artículo científico o problema avanzado (individual o máx. 3).
  - **Semana 8–9**: Entrega de propuesta escrita (1 cuartilla).
  - **Sesión 23**: Hito de avance y retroalimentación intermedia.
  - **Sesión 33**: Video expositivo (7–15 min) + Defensa oral (15 min).
- **10% Google Forms**: Participación activa (>90%) en cuestionarios conceptuales y retroalimentación semanal.
- **Política de IA**: Uso ético permitido y fomentado en código y redacción con prompts documentados. Prohibido en exámenes presenciales y defensas orales.

---

## 📚 Bibliografía Base

1. **Arfken, G. B.** (1966). *Mathematical Methods for Physicists*. Academic Press, N.Y., USA.
2. **Lebedev, N. N.** (1970). *Special Functions and Their Applications*. Dover Publications, N.Y., USA.
