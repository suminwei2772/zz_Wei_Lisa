Stat540\_assignment1
================
Lisa Wei
2017-01-06

\*\* 2.1 Passenger breakdown \*\*

``` r
## Converting Titanic array into data frame
Titanic <- data.frame(Titanic);

## Number of children on Titanic
length(which(Titanic$Age=="Child"));
```

    ## [1] 16

``` r
## Number of adults on Titanic
length(which(Titanic$Age=="Adult"))
```

    ## [1] 16

``` r
## Number of male adult passengers
males = Titanic[which(Titanic$Sex=="Male"),]
adult.males = which(males$Age=="Adult")
length(adult.males)
```

    ## [1] 8

``` r
## Number of female adult passengers
females = Titanic[which(Titanic$Sex=="Female"),]
adult.females = which(females$Age=="Adult")
length(adult.females)
```

    ## [1] 8

\*\* 2.2 Survival \*\*

``` survival
child = Titanic[which(Titanic$Age =="Child"),]
length(which(child$Survived=="No"))/nrow(child)
```

\`\`\`
