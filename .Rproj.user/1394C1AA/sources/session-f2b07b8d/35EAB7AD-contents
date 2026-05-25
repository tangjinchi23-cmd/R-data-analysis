## Demonstration of Functions from the `cluster` Package

This section demonstrates three key clustering functions from the **cluster** package:  
  **PAM**, **AGNES**, and **DIANA**.  
All examples use a small custom dataset to avoid duplication of help-page examples.

### Load Packages and Data

```{r}
library(cluster)

# create an original dataset (not from help pages)
set.seed(123)
demo_data <- data.frame(
  feature1 = rnorm(60, mean = rep(c(0, 3, 6), each = 20)),
  feature2 = rnorm(60, mean = rep(c(0, 3, 0), each = 20))
)

head(demo_data)