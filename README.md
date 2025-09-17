# Useful LaTeX Configs

## Usage
In the beginning of main.tex, do `\input{<documentclass>.tex}`, then `\input{preamble.tex}`.

## Tips 
### algorithm/pseudocode
Example snippet from [Overleaf](https://www.overleaf.com/learn/latex/Algorithms): 

```latex
\begin{algorithm}[hbt!]
    \caption{blah}
    \label{alg:blah}
    \KwData{$n \geq 0$}
    \KwResult{$y = x^n$}
    $y \gets 1$\;
    $X \gets x$\;
    $N \gets n$\;
    \While{$N \neq 0$}{
        \eIf{$N$ is even}{
            $X \gets X \times X$\;
            $N \gets \frac{N}{2} $ \Comment*[r]{This is a comment}
        }{\If{$N$ is odd}{
                $y \gets y \times X$\;
                $N \gets N - 1$\;
            }
        }
    }
\end{algorithm}
```
