![CV and Resume](demo-preview.png)

# isosafrasaurus's CV template

This is a simple LaTeX .sty file to help format CVs. Although there is only one command and one environment, they can be combined with native LaTeX features in many ways to create a versatile range of CVs. Two examples are provided.

## Dependencies

This package relies on the following standard LaTeX packages:

  * `url`
  * `titlesec`
  * `paracol`
  * `xkeyval`
  * `ifthen`
  * `enumitem`

## Installation

1.  Download `cv.sty` from this repository.
2.  Place it in the same directory as your `.tex` file (or in your local TeX tree).
3.  Load the package in your document preamble:

<!-- end list -->

```latex
\usepackage{cv}
```

## Usage

### `\entry` Command

Used for standard CV items. It accepts up to four header fields and a description body.

```latex
\entry[
    title         = {...}, % Main title (Left)
    righttitle    = {...}, % Dates (Right)
    subtitle      = {...}, % Organization (Left)
    rightsubtitle = {...}, % Location (Right)
    description   = {...}  % Body text or bullet points
]
```

### `stacked` Environment

Used to group multiple `\entry` items together under a single main header. This renders a vertical bar on the left margin to visually connect the entries.

```latex
\begin{stacked}[title={Organization Name}, subtitle={Location}]
    \entry[title={New Role}, righttitle={2023--Present}, description={...}]
    \entry[title={Previous Role}, righttitle={2020--2023}, description={...}]
\end{stacked}
```
