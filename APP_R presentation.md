APP Introduction
========================================================
author: Jinjin Mo
date: 05/24/2015

Hardy-Weinberg Equilibrium
========================================================

**INTRODUCTION**

The Hardy-Weinberg equilibrium is a principle stating that the genetic variation in a population will remain constant from one generation to the next in the absence of disturbing factors. When mating is random in a large population with no disruptive circumstances, the law predicts that both genotype and allele frequencies will remain constant because they are in equilibrium.




Hardy-Weinberg Equilibrium Calculator
========================================================
[Hardy-Weinberg Equilibrium Calculator](https://mojinjin.shinyapps.io/APP_assignment)

- **Input**: observed counts for each genotype
  -  Common Homozygotes
  -  Heterozygotes
  -  Heterozygotes

- **Output**: in the result panel
  -  observed samples
  -  statistic: X-squared, indicating the difference between expected and observed values for genotype counts.
  -  *p* value


Example
========================================================


Given in a sample population:Common Homozygotes = 10, Heterozygotes = 5 and Heterozygotes = 23,

So the test result is:

```r
resulHWE <- function(x, y, z)HWE.chisq(genotype(c(rep("A/A",x), rep("A/a", y), rep("a/a", z))))
resulHWE(10, 5, 23)
```

```

	Pearson's Chi-squared test with simulated p-value (based on 10000
	replicates)

data:  tab
X-squared = 18.7245, df = NA, p-value = 9.999e-05
```


Conclusion
========================================================
- The example above shows *p* value is smaller than the significance level(0.05), which suggests that the observed data aren't under Hardy-Weinberg equilibrium.

- Five forces leading to evolutionary change may affect the Hardy-Weinberg equilibrium:
  - *mutation*
  - *gene flow*
  - *genetic drift*
  - *nonrandom mating*
  - *natural selection*
 
 
 
