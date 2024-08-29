---
title: Math Expression
parent: Plugins
nav_order: 6
---

# Math Expression (`math`)


Use this plugin to quickly paste math expressions as PNG, SVG, or even Unicode! This can come in handy when preparing slides or writing emails.

<img src="{{ "/assets/images/Plugin_Math.png" | prepend: site.baseurl | prepend: site.url}}"/>

Click on the `Options` slider below the math preview to access various quick settings.

To use the `pdflatex` processing option, please make sure you have `pdflatex` installed and added to your path.

The following options are available:

- Input Type
  - LaTeX Math: `f(x)=x^2, f:\mathbb{R}\mapsto\mathbb{R}`
  - AsciiMath: `f(x)=x^2, f: RR |-> RR`
- Processing Method
  - [MathJax](https://www.mathjax.org/)
  - [PdfLatex](https://miktex.org/download)
- Output Type
  - PNG
  - SVG
  - Unicode
- Font Size (important for resolution)
- Resolution (% of pixels per pasted image height, relevant only for pixel graphic output)
- Paste Color
- Display Style

AsciiMath is an easy-to-write markup language, that allows you to write math expressions more effortlessly in comparison to Latex math expressions. You can read up on it [on the official website](https://asciimath.org/). There is a custom implementation for the transformation of AsciiMath to latex when using it in combination with unicode as output. This implementation is based on the specification [on the official website](https://asciimath.org/). In the following, there is an overview of all symbols:

Here are the grouped symbols with the LaTeX commands escaped so that the LaTeX code is visible.

### Greek Letters

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| alpha           | `\alpha`            | α                 |
| beta            | `\beta`             | β                 |
| gamma           | `\gamma`            | γ                 |
| delta           | `\delta`            | δ                 |
| epsilon         | `\epsilon`          | ε                 |
| zeta            | `\zeta`             | ζ                 |
| theta           | `\theta`            | θ                 |
| iota            | `\iota`             | ι                 |
| kappa           | `\kappa`            | κ                 |
| lambda          | `\lambda`           | λ                 |
| mu              | `\mu`               | μ                 |
| nu              | `\nu`               | ν                 |
| xi              | `\xi`               | ξ                 |
| pi              | `\pi`               | π                 |
| rho             | `\rho`              | ρ                 |
| sigma           | `\sigma`            | σ                 |
| tau             | `\tau`              | τ                 |
| upsilon         | `\upsilon`          | υ                 |
| phi             | `\phi`              | φ                 |
| chi             | `\chi`              | χ                 |
| psi             | `\psi`              | ψ                 |
| omega           | `\omega`            | ω                 |
| Gamma           | `\Gamma`            | Γ                 |
| Delta           | `\Delta`            | Δ                 |
| Theta           | `\Theta`            | Θ                 |
| Lambda          | `\Lambda`           | Λ                 |
| Xi              | `\Xi`               | Ξ                 |
| Pi              | `\Pi`               | Π                 |
| Sigma           | `\Sigma`            | Σ                 |
| Upsilon         | `\Upsilon`          | Υ                 |
| Phi             | `\Phi`              | Φ                 |
| Psi             | `\Psi`              | Ψ                 |
| Omega           | `\Omega`            | Ω                 |

### Basic Operations and Relations

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| <=              | `\leq`              | ≤                 |
| >=              | `\geq`              | ≥                 |
| !=              | `\neq`              | ≠                 |
| ===             | `\equiv`            | ≡                 |
| or              | `\or`               | ∨                 |
| not             | `\neg`              | ¬                 |
| implies         | `\Rightarrow`       | ⇒                 |
| iff             | `\Leftrightarrow`   | ⇔                 |

### Functions

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| sqrt            | `\sqrt`             | √                 |
| frac            | `\frac`             | ⅟                 |
| sin             | `\sin`              | sin               |
| cos             | `\cos`              | cos               |
| tan             | `\tan`              | tan               |
| log             | `\log`              | log               |
| ln              | `\ln`               | ln                |
| exp             | `\exp`              | exp               |

### Sums and Products

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| sum             | `\sum`              | ∑                 |
| prod            | `\prod`             | ∏                 |
| int             | `\int`              | ∫                 |
| oint            | `\oint`             | ∮                 |

### Other Symbols

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| infty           | `\infty`            | ∞                 |
| partial         | `\partial`          | ∂                 |
| nabla           | `\nabla`            | ∇                 |
| cdot            | `\cdot`             | ⋅                 |
| times           | `\times`            | ×                 |
| div             | `\div`              | ÷                 |
| mod             | `\mod`              | mod               |
| perp            | `\perp`             | ⊥                 |
| parallel        | `\parallel`         | ∥                 |
| angle           | `\angle`            | ∠                 |
| triangle        | `\triangle`         | △                 |
| degree          | `^{\circ}`          | °                 |

Here are the missing tables grouped by category:

### Superscripts and Subscripts

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| `x^2`           | `x^{2}`             | ²                 |
| `x_i`           | `x_{i}`             | x₁                |

### Arrows

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| uarr            | `\uparrow`          | ↑                 |
| darr            | `\downarrow`        | ↓                 |
| rarr            | `\rightarrow`       | →                 |
| larr            | `\leftarrow`        | ←                 |
| harr            | `\leftrightarrow`   | ↔                 |
| rArr            | `\Rightarrow`       | ⇒                 |
| lArr            | `\Leftarrow`        | ⇐                 |
| hArr            | `\Leftrightarrow`   | ⇔                 |
| `|->`           | `\mapsto`           | ↦                 |
| ->              | `\rightarrow`       | →                 |
| <-              | `\leftarrow`        | ←                 |
| =>              | `\Rightarrow`       | ⇒                 |
| <=              | `\leq`              | ≤                 |

### Logical Operators

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| and             | `\land`             | ∧                 |
| or              | `\lor`              | ∨                 |
| not             | `\neg`              | ¬                 |
| if              | `\rightarrow`       | →                 |
| <=>             | `\Leftrightarrow`   | ⇔                 |

### Sets

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| in              | `\in`               | ∈                 |
| ni              | `\ni`               | ∋                 |
| subset          | `\subset`           | ⊂                 |
| supset          | `\supset`           | ⊃                 |
| subseteq        | `\subseteq`         | ⊆                 |
| supseteq        | `\supseteq`         | ⊇                 |
| emptyset        | `\emptyset`         | ∅                 |
| cup             | `\cup`              | ∪                 |
| cap             | `\cap`              | ∩                 |
| setminus        | `\setminus`         | ∖                 |
| Union           | `\bigcup`           | ⋃                 |
| Intersect       | `\bigcap`           | ⋂                 |

### Accents

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| hatx            | `\hat{x}`           | ẍ                 |
| barx            | `\overline{x}`      | x̅                 |
| vecx            | `\vec{x}`           | x⃗                 |
| tildex          | `\tilde{x}`         | ẋ                 |
| dotx            | `\dot{x}`           | ẋ                 |
| ddotx           | `\ddot{x}`          | ẍ                 |

### Font Commands

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| bb "ABC"        | `\mathbb{ABC}`      | 𝔸𝔹ℂ              |
| bf "ABC"        | `\mathbf{ABC}`      | 𝐀𝐁𝐂              |
| it "ABC"        | `\mathit{ABC}`      | 𝑨𝑩𝑪              |
| sf "ABC"        | `\mathsf{ABC}`      | 𝖠𝖡𝖢              |
| tt "ABC"        | `\mathtt{ABC}`      | 𝚨𝚩𝚪              |
| fr "ABC"        | `\mathfrak{ABC}`    | 𝔄𝔅ℭ              |
| cc "ABC"        | `\mathcal{ABC}`     | 𝒜ℬ𝒞              |

### Basic Arithmetic Operators

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| +               | `+`                 | +                 |
| -               | `-`                 | -                 |
| ***             | `\star`             | ⋆                 |
| **              | `\ast`              | ∗                 |
| *               | `\cdot`             | ⋅                 |

### Special Symbols

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| xx              | `\times`            | ×                 |
| -:              | `\div`              | ÷                 |
| :               | `\colon`            | :                 |
| o+              | `\oplus`            | ⊕                 |
| ox              | `\otimes`           | ⊗                 |
| o.              | `\odot`             | ⊙                 |
| ^^              | `\wedge`            | ∧                 |
| ^^^             | `\bigwedge`         | ⋀                 |
| vvv             | `\bigvee`           | ⋁                 |
| vv              | `\vee`              | ∨                 |
| nnn             | `\bigcap`           | ⋂                 |
| nn              | `\cap`              | ∩                 |
| uuu             | `\bigcup`           | ⋃                 |
| uu              | `\cup`              | ∪                 |

### Comparison Operators

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| !=              | `\neq`              | ≠                 |
| <=              | `\leq`              | ≤                 |
| >=              | `\geq`              | ≥                 |
| ~=              | `\approx`           | ≈                 |
| ~~~             | `\approx`           | ≈                 |
| prop            | `\propto`           | ∝                 |

### Set Membership

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| -<=             | `\subset`           | ⊂                 |
| -<>             | `\subsetneq`        | ⊊                 |
| >-=             | `\supset`           | ⊃                 |
| >-<             | `\supsetneq`        | ⊋                 |
| !in             | `\notin`            | ∉                 |

### Ellipses

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| ...             | `\ldots`            | …                 |
| |cdots|         | `\cdots`            | ⋯                 |
| vdots           | `\vdots`            | ⋮                 |
| ddots           | `\ddots`            | ⋱                 |

### Geometric Shapes

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| diamond         | `\diamond`          | ◊                 |
| square          | `\square`           | □                 |
| \|__ __\|       | `\parallel`         | ∥                 |
| \|~ ~\|         | `\sim`              | ∼                 |

### Set Symbols

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| CC              | `\mathbb{C}`        | ℂ                 |
| NN              | `\mathbb{N}`        | ℕ                 |
| QQ              | `\mathbb{Q}`        | ℚ                 |
| RR              | `\mathbb{R}`        | ℝ                 |
| ZZ              | `\mathbb{Z}`        | ℤ                 |

### Quantifiers and Logical Symbols

| AsciiMath Input | LaTeX Output        | Unicode Character |
|-----------------|---------------------|-------------------|
| AA              | `\forall`           | ∀                 |
| forall          | `\forall`           | ∀                 |
| EE              | `\exists`           | ∃                 |
| exists          | `\exists`           | ∃                 |
| _\|_            | `\bot`              | ⊥                 |
| TT              | `\top`              | ⊤                 |
| \|--            | `\vdash`            | ⊢                 |
| \|==            | `\models`           | ⊨                 |

