# ANALYSIS-OF-SIMULATED-COSMIC-MICROWAVE-BACKGROUND-POLARIZATION-DATA-
Plots of powers spectrum ($C_\ell^{TT}$, $C_\ell^{EE}$, $C_\ell^{BB}$, $C_\ell^{TE}$)


![](https://i.imgur.com/lhL00Sf.jpg) 

Study of some cosmological dependencies ($r$ and $\tau$) : 

![](https://i.imgur.com/KUtmMSe.jpg)
![](https://i.imgur.com/F6iAZus.jpg)

map T : 
![](https://i.imgur.com/WyJoxK6.jpg)

map Q : 
![](https://i.imgur.com/IqkyrQK.jpg)
map U : 
![](https://i.imgur.com/7gD6n64.jpg)

data simulated using stokes parameters maps (T,Q,U) : 
![](https://i.imgur.com/ryl93Wx.jpg)

Estimation of r by gaussian Log-Likelihood minimization
---------------------------------------------------------

We can show (from [J.Errard et al 2019](https://doi.org/10.1103%2Fphysrevd.99.043529)) : 
 
$$-2 \log(L) =  fsky * \sum_{l} (2l+1)[C_{\ell}^{-1} D_{\ell} + ln(C_{\ell})] = \chi^{2}$$

$$ L = \exp\Big(-\left(\chi^{2} - \min(\chi^{2})\right)^{2}\Big) $$

Where $C_{\ell}$ is the theoretical spectrum (the model) and $D_{\ell}$ is the reconstructed spectrum with white noise. 

For the covariance, we can write : 

$$C_{\ell}(r) = \frac{1}{r_{0}} r  C_{\ell, tensor}^{BB}(r = r_{0}) + C_{\ell,lensing}^{BB} + N_{\ell}$$

Where $N_{\ell}$ is the white noise. 

![](https://i.imgur.com/Dj8M0xL.jpg)

MCMC (Marlov Chain Monte Carlo) method to estimate $r$ and $Alens$  :

![](https://i.imgur.com/DxRPH8U.jpg)

Exemple of map with mask (via PyMaster / NaMaster) : 

![](https://i.imgur.com/8UEz7Bg.jpg)


![](https://i.imgur.com/VB7Bga3.jpg)


![](https://i.imgur.com/kmtXpyH.jpg)

