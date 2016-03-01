
# Jekyll + Rmd + htmlwidgets for sharing/publishing science to the web

Purpose:
* Share interactive Rmarkdown documents with collaborators in a clean interface
* Do it all from within RStudio

How I use it:
* Edit Rmarkdown and preview rendered site in Rstudio using `servr::jekyll()`
* Use Git with a post-receive hook for building and deploying the Jekyll site remotely
* Git push (from whithin RStudio) now becomes deploy

Based on:
* knitr-jekyll by yihui, with addin of htmlwidgets support (borrowed from https://brendanrocks.com/htmlwidgets-knitr-jekyll/)
* Full-text search with lunr.js (solution borrowed from https://github.com/katydecorah/katydecorah.github.io)
* Archive timeline styling from https://github.com/katydecorah/katydecorah.github.io

Requirements:
* [Jekyll 3.x](http://jekyllrb.com)
* [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar)
* [jekyll_file_exists](https://github.com/michaelx/jekyll_file_exists) (included in this repo)

Note: if hosting on Github pages, you will have to build the site locally first since the jekyll plugins are not allowed.
