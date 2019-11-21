# babette_example_6

Branch   |[![Travis CI logo](pics/TravisCI.png)](https://travis-ci.org)                                                                                           |[![AppVeyor logo](pics/AppVeyor.png)](https://appveyor.com)                                                                                               
---------|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
`master` |[![Build Status](https://travis-ci.org/richelbilderbeek/babette_example_6.svg?branch=master)](https://travis-ci.org/richelbilderbeek/babette_example_6) |[![Build status](https://ci.appveyor.com/api/projects/status/4t5r5376tytkvxrd/branch/master?svg=true)](https://ci.appveyor.com/project/richelbilderbeek/babette-example-6/branch/master)
`develop`|[![Build Status](https://travis-ci.org/richelbilderbeek/babette_example_6.svg?branch=develop)](https://travis-ci.org/richelbilderbeek/babette_example_6)|[![Build status](https://ci.appveyor.com/api/projects/status/4t5r5376tytkvxrd/branch/develop?svg=true)](https://ci.appveyor.com/project/richelbilderbeek/babette-example-6/branch/develop)

A [babette example](https://github.com/richelbilderbeek/babette_examples).

## Example #6: Yule tree prior with a normally distributed birth rate

![Example #6: Yule tree prior with a normally distributed birth rate](pics/birth_rate_normal_2_4.png)

```{r example_6}
posterior <- bbt_run(
  "my_alignment.fas",
  tree_prior = create_yule_tree_prior(
    birth_rate_distr = create_normal_distr()
  ) 
)
```

All other parameters are set to their defaults, as in BEAUti.

## Result

![](result.png)
