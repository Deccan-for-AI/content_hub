# <span style="color:#000000">How to Write an Answer in LaTeX</span>

<video src="${PRIVATE_PREFERENCE_RANKING_VIDEO_2}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

## <span style="color:#364BC9">Key Guidelines (SOUL-Specific)</span>

|            <span style="color:#000000">Functions to be used</span>           |                          <span style="color:#0000009">Examples</span>                          |
| :--------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------: |
|         Use <span style="color:#FF0000">$...$</span> for inline math         |                           <span style="color:#008000">$F = ma$</span>                          |
|        Use <span style="color:#FF0000">$$...$$</span> for display math       |                          <span style="color:#008000">$$F = ma$$</span>                         |
| Use <span style="color:#FF0000">\mathrm{} or \ce{}</span> for chemical names |               <span style="color:#008000">$\mathrm{H\_2O}$ or $\ce{H\_2O}$</span>              |
|  Use <span style="color:#FF0000">\\, \text{kg}</span> for units with spacing |                       <span style="color:#008000">$5\\, \text{kg}$</span>                      |
|              To adjust the brackets to the big fractions inside              |                   <span style="color:#008000">\left(\frac{a}{b}\right)</span>                  |
|                                    Tables                                    | <span style="color:#008000">\begin{array}{\|c\|c\|} \hline x & y \\\ \hline \end{array}</span> |

## <span style="color:#364BC9">Use These Instead of Markdown</span>

| <span style="color:#000000">Markdown</span> |                        <span style="color:#000000">LaTeX Alternative</span>                        |
| :-----------------------------------------: | :------------------------------------------------------------------------------------------------: |
|                 \*\*bold\*\*                |                          <span style="color:#008000">\textbf{bold}</span>                          |
|                   1. item                   |   <span style="color:#008000"> \begin{enumerate}&#xA;\item &#xA;\item &#xA;\end{enumerate}</span>  |
|                    - item                   | <span style="color:#008000">       \begin{itemize}&#xA;\item &#xA;\item &#xA;\end{itemze}  </span> |
|                  # Heading                  |                  <span style="color:#008000">\section{} to \subparagraph{}</span>                  |

