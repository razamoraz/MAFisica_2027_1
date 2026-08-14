---
title: "GitHub Pages Initialization & Troubleshooting Guide"
---

# 🚀 GitHub Pages Initialization & Troubleshooting Guide

This guide contains the prompt and checklist to use when initializing a new course vault repository from this template or troubleshooting GitHub Pages deployment issues.

---

## 🤖 Agent Initialization Prompt

Use this prompt when initializing an agent in a newly cloned/instantiated vault:

```markdown
You are initializing a new course vault repository from this template for the course: "[COURSE_NAME]" (Repository: [GITHUB_USERNAME]/[REPO_NAME]).

Please perform the following initialization and configuration tasks:

1. **Fix GitHub Actions Deployment Workflow (`.github/workflows/deploy.yml`)**:
   - Ensure the Quartz build step specifies the vault root directory:
     ```yaml
     - name: Build Quartz
       run: npx quartz build -d . --output public
     ```
     *(The default Quartz build looks for a `content/` folder, but this template stores notes directly at the root, so `-d .` is mandatory).*

2. **Configure Quartz Site (`quartz.config.yaml`)**:
   - **`baseUrl`**: Set to `"[GITHUB_USERNAME].github.io/[REPO_NAME]"` (or your custom domain if applicable).
   - **`pageTitle`**: Update to reflect the course name (e.g., `"📚 [COURSE_NAME] Brain"`).
   - **Disable CNAME generation**: If using standard GitHub Pages (`*.github.io`), set `@quartz-community/cname` to `enabled: false` so it doesn't emit a placeholder `CNAME` file that breaks deployment.
   - **Ignore Patterns**: Ensure `.agents`, `.venv`, `local_index`, `output`, `public`, `scripts`, and `Templates` are in `ignorePatterns`.

3. **Validate Local Build**:
   - Run `npm install` (or `npm ci`).
   - Run `make site-build` to verify that all markdown files in `.` are found and compiled into `public/` without errors or stray `public/CNAME` files.

4. **Update Documentation**:
   - Update `README.md` and `Syllabus.md` with relevant course details, objectives, and references.
```

---

### 💡 Placeholders to fill when using the prompt:
- `[COURSE_NAME]`: e.g., `Física Estadística 2027-1`
- `[GITHUB_USERNAME]`: e.g., `razamoraz`
- `[REPO_NAME]`: e.g., `FIsicaESTAdistica_2027_1`
