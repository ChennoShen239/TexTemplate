# LaTeX Template for Mathematical Notes

A comprehensive LaTeX template designed for mathematical notes, proofs, and academic writing. Features beautiful theorem-like environments with consistent styling and colors.

## Features

- **Clean and Professional Design**: Carefully crafted layout with consistent spacing and margins
- **Beautiful Theorem Environments**: Color-coded environments for different types of content:
  - Theorems (Blue)
  - Examples (Green)
  - Definitions (Violet)
  - Exercises (Teal)
  - Notes (Orange)
  - Problems (Red)
  - Solutions (Light Blue)
- **Advanced Mathematical Support**: Full support for mathematical symbols, equations, and diagrams
- **Cross-referencing**: Built-in support for references and hyperlinks
- **Algorithm Support**: Environment for writing algorithms with proper formatting
- **Graph Drawing**: TikZ and pgfplots integration for creating mathematical graphs

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/cheney_gao/TexTemplates.git
   ```

2. Copy the template files to your working directory:
   ```bash
   cp template/* your/working/directory/
   ```

3. Rename template.tex to your desired filename:
   ```bash
   mv template.tex your_file.tex
   ```

## Usage

The template consists of two main files:
- `template.tex`: The main document where you write your content
- `preamble.tex`: Contains all package imports and environment definitions

### Theorem-like Environments

```latex
\begin{Definition}{Title}{label}
    Your definition here...
\end{Definition}

\begin{Theorem}{Title}{label}
    Your theorem here...
\end{Theorem}

\begin{Example}{Title}{label}
    Your example here...
\end{Example}

\begin{Exercise}{Title}{label}
    Your exercise here...
\end{Exercise}

\begin{Problem}{Title}{label}
    Your problem here...
\end{Problem}

\begin{solution}
    Your solution here...
\end{solution}

\begin{note}
    Your note here...
\end{note}
```

### Mathematical Features

- Full AMS-Math support
- Custom mathematical operators
- Equation numbering and referencing
- Matrix and array environments
- Commutative diagrams (tikz-cd)

### Graphing Support

```latex
\begin{tikzpicture}
    \begin{axis}[
        xlabel={$x$},
        ylabel={$y$}
    ]
    \addplot[color=blue] {x^2};
    \end{axis}
\end{tikzpicture}
```

## Required Packages

The template uses several LaTeX packages. Most are included in standard LaTeX distributions like TeX Live. Key packages include:
- amsmath, amsfonts, amsthm, amssymb
- tcolorbox
- tikz, pgfplots
- hyperref
- algorithm2e

## License

This template is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to submit issues and enhancement requests!
