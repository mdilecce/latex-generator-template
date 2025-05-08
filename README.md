# LaTeX Generator Template

[![Build LaTeX](https://github.com/<your-username>/<your-repo>/actions/workflows/latex_jobs.yaml/badge.svg)](https://github.com/<your-username>/<your-repo>/actions/workflows/latex_jobs.yaml)

This project is a template that uses GitHub Actions to automatically compile LaTeX files whenever changes are pushed to the remote repository. It simplifies the process of generating PDFs from LaTeX source files.

## Features
- Automated LaTeX compilation using GitHub Actions.
- Customizable YAML configuration for different compilation jobs.
- Optional integration with Overleaf for collaborative editing.

## Getting Started

### Create a New Repository
1. Click the "Use this template" button on GitHub to create a new repository based on this template.

### YAML Configuration
The `latex_jobs.yaml` file defines the compilation jobs. Below is a brief explanation of its key fields:

- **`proj_name`**: Name of your project.
- **`jobname`**: Label for the compilation job.
- **`compile`**: Set to `true` to enable compilation.
- **`file`**: Path to the main LaTeX document (e.g., `main.tex`).
- **`latex_compiler`**: Choose a compiler (`pdflatex`, `xelatex`, or `lualatex`).
- **`draft`**: Set to `true` for draft mode (faster compilation).
- **`output_dir`**: Directory where compiled files will be saved.
- **`output_format`**: Output format (`pdf` or `dvi`).
- **`lua_script`**: Path to a Lua script (only for `lualatex`).
- **`extra_args`**: Additional arguments for the LaTeX compiler.

### Workflow with Overleaf (Optional)
1. Link your GitHub account with Overleaf.
2. Import the project from GitHub into Overleaf to edit the LaTeX source files collaboratively.
3. Push changes from Overleaf back to GitHub to trigger the compilation workflow.

## How It Works
1. Push your LaTeX files to the repository.
2. GitHub Actions automatically runs the workflow defined in `latex_jobs.yaml`.
3. The compiled PDF is saved in the specified output directory.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.