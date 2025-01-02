# Spectral models in VTSCat

The following spectral models are used in VTSCat.

## Gamma-ray spectral models

### Power law

*type: pl*

$$f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}$$

- f<sub>0</sub>: normalisation factor ( = norm in yaml files)
- gamma: spectral index ( = index in yaml files)
- E<sub>ref</sub>: normalisation energy ( = e_ref in yaml files)

### Power law (with integrated normalisation factor)

*type: pl2*

$$\frac{dN}{dE} = F_0 \cdot \left(\frac{E}{E_0}\right)^{-\gamma} \cdot \frac{\gamma+1}{E_{max}^{-\gamma+1}-E_{min}^{-\gamma+1}}$$

- F<sub>0</sub>: integral flux in the interval E<sub>min</sub> to E<sub>max</sub> ( = flux in yaml files)

- gamma: spectral index  ( = index in yaml files)
- E<sub>min</sub>, E<sub>max</sub>: energy interval for integral flux calculation

### Power law with exponential cutoff

*type: ecpl*

$$\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}\cdot \exp \left(-\frac{E}{E_{cut}}\right)$$

- f<sub>0</sub>: normalisation factor ( = norm in yaml files)
- gamma: spectral index   ( = index in yaml files)
- E<sub>ref</sub>: normalisation energy ( = e_ref in yaml files)
- E<sub>cut</sub>: cutoff energy  ( = e_cut in yaml files)

### Log-parabola power law

*type: lppl*

$$\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\alpha - \beta \log \frac{E}{E_{ref}}}$$

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- alpha: spectral index ( = alpha in yaml files)
- beta: pre-factor beta ( = beta in yaml files)
- E<sub>ref</sub>: break energy ( = e_ref in yaml files)

### Smoothly broken power law

*type: brokenpl*

$$\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma_1} \cdot \frac{1}{1+(E/E_{break}^{\gamma_2-\gamma_1})}$$

### Sum of two power laws

*type: pl+pl*

### Sum of power law and power law with exponential cutoff

*type pl+ecpl*

## Cosmic-ray spectral models

### Power law

*type: plCR*

$$\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}$$

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- gamma: spectral index ( = index in yaml files)
- E<sub>ref</sub>: break energy ( = e_ref in yaml files)

### Broken power law

*type: brokenplCR*

$$\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_b}\right)^{-\gamma_1} \ \ \mathrm{if} E \leq E_b$$

$$\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_b}\right)^{-\gamma_2} \ \ \mathrm{if} E > E_b$$

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- gamma_1: spectral index below break energy E<sub>b</sub>  ( = index_1 in yaml files)
- gamma_2: spectral index above break energy E<sub>b</sub>  ( = index_2 in yaml files)
- E<sub>b</sub>: break energy ( = e_break in yaml files)
