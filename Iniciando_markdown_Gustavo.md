---
title: "markdown"
author: "Gustavo Jun Yakushiji"
date: ''
header-includes:
   - \usepackage[portuguese]{babel}
output:
  word_document: 
    fig_caption: yes
    highlight: espresso
    keep_md: yes
    toc: yes
  html_document:
    fontsize: 12pt
    number_sections: yes
    toc: yes
  pdf_document: 
    fig_caption: yes
    highlight: espresso
    keep_tex: yes
    number_sections: yes
    toc: yes
linestretch: 1
geometry: left=3cm, right=3cm, top=2.5cm, bottom=2.5cm
bibliography: referencias.bib
---



# Titulo
No penúltimo jogo da Copa América de 2020, a Colômbia venceu o Peru de virada por 3 a 2 em Brasília nesta sexta-feira e ficou com o terceiro lugar na classificação geral da competição.

O Peru abriu o placar aos 45 minutos do primeiro tempo com Yotun. Na etapa final, a Colômbia virou com Cuadrado aos 4 minutos e Luis Diáz aos 21 da etapa final. Aos 37 do segundo tempo, Lapadula, de cabeça, empatou o confronto para os peruanos.


## Titulo
No penúltimo jogo da Copa América de 2020, a Colômbia venceu o Peru de virada por 3 a 2 em Brasília nesta sexta-feira e ficou com o terceiro lugar na classificação geral da competição.

O Peru abriu o placar aos 45 minutos do primeiro tempo com Yotun. Na etapa final, a Colômbia virou com Cuadrado aos 4 minutos e Luis Diáz aos 21 da etapa final. Aos 37 do segundo tempo, Lapadula, de cabeça, empatou o confronto para os peruanos.

### Titulo
No penúltimo jogo da Copa América de 2020, a Colômbia venceu o Peru de virada por 3 a 2 em Brasília nesta sexta-feira e ficou com o terceiro lugar na classificação geral da competição.

O Peru abriu o placar aos 45 minutos do primeiro tempo com Yotun. Na etapa final, a Colômbia virou com Cuadrado aos 4 minutos e Luis Diáz aos 21 da etapa final. Aos 37 do segundo tempo, Lapadula, de cabeça, empatou o confronto para os peruanos.


```r
summary(pressure)
```

```
##   temperature     pressure       
##  Min.   :  0   Min.   :  0.0002  
##  1st Qu.: 90   1st Qu.:  0.1800  
##  Median :180   Median :  8.8000  
##  Mean   :180   Mean   :124.3367  
##  3rd Qu.:270   3rd Qu.:126.5000  
##  Max.   :360   Max.   :806.0000
```


![Knitr logo](knit_logo.png)

## Fórmulas

Veja $f(x)=x^2$

A seguir um gráfico de dispersão dos nossos dados...(Veja Figura \ref{scatterplot})


```r
plot(Ozone~Wind, data=airquality, pch=20, 
     col="darkorange", lwd=3)
```

![\label{scatterplot}Titulo do meu gráfico](Iniciando_markdown_Gustavo_files/figure-docx/unnamed-chunk-3-1.png)

A seguir o ajuste do modelo usando o \textcolor{red}{software R}


```r
ajuste<- lm(Ozone~Wind, data=airquality)
teta<- round(coef(ajuste),3)
betaS<- round(coef(summary(ajuste)),3)
knitr::kable(betaS, caption = "\\label{tabelajuste}
             Ajuste de um ML para os dados airquality")
```



Table: \label{tabelajuste}
             Ajuste de um ML para os dados airquality

|            | Estimate| Std. Error| t value| Pr(>&#124;t&#124;)|
|:-----------|--------:|----------:|-------:|------------------:|
|(Intercept) |   96.873|      7.239|  13.383|                  0|
|Wind        |   -5.551|      0.690|  -8.040|                  0|

O modelo ajustado foi $\widehat{\text{Ozone}}_i=$ 96.873 -5.551 $\text{Wind}_i$ (Veja Tabela  \ref{tabelajuste})


```r
citation("ggplot2")
```

```
## 
## To cite ggplot2 in publications, please use:
## 
##   H. Wickham. ggplot2: Elegant Graphics for Data Analysis.
##   Springer-Verlag New York, 2016.
## 
## A BibTeX entry for LaTeX users is
## 
##   @Book{,
##     author = {Hadley Wickham},
##     title = {ggplot2: Elegant Graphics for Data Analysis},
##     publisher = {Springer-Verlag New York},
##     year = {2016},
##     isbn = {978-3-319-24277-4},
##     url = {https://ggplot2.tidyverse.org},
##   }
```


```r
library(ggplot2)
```


Podemos usar @ggplot2 ou [@ggplot2].  

# Referências
