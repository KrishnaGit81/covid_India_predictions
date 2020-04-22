
# Compartmental Epidemic Model for COVID analysis
![seirqdp model](/seirqdp.png)

To characterize the epidemic of COVID-19, a generalized classical SEIR model is used by introducing 7 different states
Constant <p align="center"><img src="/tex/bb9188fdda20aa975fe905e0527c2622.svg?invert_in_darkmode&sanitize=true" align=middle width=242.59716854999996pt height=14.42921205pt/></p> is the total population.
The coefficients are
*<p align="center"><img src="/tex/a6eca520b045472266ecb2c6c5f2a71c.svg?invert_in_darkmode&sanitize=true" align=middle width=10.576504949999999pt height=7.0776222pt/></p> → protection rate
*<p align="center"><img src="/tex/d74acd278fad497ab7a6e38616718ebc.svg?invert_in_darkmode&sanitize=true" align=middle width=10.165550999999999pt height=14.611878599999999pt/></p> → infection rate
*<p align="center"><img src="/tex/2c0da98e9c4fe60111c204449e329f9f.svg?invert_in_darkmode&sanitize=true" align=middle width=26.25042915pt height=17.399144399999997pt/></p> → avg latent time
*<p align="center"><img src="/tex/cfabb555ac9b0e396f5e788663f376c6.svg?invert_in_darkmode&sanitize=true" align=middle width=24.7546398pt height=14.202794099999998pt/></p> → avg quarantine time
*<p align="center"><img src="/tex/067d63d908a15151c5ec5403374e410c.svg?invert_in_darkmode&sanitize=true" align=middle width=164.93717955pt height=20.5316694pt/></p> → cure rate
*<p align="center"><img src="/tex/89a39e63fc0cc1bc7792643ec8ba7f4e.svg?invert_in_darkmode&sanitize=true" align=middle width=106.70107635000001pt height=18.0201615pt/></p> → mortality rate
  
It is assumed the cure rate <p align="center"><img src="/tex/18f8eacfb4280d2c13c04e23edc6650d.svg?invert_in_darkmode&sanitize=true" align=middle width=9.589082249999999pt height=11.4155283pt/></p> and the mortality rate <p align="center"><img src="/tex/8d8d6de7d9b2c975505cf593972a87a0.svg?invert_in_darkmode&sanitize=true" align=middle width=9.4711155pt height=7.0776222pt/></p> are both time dependent.
The SEIRQP model is described by following differential equations

<p align="center"><img src="/tex/cc4cde61b4f05d62b730cf403142b380.svg?invert_in_darkmode&sanitize=true&sanitize=true" align=middle width=14.469991799999997pt height=14.77813755pt/></p>
