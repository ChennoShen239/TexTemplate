# LaTeX Templates for Mathematical Notes and Homework

A comprehensive collection of LaTeX templates designed for mathematical notes, homework assignments, and academic writing, with a focus on Analysis and Advanced Mathematics. Features beautiful theorem-like environments with consistent styling and colors.

## Acknowledgment

This template is forked from [BrandonPacewic/LaTexTemplates](https://github.com/BrandonPacewic/LaTexTemplates). Special thanks to Brandon Pacewic for creating the original template that served as the foundation for this work.

## Overview

These templates were created for MATH 104 (Introduction to Analysis) at UC Berkeley. The collection includes:

1. **Notes Template** (`template.tex`): A comprehensive template for taking detailed course notes
2. **Homework Template** (`homework.tex`): A clean, professional template for homework submissions

## Features

### Common Features (Both Templates)
- **Beautiful Theorem Environments**: Color-coded environments for different types of content:
  - Theorems (Blue) - For important mathematical statements and proofs
  - Examples (Green) - For illustrative examples
  - Definitions (Violet) - For formal mathematical definitions
  - Exercises (Teal) - For practice problems
  - Notes (Orange) - For additional insights
  - Problems (Red) - For challenging problems
  - Solutions (Light Blue) - For detailed solutions

### Notes Template Features
- Clean and professional layout with consistent spacing
- Table of contents for easy navigation
- Advanced mathematical typesetting support
- Graph drawing capabilities with TikZ
- Algorithm writing support

### Homework Template Features
- Professional header with course info and student details
- Page numbers in footer
- Compact and clean design
- Focus on problem-solution format

## Example Usage

### Notes Template
```latex
\begin{Definition}{Limit of a Function}{def:limit}
    For a function $f(x)$, we say $\lim_{x \to a} f(x) = L$ if for every $\epsilon > 0$, 
    there exists a $\delta > 0$ such that:
    \[0 < |x - a| < \delta \implies |f(x) - L| < \epsilon\]
\end{Definition}
```

### Homework Template
```latex
% Header setup
\usepackage{fancyhdr}
\pagestyle{fancy}
\fancyhf{} % Clear default headers/footers
\renewcommand{\headrulewidth}{0.4pt}

% Left header: Course info and homework number
\lhead{MATH 104 - Analysis \\ Homework 1}
% Right header: Name and date
\rhead{Your Name \\ Due: Date}
% Center footer: Page number
\cfoot{\thepage}
```

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/ChennoShen239/TexTemplate.git
   ```

2. Copy the template files to your working directory:
   ```bash
   cp template/* your/working/directory/
   ```

3. Choose the appropriate template:
   - For course notes: Use `template.tex`
   - For homework: Use `homework.tex`

## Required Packages

The templates use several LaTeX packages. Most are included in standard LaTeX distributions like TeX Live. Key packages include:
- amsmath, amsfonts, amsthm, amssymb
- tcolorbox (for beautiful theorem environments)
- tikz, pgfplots (for graphs and diagrams)
- hyperref (for cross-referencing)
- algorithm2e (for algorithms)
- fancyhdr (for homework template headers)

## License

This template is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
