Discrimination slope (DS), Integrated discrimination improvement (IDI) demo
===
Graphical representation of how the discrimination slope for a time _t_ is calculated using survival data. The discrimination slope (DS) is probably more well known as one half of the integrated discrimination improvement ([IDI](http://onlinelibrary.wiley.com/doi/10.1002/sim.2929/full)). Specifically, IDI is the _improvement_ in DS between two survival models (typically model A uses a baseline set of predictors and model B adds a predictor of interest).

There is an interactive element: click on the desired time _t_ on the scatterplot, which will trigger the animation for calculating DS at _t_. Click again to reset.

Note that this shows an inefficient estimation method, as censoring is ignored. It's useful mainly as an intuitive visual teaching tool. [Uno _et al._ (2012)](http://onlinelibrary.wiley.com/doi/10.1002/sim.5647/full) developed an estimator that incorporates censoring and assumes the Cox model. They also have an [accompanying R package](http://cran.r-project.org/web/packages/survIDINRI/index.html).

Some things yet to do:

* Still need to convert from native predictor scale to predicted probability scale
* Need to insert explanatory text and tooltips

Please feel free to suggest comments and/or submit pull requests! Built using [D3.js](https://github.com/mbostock/d3).