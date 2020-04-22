
# Compartmental Epidemic Model for COVID analysis
reference : https://arxiv.org/pdf/2002.06563.pdf

![seirqdp model](/seirqdp.png)

To characterize the epidemic of COVID-19, a generalized classical SEIR model is used by introducing 7 different states

Constant <p align="center"><img src="/tex/bb9188fdda20aa975fe905e0527c2622.svg?invert_in_darkmode&sanitize=true" align=middle width=242.59716854999996pt height=14.42921205pt/></p> is the total population.

The coefficients are
  * `<\alpha>` → protection rate
  * `<\beta>` → infection rate
  * `<\gamma^{-1}>` → avg latent time
  * `<\delta^{-1}>` → avg quarantine time
  * `<\lambda(t)=\lambda_0(1-e^{-\lambda_1t})>` → cure rate
  * `<\kappa(t)=\kappa_0e^{-\kappa_1t}>` → mortality rate

It is assumed the cure rate `<\lambda>` and the mortality rate `<\kappa>` are both time dependent.

The SEIRQP model is described by following differential equations

$$\frac{dS\left(t\right)}{dt}=-\beta\frac{S\left(t\right)I\left(t\right)}{N}-\alpha S\left(t\right)$$

$$\frac{dE\left(t\right)}{dt}=\beta\frac{S\left(t\right)I\left(t\right)}{N}-\gamma E\left(t\right)$$

$$\frac{dI\left(t\right)}{dt}=\gamma E\left(t\right)-\delta I\left(t\right)$$

$$\frac{dQ\left(t\right)}{dt}=\delta I\left(t\right)-\lambda\left(t\right)Q\left(t\right)-\kappa\left(t\right)Q\left(t\right)$$

$$\frac{dR\left(t\right)}{dt}=\lambda\left(t\right)Q\left(t\right)$$

$$\frac{dD\left(t\right)}{dt}=\kappa\left(t\right)Q\left(t\right)$$

$$\frac{dP\left(t\right)}{dt}=\alpha S\left(t\right) $$

## Parameter Estimation
The fitting is done using the time histories of the number of quarantined Q(t), recovered R(t) and deaths D(t) only. Time histories obtained from   https://www.worldometers.info/coronavirus/country/india/

## Forecast from estimated model

