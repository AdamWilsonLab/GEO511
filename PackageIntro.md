---
title: "Resource Introduction"
---

# Description

Each student will be expected to introduce an R-related resource that is relevant to their research interests in a 5 minute presentation during a class session.  Most students elect to introduce an R package, but you could also introduce a data source, interesting blog, etc., as long as it's relevant to the course.  If you are aren't sure, please ask Professor Wilson.  The objectives are:

* Learn how to find/download/install a new package and learn how to use it
* Teach your peers about existing R packages that may be useful in their research

The presentation must include:

1. Brief introduction: what does the package do and why is it useful? (**1-2 slides, 1 minute**)
2. Author introduction: a short background (affiliation and other packages, etc.) on at least one of the package authors (**1 slide, 1 minute**)
2. Simple demonstration of package code: example input/output from the examples or custom coded examples (**2-3 slides, 3 minutes**)

There will not be time to actually run any code *on-the-fly* during your presentation.  Instead, use RMarkdown to create a presentation (html) or markdown (md) file so that you can simply display it during class (like the lectures).  Then paste your github link into the schedule spreadsheet so we can easily open/view it during class. For the first few weeks, you may simply share your screen and use a powerpoint or other presentation software.

To select a package, I recommend starting with the [views on CRAN](https://cran.r-project.org/web/views/) for a topic of interest.  Then read the narrative in the task view for something interesting to you and install the package in R with `install.package("packagename")` in R and take a look at what it can do.  Most package functions include sample code that performs a function.    For example, if I was introducing the `dplyr` package, I might choose the `filter()` function.  If you look in the help you will find a section called "Examples" that you can use for your example code in your presentation.  All you have to do is copy-paste it from the help into the R console and them summarize what it's doing in your presentation.  For example, I might demonstrate (from the `filter()` documentation) that the following code will select all characters from Star Wars that are human.


```r
library(dplyr)
filter(starwars, species == "Human")
```

```
## # A tibble: 35 x 14
##    name  height  mass hair_color skin_color eye_color birth_year sex   gender
##    <chr>  <int> <dbl> <chr>      <chr>      <chr>          <dbl> <chr> <chr> 
##  1 Luke…    172    77 blond      fair       blue            19   male  mascu…
##  2 Dart…    202   136 none       white      yellow          41.9 male  mascu…
##  3 Leia…    150    49 brown      light      brown           19   fema… femin…
##  4 Owen…    178   120 brown, gr… light      blue            52   male  mascu…
##  5 Beru…    165    75 brown      light      blue            47   fema… femin…
##  6 Bigg…    183    84 black      light      brown           24   male  mascu…
##  7 Obi-…    182    77 auburn, w… fair       blue-gray       57   male  mascu…
##  8 Anak…    188    84 blond      fair       blue            41.9 male  mascu…
##  9 Wilh…    180    NA auburn, g… fair       blue            64   male  mascu…
## 10 Han …    180    80 brown      fair       brown           29   male  mascu…
## # … with 25 more rows, and 5 more variables: homeworld <chr>, species <chr>,
## #   films <list>, vehicles <list>, starships <list>
```

## Example Presentation

Here is an example presentation about the [`ggrepel` package](pres/PackagePresentation.html) that was built using this [R Markdown file](pres/PackagePresentation.Rmd), which is [also visible on github](https://github.com/AdamWilsonLab/GEO511/blob/master/pres/PackagePresentation.Rmd).


