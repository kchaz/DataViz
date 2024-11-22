This folder contains code for a homework problem for Stat 242 : Time Series in Fall 2024.

Original data come from

​	Fisher, N.I. (1993) *Statistical Analysis of Circular Data*. Cambridge: Cambridge University Press. 

In the class, we modelled these data as coming from a Hidden Markov Model with $Y_t$ measured wind direction viewed as noisy measurements of a true underlying wind direction $\alpha_t$. The processed data in this repo are the result of a particle filter that I implement on these data (I omit this in case this is a homework question in future years of the course). After obtaining posterior samples for $\alpha_t$ and using $\mod(\alpha_t,2\pi)$ to restrict them to $(0,2\pi]$, I calculate the circular mean $\beta_t$ on them [(source)](https://en.wikipedia.org/wiki/Circular_mean) and then plot ($\cos(\beta_t),\sin(\beta_t)$) in the animation.

To see the visualization, click [here](https://kchaz.github.io/DataViz/windviz.html)

