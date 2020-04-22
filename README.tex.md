
# Compartmental Epidemic Model for COVID analysis
![seirqdp model](/seirqdp.png)

To characterize the epidemic of COVID-19, a generalized classical SEIR model is used by introducing 7 different states
Constant $$N=S+P+E+I+Q+R+D$$ is the total population.
The coefficients are
*$$\alpha$$ → protection rate
*$$\beta$$ → infection rate
*$$\gamma^{-1}$$ → avg latent time
*$$\delta^{-1}$$ → avg quarantine time
*$$\lambda\left(t\right)=\lambda_0\left(1-e^{-\lambda_1t}\right)\$$ → cure rate
*$$\kappa\left(t\right)=\kappa_0e^{-\kappa_1t}$$ → mortality rate
  
It is assumed the cure rate $$\lambda$$ and the mortality rate $$\kappa$$ are both time dependent.
The SEIRQP model is described by following differential equations

<p align="center"><img src="/tex/cc4cde61b4f05d62b730cf403142b380.svg?invert_in_darkmode&sanitize=true" align=middle width=14.469991799999997pt height=14.77813755pt/></p>
