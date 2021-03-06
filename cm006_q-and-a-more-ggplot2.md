---
output:
  html_document:
    toc: true
    toc_depth: 4
---

### cm006 2014-09-22 Monday overview

  * HW01 and associated peer review has been processed; expect feedback in next ~day
  * You've seen and done all the mechanics now: Git(Hub), R Markdown, HW submission, peer review, Discussion, etc.
    - Questions? Comments?
    - FYI: We have our own apps working now, on our own server, so peer marks will be submitted that way from now on (instead of via Google form).
  * Complete our introduction to `ggplot2`
  * What's next?
    - Wed we'll begin data wrangling and aggregation with `dplyr`
    - [HW 3](hw03_???.html) due before class Monday 2014-09-29. It will be making more figures, more sophisticated than last week, and more explorations/summaries of data. Probably Gapminder, though you can ask for approval to use something else. Will cover `ggplot2` and `dplyr`.    
    
#### Slides and links

*there were no slides*

Links about things we talked about during open Q and A

Yes, maybe you will want to make truly interactive, web-native graphs instead of embedding PNGs. Course will probably cover [`ggvis`](http://ggvis.rstudio.com) in second half.

  * [`ggvis`](http://ggvis.rstudio.com): a "pure R/RStudio" solution (though it is most certainly wrapping Javascript; it's just shielding the user from that)
  * [`rCharts`](http://rcharts.io): a package from Ramnath Vaidyanathan providing access to a much richer set of Javascript visualization libraries from R
  * [`d3.js`](http://d3js.org): probably the most powerful, most beautiful way to make web native figures
    - <http://bl.ocks.org/mbostock> just stand back and admire

R Markdown is not the only way to get a pretty report. You can also get one from an __R script__.

  * When editing a `.r` file, RStudio offers a button for this is the spiral bound notebook icon, near where the "Knit HTML" button appears for `.rmd`. Click and you get "Compile Notebook".
  * Under the hood, you are using a function called `spin()` from the `knitr` package.
  * Jenny's [`ggplot2` demos from her May 2014 tutorial](https://github.com/jennybc/ggplot2-tutorial) were all made this way
    - look at source vs. rendered to get a feel for this
    - download the source and render yourself!
  * Basically, the special comment prefix `#'` becomes very important
  * R Markdown: prose is queen, R code is sequestered in special chunks
  * R script: code is queen, prose is sequestered in special comments
  * You can get virtually same HTML report either way. Which to choose? Depends whether the report is primary goal (choose `.rmd`) or a by-product (choose `.r`).
  
I passed around hard copies of these 5 books (note: some links to eBooks and repositories are tuned to UBC users):

  * [R Graphics Cookbook](http://shop.oreilly.com/product/0636920023135.do) by Winston Chang, O'Reilly (2013). The [graphs section](http://www.cookbook-r.com/Graphs/) of his [Cookbook for R website](http://www.cookbook-r.com) will give you a good sense of the book, which contains more material in greater detail.

  * ggplot2: Elegant Graphics for Data Analysis [available via SpringerLink](http://ezproxy.library.ubc.ca/login?url=http://link.springer.com.ezproxy.library.ubc.ca/book/10.1007/978-0-387-98141-3/page/1) by Hadley Wickham, Springer (2009) | [online docs (nice!)](http://docs.ggplot2.org/current/) | [author's website for the book](http://ggplot2.org/book/), including all the code | [author's landing page for the package](http://ggplot2.org)

  * R Graphics, 2nd edition [available via StatsNetbase](http://ezproxy.library.ubc.ca/login?url=http://www.crcnetbase.com.ezproxy.library.ubc.ca/ISBN/978-1-4398-3176-2) by Paul Murrell, Chapman & Hall/CRC Press (2011) | [author's webpage for the book](http://www.stat.auckland.ac.nz/~paul/RG2e/) | [GoogleBooks search](http://books.google.ca/books?id=uacCQgAACAAJ&source=gbs_book_other_versions) | [companion R package, RGraphics, on CRAN](http://cran.r-project.org/web/packages/RGraphics/index.html)

  * [Dynamic documents with R and `knitr`](http://www.amazon.com/Dynamic-Documents-knitr-Chapman-Series/dp/1482203537) by Yihui Xie, part of the CRC Press / Chapman & Hall R Series (2013). ISBN: 9781482203530. *No online access (yet?).*

  * [Reproducible Research with R & RStudio](http://www.amazon.com/Reproducible-Research-RStudio-Chapman-Series/dp/1466572841) by Christopher Gandrud, part of the CRC Press / Chapman & Hall R Series (2013). ISBN: 978-1466572843. [Book website](http://christophergandrud.github.io/RepResR-RStudio/) | [Examples and code](https://github.com/christophergandrud/Rep-Res-Examples) | [Book source](https://github.com/christophergandrud/Rep-Res-Book). *No online access (yet?).*
  
#### `ggplot2` links

  * A `ggplot2` [tutorial](https://github.com/jennybc/ggplot2-tutorial) I taught May 2014 contains lots of working code, in source form and compiled to something pretty
    - [ggplot2 online docs](http://docs.ggplot2.org/current/)
    - [ggplot2 "homepage"](http://ggplot2.org)
    - [ggplot2 development on github](https://github.com/hadley/ggplot2) 
    - [The R Graphics Cookbook](http://shop.oreilly.com/product/0636920023135.do), an excellent book by Winston Chang.
    - The [graphs section](http://www.cookbook-r.com/Graphs/) of Winston Chang's website Cookbook for R. The book listed above contains much more material, but the website is good too.
    - [ggplot2: Elegant Graphics for Data Analysis](http://www.amazon.com/dp/0387981403/ref=cm_sw_su_dp?tag=ggplot2-20) by Hadley Wickham. [Book's companion website](http://ggplot2.org/book/) offers one R script per chapter, providing the code used in the book.
    - [A quick introduction to ggplot2](http://inundata.org/2013/04/10/a-quick-introduction-to-ggplot2/) by Karthik Ram. Slides and code from a 2 hour talk/hands on presentation for ggplot2 beginners.
  