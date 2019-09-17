---
title: Report for simulation run on {{date}}
author: Benjamin Rüth
header-includes: |
    \usepackage{booktabs}
abstract: ---
---

## Input parameters

\begin{itemize}
\item $\alpha = {{alpha}}$
\item $\beta = {{beta}}$
\item $\gamma = {{gamma}}$
\item \texttt{-mth = {{method}}}
\item \texttt{-exec = {{executable}}}
\item \texttt{-t = {{time_dependence}}}
\item \texttt{-wri = {{waveform_interpolation_strategy}}}
\item \texttt{-ctol = {{coupling_tolerance}}}
\item \texttt{-stol = {{solver_tolerance}}}
\end{itemize}

## Manufactured Solution

\begin{equation*}
u_\text{exact} = {{manufactured_solution}}
\end{equation*}

## Source Code

\begin{itemize}
\item \texttt{tutorials: {{tutorials_hash}}}
\item \texttt{fenics-adapter: {{adapter_hash}}}
\item \texttt{waveform-bindings: {{waveform_bindings_hash}}}
\item \texttt{precice: {{precice_hash}}}
\end{itemize}

\begin{table}
\centering
{{qn_table}}
\caption{QN Iterations}
\end{table}

\begin{table}
\centering
{{error_table}}
\caption{Errors}
\end{table}