# LaTeX Template for Mathematical Notes

A comprehensive LaTeX template designed for mathematical notes, proofs, and academic writing, with a focus on Analysis and Advanced Mathematics. Features beautiful theorem-like environments with consistent styling and colors.

## Overview

This template was created for MATH 104 (Introduction to Analysis) at UC Berkeley, but it's suitable for any advanced mathematics course. It provides a clean, professional layout with color-coded environments for theorems, definitions, examples, and more.

## Features

- **Clean and Professional Design**: Carefully crafted layout with consistent spacing and margins
- **Beautiful Theorem Environments**: Color-coded environments for different types of content:
  - Theorems (Blue) - For important mathematical statements and proofs
  - Examples (Green) - For illustrative examples (e.g., continuous functions)
  - Definitions (Violet) - For formal mathematical definitions (e.g., limits, vector spaces)
  - Exercises (Teal) - For practice problems (e.g., derivative computations)
  - Notes (Orange) - For additional insights and explanations
  - Problems (Red) - For challenging problems and research questions
  - Solutions (Light Blue) - For detailed solution explanations
- **Advanced Mathematical Support**: Full support for mathematical symbols, equations, and diagrams
- **Cross-referencing**: Built-in support for references and hyperlinks
- **Algorithm Support**: Environment for writing algorithms (e.g., Selection Sort)
- **Graph Drawing**: TikZ and pgfplots integration for creating mathematical graphs

## Example Usage

### Course Information
```latex
\title{Introduction to Analysis}
\author{Chen Gao}
\date{Spring 2025}

\begin{center}
\begin{tabular}{ll}
\textbf{Course:} & MATH 104 \\
\textbf{Institution:} & University of California, Berkeley \\
\textbf{Semester:} & Spring 2025
\end{tabular}
\end{center}
```

### Theorem-like Environments

```latex
\begin{Definition}{Limit of a Function}{def:limit}
    For a function $f(x)$, we say $\lim_{x \to a} f(x) = L$ if for every $\epsilon > 0$, 
    there exists a $\delta > 0$ such that:
    \[0 < |x - a| < \delta \implies |f(x) - L| < \epsilon\]
\end{Definition}

\begin{Theorem}{Limit Laws}{thm:limit-laws}
    If $\lim_{x \to a} f(x) = L$ and $\lim_{x \to a} g(x) = M$, then:
    \begin{enumerate}
        \item $\lim_{x \to a} [f(x) + g(x)] = L + M$
        \item $\lim_{x \to a} [f(x) \cdot g(x)] = L \cdot M$
        \item $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{L}{M}$, if $M \neq 0$
    \end{enumerate}
\end{Theorem}

\begin{Example}{Continuous Function}{ex:continuous}
    Consider $f(x) = x^2$. This function is continuous at every point $x \in \mathbb{R}$ because:
    \[\lim_{h \to 0} [f(x+h) - f(x)] = \lim_{h \to 0} [(x+h)^2 - x^2] = 0\]
\end{Example}
```

### Mathematical Features

The template includes support for:
- Advanced equation formatting and alignment
- Matrix and vector operations
- Commutative diagrams
- Custom mathematical operators
- Automatic equation numbering and referencing

### Graphing Support

```latex
\begin{figure}[ht]
    \centering
    \begin{tikzpicture}
        \begin{axis}[
            xlabel={$x$},
            ylabel={$f(x)$},
            title={Quadratic Function $f(x) = x^2 - 2x + 1$},
            grid=major
        ]
        \addplot[color=blue,mark=*,smooth] {x^2 - 2*x + 1};
        \end{axis}
    \end{tikzpicture}
\end{figure}
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

3. Rename template.tex to your desired filename:
   ```bash
   mv template.tex your_file.tex
   ```

## Required Packages

The template uses several LaTeX packages. Most are included in standard LaTeX distributions like TeX Live. Key packages include:
- amsmath, amsfonts, amsthm, amssymb
- tcolorbox (for beautiful theorem environments)
- tikz, pgfplots (for graphs and diagrams)
- hyperref (for cross-referencing)
- algorithm2e (for algorithms)

## License

This template is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to submit issues and enhancement requests! This template is actively used for mathematics courses at UC Berkeley and is continuously being improved.
