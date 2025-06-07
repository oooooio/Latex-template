# LaTeX Academic Template

A comprehensive LaTeX template for academic writing, including manuscript preparation, cover letters, and response letters for journal submissions.

## 📁 Project Structure

```
Latex-template/
├── manuscript.tex          # Main manuscript template
├── cover-letter/           # Cover letter templates and examples
│   ├── cover-letter.tex    # Template with placeholders
│   ├── cover-letter-example.tex  # Filled example
│   ├── README.md          # Detailed usage guide
│   └── logo.jpg           # Institution logo
├── response/              # Response to reviewers template
│   └── response.tex
├── elsarticle-harv.bst    # Bibliography style file
└── LICENSE                # GPL v3 License
```

## 🚀 Quick Start

### Prerequisites

- LaTeX distribution (TeX Live 2025 recommended)
- Required packages:
  - `elsarticle` (for Elsevier journals)
  - `amsmath`, `amssymb` (for mathematics)
  - `graphicx` (for figures)
  - `hyperref` (for links)
  - `geometry` (for page layout)
  - `fancyhdr` (for headers/footers)

### Usage

1. **For Manuscript Submission:**
   ```bash
   pdflatex manuscript.tex
   bibtex manuscript
   pdflatex manuscript.tex
   pdflatex manuscript.tex
   ```

2. **For Cover Letter:**
   ```bash
   cd cover-letter/
   pdflatex cover-letter.tex
   ```

3. **For Response to Reviewers:**
   ```bash
   cd response/
   pdflatex response.tex
   ```

## 📝 Template Features

### Manuscript Template (`manuscript.tex`)
- **Journal:** Nuclear Physics B (easily configurable)
- **Document Class:** `elsarticle` with review option
- **Features:**
  - Author affiliations with labels
  - Abstract and keywords
  - Graphical abstract support
  - Research highlights
  - Line numbering option
  - Bibliography with Harvard style

### Cover Letter Templates (`cover-letter/`)
- **Main Template:** `cover-letter.tex` with comprehensive placeholders
- **Example:** `cover-letter-example.tex` showing completed research submission
- **Font:** Charter for professional appearance
- **Layout:** A4 with 1-inch margins
- **Features:**
  - Institution logo support
  - Professional header/footer design
  - Contact information section
  - Structured content layout with detailed guidance
  - Placeholder system for easy customization
  - Comprehensive usage documentation
- **Customization:** All bracketed placeholders `[PLACEHOLDER]` need replacement
- **Documentation:** Detailed `README.md` with step-by-step instructions

### Response Template (`response/response.tex`)
- **Purpose:** Structured response to peer reviewers
- **Features:**
  - Color-coded responses (red for modifications)
  - Numbered reviewer comments
  - Professional formatting
  - Multiple reviewer support

## 🔬 Example Research Context

The templates include example content for a research paper on:
- **Title:** "Improving Significant Wave Height Prediction Using Chronos Model"
- **Field:** Oceanographic modeling and machine learning
- **Methods:** Transformer-based time series forecasting
- **Data:** NOAA buoy stations with 14-32 years of records

## 📖 Customization Guide

### Manuscript Customization
1. **Journal Selection:** Change `\journal{Nuclear Physics B}` to your target journal
2. **Author Information:** Update author names, affiliations, and contact details
3. **Title and Abstract:** Replace placeholder content
4. **Bibliography:** Use `elsarticle-harv.bst` for Harvard style citations

### Cover Letter Customization
1. **Personal Information:** Replace all `[BRACKETED PLACEHOLDERS]` with your details
2. **Logo:** Replace `logo.jpg` with your institution's logo  
3. **Research Content:** Fill in manuscript title, journal name, and research description
4. **Contributions:** Customize the bullet points with your specific contributions
5. **Optional Sections:** Uncomment editor addressing or preprint information if needed
6. **Detailed Guide:** See `cover-letter/README.md` for comprehensive instructions

**Quick Template Usage:**
- Use `cover-letter.tex` as your working template
- Reference `cover-letter-example.tex` to see how it should look when completed
- Follow the placeholder system: `[YOUR NAME]`, `[YOUR EMAIL]`, etc.

### Response Letter Customization
1. **Journal Reference:** Update manuscript reference number
2. **Reviewer Comments:** Replace example comments with actual feedback
3. **Color Coding:** Use `{\color{red}...}` for highlighting changes
4. **Multiple Reviews:** Add sections for additional reviewers

## 📚 Bibliography Management

The template uses `elsarticle-harv.bst` which provides:
- Harvard-style citations
- DOI and URL support
- arXiv preprint support
- PubMed integration
- Comprehensive journal abbreviations

### Adding References
```latex
\bibliographystyle{elsarticle-harv}
\bibliography{references}
```

## 🛠 Compilation Instructions

### Full Compilation Workflow
```bash
# Compile main document
pdflatex manuscript.tex

# Process bibliography
bibtex manuscript

# Final compilation (run twice for cross-references)
pdflatex manuscript.tex
pdflatex manuscript.tex
```

### Using Latexmk (Recommended)
```bash
latexmk -pdf manuscript.tex
```

## 📋 Checklist for Submission

- [ ] Title and abstract completed
- [ ] All authors and affiliations listed
- [ ] Keywords and research highlights added
- [ ] Figures and tables properly formatted
- [ ] References compiled correctly
- [ ] Cover letter personalized
- [ ] Response to reviewers (if revision)

## 🤝 Contributing

This template is released under GPL v3. Contributions are welcome:
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For issues or questions:
- Check LaTeX documentation for package-specific problems
- Verify all required packages are installed
- Ensure proper compilation order (especially for bibliography)

## 🔗 Useful Links

- [Elsevier Author Guidelines](https://www.elsevier.com/authors/author-schemas/latex-instructions)
- [LaTeX Project](https://www.latex-project.org/)
- [CTAN Package Archive](https://ctan.org/)
- [Overleaf Documentation](https://www.overleaf.com/learn)

---

**Note:** This template includes example content for oceanographic research. Please replace all placeholder content with your actual research details before submission.