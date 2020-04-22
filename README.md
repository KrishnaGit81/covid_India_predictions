
# Compartmental Epidemic Model for COVID analysis
reference : https://arxiv.org/pdf/2002.06563.pdf

![seirqdp model](/seirqdp.png)

To characterize the epidemic of COVID-19, a generalized classical SEIR model is used by introducing 7 different states

Constant <p align="center"><img src="/tex/bb9188fdda20aa975fe905e0527c2622.svg?invert_in_darkmode&sanitize=true&sanitize=true" align=middle width=242.59716854999996pt height=14.42921205pt/></p> is the total population.

The coefficients are
  * `<\alpha>` → protection rate
  * `<\beta>` → infection rate
  * `<\gamma^{-1}>` → avg latent time
  * `<\delta^{-1}>` → avg quarantine time
  * `<\lambda(t)=\lambda_0(1-e^{-\lambda_1t})>` → cure rate
  * `<\kappa(t)=\kappa_0e^{-\kappa_1t}>` → mortality rate

It is assumed the cure rate `<\lambda>` and the mortality rate `<\kappa>` are both time dependent.

The SEIRQP model is described by following differential equations

<p align="center"><img src="/tex/bbd3a63b515463869e062086429bc58f.svg?invert_in_darkmode&sanitize=true" align=middle width=220.19243070000002pt height=34.7253258pt/></p>

<p align="center"><img src="/tex/1240a1badb62029be2f1011fe7e2b128.svg?invert_in_darkmode&sanitize=true" align=middle width=210.36394994999998pt height=34.7253258pt/></p>

<p align="center"><img src="/tex/474722f164ee8e4f1020d226b9e05531.svg?invert_in_darkmode&sanitize=true" align=middle width=164.3869128pt height=34.7253258pt/></p>

<p align="center"><img src="/tex/a87cb440737793e05b45b99a5bd8a9cc.svg?invert_in_darkmode&sanitize=true" align=middle width=281.36538705pt height=34.7253258pt/></p>

<p align="center"><img src="/tex/df90b9f30645670978ff8e95f851baee.svg?invert_in_darkmode&sanitize=true" align=middle width=134.76232109999998pt height=34.7253258pt/></p>

<p align="center"><img src="/tex/6406db8b8f64acbf428e734e7b47a448.svg?invert_in_darkmode&sanitize=true" align=middle width=136.10209799999998pt height=34.7253258pt/></p>

<p align="center"><img src="/tex/25373626249f69137d1019c979697fd7.svg?invert_in_darkmode&sanitize=true" align=middle width=109.80917475000001pt height=34.7253258pt/></p>

## Parameter Estimation
The fitting is done using the time histories of the number of quarantined Q(t), recovered R(t) and deaths D(t) only. Time histories obtained from   https://www.worldometers.info/coronavirus/country/india/

## Forecast from estimated model

