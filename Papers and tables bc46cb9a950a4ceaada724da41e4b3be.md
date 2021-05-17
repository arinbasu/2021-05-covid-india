# Papers and tables

Insert tables inline

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2F30sPwjQzUven6SgKeb0ivC%2FFirst-Project%3Fnode-id%3D0%253A1" allowfullscreen></iframe>

Latent variable model shown above, below is the code for evaluation

```r
library(lavaan)
# build a model
model1 = '
   latent var =~ Test + Test + Test
'
# fit the model with data
fit1 = cfa(model1, data = mydata)
# fit the model with cov matrix
fit1a = cfa(model1, sample.cov = mycov,
             sample.nobs = 500)

# summary
summary(fit1)
```

👈 To go back, click the link at the top left, or use your sidebar.
