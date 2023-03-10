---
title: "Pressure"
subtitle: Relating temperature and pressure
author: "Sofia Russo"
date: "Università degli Studi di Padova"
output:
  pdf_document:
    number_sections: yes
    toc: yes
    toc_depth: 3
linestretch: 1.5
geometry: margin=1in
bibliography: bibliography/biblio_SECOND.bib
---



# DATASET
<!-- prova -->
## Variable: pressure 
*Prova* **prova** ***blablabla*** \textcolor{red}{prova} \color{red}\Huge blablabla \normalsize \normalcolor prova \Huge blablabla \normalsize  @epifania2021implicit

>Prova prova blablabla Prova prova blablabla  

- Prova 
- prova 
    1. Papappero 
        1. Pappararra
- blablabla 

1. Prova 
2. prova 
7. blablabla 

### Inspection 
Prova prova blablabla Prova prova blablabla Prova prova blablabla Prova prova blablabla Prova prova blablabla Prova prova blablabla Prova prova blablabla Prova prova blablabla Prova prova blablabla 

- Prova
    - Mannaggia
        - Aaaaaa
    - Mannaggia
- Prova    

Con i piedi[^1]

[^1]: ciao ciao

Con le mani [^2]

[^2]: ciao

#### What is relevant to note: nothing 

prova \color{blue}[Link](https://poterealpopolo.org/)\normalcolor

#### Oh well whatever: nevermind 

\color{blue}[![cieli](images/blues.png)](https://it.wikipedia.org/wiki/Cielo)\normalcolor
![cieli](images/blues.png) 


```r
knitr::include_graphics(path = "images/earth_core.jpeg")
```

\begin{figure}

\hfill{}\includegraphics[width=0.1\linewidth]{images/earth_core} 

\caption{Caption}\label{fig:unnamed-chunk-1}
\end{figure}

<!-- Porva bibliografia @epifania2020dscoreapp  -->


```
lol   temperature pressure
lol 1           0   0.0002
lol 2          20   0.0012
lol 3          40   0.0060
lol 4          60   0.0300
lol 5          80   0.0900
lol 6         100   0.2700
```
Questo è il dataset: 

```
lol     Min.  1st Qu.   Median     Mean  3rd Qu.     Max. 
lol   0.0002   0.1800   8.8000 124.3367 126.5000 806.0000
```


```r
data
```

```
nonlol    temperature pressure   y        x
nonlol 1            0   0.0002   0   0.0002
nonlol 2           20   0.0012  20   0.0012
nonlol 3           40   0.0060  40   0.0060
....
```

e questo è il plot grezzi:

\begin{center}\includegraphics{Prova_knit_files/figure-latex/unnamed-chunk-5-1} \end{center}

mentre questo è la regressione applicata, con codice e risultati: 

```r
# regressione
m = lm(y ~ x, data = data)
# summary del modello
summary(m)
```

```
lol 
lol Call:
lol lm(formula = y ~ x, data = data)
lol 
lol Residuals:
lol      Min       1Q   Median       3Q      Max 
lol -132.791  -62.813    6.507   67.033   90.759 
lol 
lol Coefficients:
lol              Estimate Std. Error t value Pr(>|t|)    
lol (Intercept) 132.79072   19.94314   6.658 4.03e-06 ***
lol x             0.37969    0.07929   4.788 0.000171 ***
lol ---
lol Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
lol 
lol Residual standard error: 75.56 on 17 degrees of freedom
lol Multiple R-squared:  0.5742,	Adjusted R-squared:  0.5492 
lol F-statistic: 22.93 on 1 and 17 DF,  p-value: 0.000171
```


\begin{table}[!htbp] \centering 
  \caption{Tabella di summary} 
  \label{} 
\begin{tabular}{@{\extracolsep{5pt}}lccccc} 
\\[-1.8ex]\hline 
\hline \\[-1.8ex] 
Statistic & \multicolumn{1}{c}{N} & \multicolumn{1}{c}{Mean} & \multicolumn{1}{c}{St. Dev.} & \multicolumn{1}{c}{Min} & \multicolumn{1}{c}{Max} \\ 
\hline \\[-1.8ex] 
temperature & 19 & 180.00 & 112.55 & 0 & 360 \\ 
pressure & 19 & 124.34 & 224.62 & 0.0002 & 806.00 \\ 
y & 19 & 180.00 & 112.55 & 0 & 360 \\ 
x & 19 & 124.34 & 224.62 & 0.0002 & 806.00 \\ 
\hline \\[-1.8ex] 
\end{tabular} 
\end{table} 

\begin{table}[!htbp] \centering 
  \caption{Risultati del modello} 
  \label{} 
\begin{tabular}{@{\extracolsep{5pt}}lc} 
\\[-1.8ex]\hline 
\hline \\[-1.8ex] 
 & \multicolumn{1}{c}{\textit{Dependent variable:}} \\ 
\cline{2-2} 
\\[-1.8ex] & y \\ 
\hline \\[-1.8ex] 
 x & 0.38$^{***}$ \\ 
  & (0.08) \\ 
  & \\ 
 Constant & 132.79$^{***}$ \\ 
  & (19.94) \\ 
  & \\ 
\hline \\[-1.8ex] 
Observations & 19 \\ 
R$^{2}$ & 0.57 \\ 
Adjusted R$^{2}$ & 0.55 \\ 
Residual Std. Error & 75.56 (df = 17) \\ 
F Statistic & 22.93$^{***}$ (df = 1; 17) \\ 
\hline 
\hline \\[-1.8ex] 
\textit{Note:}  & \multicolumn{1}{r}{$^{*}$p$<$0.1; $^{**}$p$<$0.05; $^{***}$p$<$0.01} \\ 
\end{tabular} 
\end{table} 





\begin{table}[!htbp] \centering 
\begin{tabular}{@{\extracolsep{5pt}}lcc} 
\\[-1.8ex]\hline 
\hline \\[-1.8ex] 
 & \multicolumn{2}{c}{\textit{Dependent variable:}} \\ 
\cline{2-3} 
\\[-1.8ex] & \multicolumn{2}{c}{temperature} \\ 
\\[-1.8ex] & (1) & (2)\\ 
\hline \\[-1.8ex] 
 Constant & 180.00$^{***}$ & 132.79$^{***}$ \\ 
  & (25.82) & (19.94) \\ 
  & & \\ 
 pressure &  & 0.38$^{***}$ \\ 
  &  & (0.08) \\ 
  & & \\ 
\hline \\[-1.8ex] 
Observations & 19 & 19 \\ 
R$^{2}$ & 0.00 & 0.57 \\ 
Adjusted R$^{2}$ & 0.00 & 0.55 \\ 
Residual Std. Error & 112.55 (df = 18) & 75.56 (df = 17) \\ 
F Statistic &  & 22.93$^{***}$ (df = 1; 17) \\ 
\hline 
\hline \\[-1.8ex] 
\textit{Note:}  & \multicolumn{2}{r}{$^{*}$p$<$0.1; $^{**}$p$<$0.05; $^{***}$p$<$0.01} \\ 
\end{tabular} 
  \caption{Model comparison} 
  \label{} 
\end{table}  

Formule 



$z = \frac{x_i - \bar{X}}{sd} = \frac{\ensuremath{2\times 10^{-4}}- 124.3367053}{224.6225399 } = -0.5533362$ 


```r
x = data$pressure
y = data$temperature
```


$ y = \left(\frac{a}{b})\right ^2$ 

<!-- $ a = \left(\frac {\ensuremath{2\times 10^{-4}}, 0.0012, 0.006, 0.03, 0.09, 0.27, 0.75, 1.85, 4.2, 8.8, 17.3, 32.1, 57, 96, 157, 247, 376, 558, 806}{0, 20, 40, 60, 80, 100, 120, 140, 160, 180, 200, 220, 240, 260, 280, 300, 320, 340, 360} \ right)^2 = \ensuremath{\infty{}}, \ensuremath{3.6\times 10^{-9}}, \ensuremath{2.25\times 10^{-8}}, \ensuremath{2.5\times 10^{-7}}, \ensuremath{1.265625\times 10^{-6}}, \ensuremath{7.29\times 10^{-6}}, \ensuremath{3.90625\times 10^{-5}}, \ensuremath{1.7461735\times 10^{-4}}, \ensuremath{6.890625\times 10^{-4}}, 0.0023901, 0.0074823, 0.0212895, 0.0564062, 0.1363314, 0.3144005, 0.6778778, 1.380625, 2.6934602, 5.0126235$ -->
