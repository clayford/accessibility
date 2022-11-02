# Notes on creating accessible R Markdown/Quarto Documents 

From [https://r-resources.massey.ac.nz/rmarkdown/](https://r-resources.massey.ac.nz/rmarkdown/)

- Provide the original source files as well as the final HTML documents you create
- HTML is more accessible than PDF
- Use proper heading styles
- Use tables for tabulation, not presentation/layout
- Use the standard LaTeX style method for inserting mathematical content, but enter simple mathematical elements as text (such x, y, etc)
- Use parentheses, `()`, after function names 
- Get rid of hash/number signs in R output: `opts_chunk$set(comment="")`
- Label all graphics with alt text tags. Use `fig.cap` in figure chunk headers. Examples:

````
```{r fig.cap="describe the plot", fig.align='center'}
plot(x, y)
```
````


````
```{r, fig.cap="alt text"}
knitr::include_graphics('figures/my_image.png')
```
````

See also: https://jacob-gg.github.io/accessibility-statlab/
