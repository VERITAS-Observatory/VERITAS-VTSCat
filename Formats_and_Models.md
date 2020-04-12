# File types, data formats, and spectral models

1. [ Overview of file types. ](#files)
2. [ Observational data (File type VER*.yaml). ](#obs)
3. [ Spectral data (File type VER*sed.ecsv). ](#sed)
4. [ Light-curve data (File type VER*lc.ecsv). ](#lc)
5. [ Spectral models. ](#models)

<a name="files"></a>
## Overview of file types

A README.md file in the directory of each publication provides an overview over available  data products, figures, source names, and citations. The following files types are used and described in more details below:

- VER*.yaml: Observational details and results like observation time, detection significance, source position and morphology, and spectral models results.
- VER*sed.ecsv: Spectral flux points including error and upper limits
- VER*lc.ecsv: Light-curve data (integrated gamma-ray fluxes vs time)
- VER*.fits: Statistical significance or excess coutns sky map (if available)
- VER*table.ecsv: additional tabulated data (if available)

<a name="obs"></a>

## Observational data (File type VER*.yaml)

Observation details are stored in files of *yaml* type. The following table gives an overview of the used keywords and their definitions. Not all entries are given for each data file, as the type of measurement reported varies between the publications.

| Keyword | Definition |
|---|---|
| **data** | observational data and source detection results |
| data:livetime | length of observation time |
| data:significance | statistical significance of observation |
| data:excess | number of excess counts |
| data:excess_err | error on number of excess counts |
| data:non | number of counts in on region |
| data:noff | number of counts in off region |
| data:alpha | normalisation factor between on and off regions |
| **flux** | integral flux measurements |
| flux:flux | integral flux (value and error) |
| flux:eflux | integral energy flux |
| flux:flux_ul | flux upper limit |
| flux:conf | confidence level of flux upper limit |
| flux:emin | energy threshold assumed in integral flux calculation |
| **pos** | results from position fits |
| pos:ra | object position from fit to VERITAS data (right ascension) |
| pos:dec | object position from fit to VERITAS data (declination) |
| pos:glon | object position from fit to VERITAS data (galactic longitude) |
| pos:glat | object position from fit to VERITAS data (galactic latitude) |
| **morph** | results on source morphology |
| morph:type | source morphology type (point or gauss) |
| morph:sigma | source extension (symmetric gaussian or asymetric gaussian morphology) |
| morph:sigma2 | source extension (asymetric gaussian morphology) |
| morph:pa | rotation angle to plane for assymetric gaussian morphology |
| **spec** | results from spectral fits |
| spec:erange | energy range of spectral fit |
| spec:mjd | time range of data used for spectral fit (in MJD) |
| spec:model | spectral model assumed for fit |
| spec:model:type | model type (see below for a description of all spectral models) |
| spec:model:parameters | model parameters (see [below](#models) for a description of all spectral models) |
| spec:theta | integration radius for spectral measurement |

<a name="sed"></a>
### Spectral data (File type VER*sed.ecsv)

Spectral measurements are provided in ecsv files containing all the necessary information unit in their metadata section. The following table gives an overview of the used keywords and their definitions. Not all entries are given for each data file, as the type of measurement reported varies between the publications.

| Keyword | Definition |
|---|---|
| e_ref | reference value for energy bin of spectral measurements |
| e_min/e_max | min and max value of energy bin |
| e_diff | width of energy bin |
| dnde | differential photon flux |
| dnde_err/dnde_errn/dnde_errp | error (average/lower/upper) differential photon flux |
| dnde_ul | upper limit on differential photon flux |
| e2dnde | differential energy flux |
| e2dnde_err | error on differential energy flux |
| e2dnde_ul | upper limit on differential energy flux |
| significance | statistical significance of measurement of gamma-ray excess in this energy bin |

<a name="lc"></a>
### Light-curve data (File type VER*lc.ecsv)

Light-curve measurements are provided in ecsv files containing all the necessary information unit in their metadata section. The following table gives an overview of the used keywords and their definitions. Not all entries are given for each data file, as the type of measurement reported varies between the publications.

| Keyword | Definition |
|---|---|
| time | time of measurement (mean of time bin) |
| time_min/time_max | edges of time bin |
| time_err | width of time bin |
| e_min | minimum energy for flux integration |
| flux | integral energy flux above e_min |
| flux_err/flux_errn/flux_errp | error (average/lower/upper) on integral photon flux |
| flux_ul | upper limit on photon energy flux |
| eflux | integral energy flux above e_min |
| eflux_err/eflux_errn/eflux_errp | error (average/lower/upper) on integral energy flux |
| eflux_ul | upper limit on integral energy flux |

<a name="models"></a>
## Spectral models

The following spectral models are used to descript the fit results from VERITAS observations.  The spectral model description is general identical to the [gammapy](https://docs.gammapy.org/0.17/modeling/index.html) modeling (which is used for plotting of most of the spectra in VTSCat).

### Gamma-ray spectral models

#### Power law

*type: pl*


![f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}](https://render.githubusercontent.com/render/math?math=f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Cgamma%7D)

- f<sub>0</sub>: normalisation factor ( = norm in yaml files)
- gamma: spectral index ( = index in yaml files)
- E<sub>ref</sub>: normalisation energy ( = e_ref in yaml files)

#### Power law (with integrated normalisation factor)

*type: pl2*

![\frac{dN}{dE} = F_0 \cdot \left(\frac{E}{E_0}\right)^{-\gamma} \cdot \frac{\gamma+1}{E_{max}^{-\gamma+1}-E_{min}^{-\gamma+1}}](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%7D%20%3D%20F_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_0%7D%5Cright)%5E%7B-%5Cgamma%7D%20%5Ccdot%20%5Cfrac%7B%5Cgamma%2B1%7D%7BE_%7Bmax%7D%5E%7B-%5Cgamma%2B1%7D-E_%7Bmin%7D%5E%7B-%5Cgamma%2B1%7D%7D)

- F<sub>0</sub>: integral flux in the inverval E<sub>min</sub> to E<sub>max</sub> ( = flux in yaml files)

- gamma: spectral index  ( = index in yaml files)
- E<sub>min</sub>, E<sub>max</sub>: energy interval for integral flux calculation

#### Power law with exponential cutoff 

*type: ecpl*

![\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}\cdot \exp \left(-\frac{E}{E_{cut}}\right)](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Cgamma%7D%5Ccdot%20%5Cexp%20%5Cleft(-%5Cfrac%7BE%7D%7BE_%7Bcut%7D%7D%5Cright))

- f<sub>0</sub>: normalisation factor ( = norm in yaml files)
- gamma: spectral index   ( = index in yaml files)
- E<sub>ref</sub>: normalisation energy ( = e_ref in yaml files)
- E<sub>cut</sub>: cutoff energy  ( = e_cut in yaml files)

#### Log-parabola power law

*type: lppl*

![\frac{dN}{dE} = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\alpha - \beta \log \frac{E}{E_{ref}}}](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Calpha%20-%20%5Cbeta%20%5Clog%20%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%7D)

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- alpha: spectral index ( = alpha in yaml files)
- beta: pre-factor beta ( = beta in yaml files)
- E<sub>ref</sub>: break energy ( = e_ref in yaml files)

### Cosmic-ray spectral models

#### Power law

*type: plCR*

![\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_{ref}}\right)^{-\gamma}](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%20dA%20dt%20d%5COmega%20%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_%7Bref%7D%7D%5Cright)%5E%7B-%5Cgamma%7D)

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- gamma: spectral index ( = index in yaml files)
- E<sub>ref</sub>: break energy ( = e_ref in yaml files)

#### Broken power law

*type: brokenplCR*

![\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_b}\right)^{-\gamma_1} \ \ \mathrm{if} E \leq E_b](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%20dA%20dt%20d%5COmega%20%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_b%7D%5Cright)%5E%7B-%5Cgamma_1%7D%20%5C%20%5C%20%5Cmathrm%7Bif%7D%20E%20%5Cleq%20E_b)

![\frac{dN}{dE dA dt d\Omega } = f_0 \cdot \left(\frac{E}{E_b}\right)^{-\gamma_2} \ \ \mathrm{if} E > E_b](https://render.githubusercontent.com/render/math?math=%5Cfrac%7BdN%7D%7BdE%20dA%20dt%20d%5COmega%20%7D%20%3D%20f_0%20%5Ccdot%20%5Cleft(%5Cfrac%7BE%7D%7BE_b%7D%5Cright)%5E%7B-%5Cgamma_2%7D%20%5C%20%5C%20%5Cmathrm%7Bif%7D%20E%20%3E%20E_b)

- f<sub>0</sub>: normalisation factor  ( = norm in yaml files)
- gamma_1: spectral index below break energy E<sub>b</sub>  ( = index_1 in yaml files)
- gamma_2: spectral index above break energy E<sub>b</sub>  ( = index_2 in yaml files)
- E<sub>b</sub>: break energy ( = e_break in yaml files)
