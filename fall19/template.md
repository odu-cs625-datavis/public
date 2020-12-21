Enter title here
================
Enter Your Name here

*Example of using runnable R code to generate plot*

``` r
ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy, color = class))
```

![](template_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

***Make sure after Knitting to commit the generated `.md` file and all
files in the generated `_files` folder.***
