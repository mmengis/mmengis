- š Hi, Iām @mmengis
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
mmengis/mmengis is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
ainv <- ainverse(gryphonped)

model1 <- asreml(
  fixed = bwt ~ 1, random = ~ vm(animal, ainv),
  residual = ~ idv(units),
  data = gryphon,
  na.action = na.method(x = "omit", y = "omit")
)
