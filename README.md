# IST LaTeX Report Template

A simple LaTeX template for [Instituto Superior Técnico](https://tecnico.ulisboa.pt/) course and lab reports.



## Layout

```
.
├── appendices/
│   ├── 01-first.tex
│   └── 02-second.tex
├── front/
│   ├── cover.tex
│   └── lists.tex
├── sections/
│   ├── 01-intro.tex
│   ├── 02-problem.tex
│   ├── 03-solution.tex
│   └── 04-conclusion.tex
├── Images/
├── main.tex
└── refs.bib
```

To add a section, create a file into `sections/` and add one `\input{sections/nn-name}` line.



## Requirements

`latexmk` from TeX Live, MacTeX or TinyTeX. Every package in the preamble ships with a current TeX Live, so a normal install is enough.



## Compiling

From the project root:

```bash
latexmk -pdf main.tex
```

Continuous mode, rebuilds on every save:
```bash
latexmk -pdf -pvc main.tex
```  

remove all build artifacts:
```bash
latexmk -C
```

With the LaTeX Workshop extension installed, ctrl+S builds it automatically.



## Credits

Inspired by:

- [themiguelamador/ThesisIST](https://github.com/themiguelamador/ThesisIST)
- [samfcmc/ist-dissertation-latex-template](https://github.com/samfcmc/ist-dissertation-latex-template)
- [Report Template IST (EN) on Overleaf](https://it.overleaf.com/latex/templates/report-template-ist-en/jvjdsvbtcbpn)
