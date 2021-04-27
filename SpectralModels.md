# Spectral models in VTSCat

Spectral model description is in most cases identical to the [gammapy](https://docs.gammapy.org/0.17/modeling/index.html) modeling (which is used for plotting of most of the spectra in VTSCat).

## Gamma-ray spectral models

### Power law

*type: pl*


![f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}](https://render.githubusercontent.com/render/math?math=f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Cgamma%7D)

- f<sub>0</sub>: normalisation factor ( = norm in yaml files)
- gamma: spectral index ( = index in yaml files)
- E<sub>ref</sub>: normalisation energy ( = e_ref in yaml files)

### Power law (with integrated normalisation factor)

*type: pl2*

![\frac{dN}{dE} = F_0 \cdot \left(\frac{E}{E_0}\right)^{-\gamma} \cdot \frac{\gamma+1}{E_{max}^{-\gamma+1}-E_{min}^{-\gamma+1}}](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%7D%20%3D%20F_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_0%7D%5Cright)%5E%7B-%5Cgamma%7D%20%5Ccdot%20%5Cfrac%7B%5Cgamma%2B1%7D%7BE_%7Bmax%7D%5E%7B-%5Cgamma%2B1%7D-E_%7Bmin%7D%5E%7B-%5Cgamma%2B1%7D%7D)

- F<sub>0</sub>: integral flux in the inverval E<sub>min</sub> to E<sub>max</sub> ( = flux in yaml files)

- gamma: spectral index  ( = index in yaml files)
- E<sub>min</sub>, E<sub>max</sub>: energy interval for integral flux calculation

### Power law with exponential cutoff 

*type: ecpl*

![\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}\cdot \exp \left(-\frac{E}{E_{cut}}\right)](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Cgamma%7D%5Ccdot%20%5Cexp%20%5Cleft(-%5Cfrac%7BE%7D%7BE_%7Bcut%7D%7D%5Cright))

- f<sub>0</sub>: normalisation factor ( = norm in yaml files)
- gamma: spectral index   ( = index in yaml files)
- E<sub>ref</sub>: normalisation energy ( = e_ref in yaml files)
- E<sub>cut</sub>: cutoff energy  ( = e_cut in yaml files)

### Log-parabola power law

*type: lppl*

![\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\alpha - \beta \log \frac{E}{E_{ref}}}](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Calpha%20-%20%5Cbeta%20%5Clog%20%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%7D)

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- alpha: spectral index ( = alpha in yaml files)
- beta: pre-factor beta ( = beta in yaml files)
- E<sub>ref</sub>: break energy ( = e_ref in yaml files)

## Cosmic-ray spectral models

### Power law

*type: plCR*

![\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%20dA%20dt%20d%5COmega%20%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Cgamma%7D)

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- gamma: spectral index ( = index in yaml files)
- E<sub>ref</sub>: break energy ( = e_ref in yaml files)

### Broken power law

*type: brokenplCR*

![\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_b}\right)^{-\gamma_1} \ \ \mathrm{if} E \leq E_b](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%20dA%20dt%20d%5COmega%20%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_b%7D%5Cright)%5E%7B-%5Cgamma_1%7D%20%5C%20%5C%20%5Cmathrm%7Bif%7D%20E%20%5Cleq%20E_b)

![\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_b}\right)^{-\gamma_2} \ \ \mathrm{if} E > E_b](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%20dA%20dt%20d%5COmega%20%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_b%7D%5Cright)%5E%7B-%5Cgamma_2%7D%20%5C%20%5C%20%5Cmathrm%7Bif%7D%20E%20%3E%20E_b)

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- gamma_1: spectral index below break energy E<sub>b</sub>  ( = index_1 in yaml files)
- gamma_2: spectral index above break energy E<sub>b</sub>  ( = index_2 in yaml files)
- E<sub>b</sub>: break energy ( = e_break in yaml files)
