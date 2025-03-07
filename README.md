# LaTeX Thesis Template

A comprehensive LaTeX template for academic theses (Masters/PhD), designed to provide a clean, professional structure for your academic writing.

## 📋 Overview

This template provides a well-structured foundation for writing your thesis using LaTeX. It includes:

- Pre-configured thesis structure with chapters, appendices, and front/back matter
- Consistent formatting and styling
- Bibliography management using natbib
- Figure and table management
- Easy customization options

## 🗂️ Repository Structure

```
thesis_template/
├── thesis-main.tex     # Main document file that brings everything together
├── preamble.tex        # Package imports and document settings
├── thesis.sty          # Custom style definitions for the thesis
├── natbib.sty          # Bibliography style file
├── abstract.tex        # Template for thesis abstract
├── intro.tex           # Introduction chapter
├── chapter01.tex       # First chapter template
├── chapter02.tex       # Second chapter template
├── appendix01.tex      # First appendix template
├── appendix02.tex      # Second appendix template
├── end.tex             # End matter (acknowledgments, etc.)
└── figures/            # Directory for storing figures and images
```

## 🚀 Getting Started

### Prerequisites

To use this template, you need a LaTeX distribution installed on your system:

- **Windows**: [MiKTeX](https://miktex.org/) or [TeX Live](https://www.tug.org/texlive/)
- **macOS**: [MacTeX](https://www.tug.org/mactex/)
- **Linux**: TeX Live (`sudo apt-get install texlive-full` on Debian/Ubuntu)

A LaTeX editor is also recommended:
- [Overleaf](https://www.overleaf.com/) (online)
- [TeXstudio](https://www.texstudio.org/)
- [VS Code](https://code.visualstudio.com/) with LaTeX Workshop extension

### Using the Template

1. Clone this repository or download it as a ZIP file.
2. Open `thesis-main.tex` in your LaTeX editor.
3. Customize the metadata (title, author, etc.) in the preamble.
4. Begin writing your content in the provided chapter files.
5. Add your references to a `.bib` file and cite them in your text.

## 📝 Writing Your Thesis

### Basic Structure

The template is organized as follows:

1. **Front Matter**: Title page, abstract, table of contents.
2. **Main Content**: Introduction and chapters.
3. **Back Matter**: Appendices, bibliography, etc.

### Adding Chapters

1. Create a new `.tex` file for each chapter following the pattern of existing chapter files.
2. Include the new chapter in `thesis-main.tex` using the `\input{chapter-name.tex}` command.

### Adding Figures

1. Place your figure files in the `figures/` directory.
2. Reference them in your documents using the standard LaTeX figure environment:

```latex
\begin{figure}[htbp]
    \centering
    \includegraphics[width=0.8\textwidth]{figures/your-image-file}
    \caption{Your figure caption}
    \label{fig:your-reference-label}
\end{figure}
```

## 🔄 Compilation

To compile your thesis, follow these steps:

### Using Command Line

For a complete build with references and citations:

```bash
pdflatex thesis-main
bibtex thesis-main
pdflatex thesis-main
pdflatex thesis-main
```

Running pdflatex multiple times ensures that all references, citations, and table of contents are properly updated.

### Using an Editor

Most LaTeX editors provide one-click compilation options:

- In **TeXstudio**: Open `thesis-main.tex` and click the "Build & View" button.
- In **VS Code with LaTeX Workshop**: Open `thesis-main.tex` and use the build commands (typically Ctrl+Alt+B).
- In **Overleaf**: The compilation happens automatically.

## ⚙️ Customization

### Thesis Information

Edit the beginning of `thesis-main.tex` to update:
- Thesis title
- Author name
- Department/Institution
- Date/Year
- Degree information

### Page Layout and Formatting

Modify `preamble.tex` to change:
- Margins and page geometry
- Font styles and sizes
- Header and footer configuration
- Line spacing

### Citation Style

The template uses the `natbib` package for references. You can change the citation style by modifying the bibliography style in `thesis-main.tex`.

## 📚 Tips and Best Practices

- **Version Control**: Commit regularly to track changes to your thesis.
- **Backup**: Regularly backup your work to cloud storage or an external drive.
- **Modular Writing**: Write each chapter in a separate file for better organization.
- **Comments**: Use LaTeX comments (`%`) to leave notes for yourself.
- **Draft Mode**: Use the `draft` option in the document class for faster compilation during writing.

## 📄 License

This template is available under the MIT License - feel free to modify and use it for your academic work.

## 🤝 Contributing

Contributions to improve this template are welcome. Please feel free to submit a pull request or open an issue.

---

Good luck with your thesis! 📚✨

