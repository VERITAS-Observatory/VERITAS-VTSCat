# File types and data formats in VTSCat

1. [ Overview of file types. ](#files)
2. [ Observational data (File type VER*.yaml). ](#obs)
3. [ Spectral data (File type VER*sed.ecsv). ](#sed)
4. [ Light-curve data (File type VER*lc.ecsv). ](#lc)

For a description of the spectral models used, see [SpectralModels.md](SpectralModels.md).

<a name="files"></a>
## File types

A README.md file in the directory of each publication provides an overview over available  data products, figures, source names, and citations.
A Bibtex file (*bibtex.bib*) allows to include easily the citation for each publication into a Latex-style document.

The following files types are used and described in more details below:

- VER*.yaml: Observational details and results like observation time, detection significance, source position and morphology, and spectral models results.
- VER*sed.ecsv: Spectral flux points including error and upper limits
- VER*lc.ecsv: Light-curve data (integrated gamma-ray fluxes vs time)
- VER*.fits: Statistical significance or excess counts sky map (if available)
- VER*table.ecsv: additional tabulated data (if available)

<a name="obs"></a>

## Observational data (File type VER*.yaml)

Observation details are stored in files of *yaml* type. The following table gives an overview of the used keywords and their definitions. Not all entries are given for each data file, as the type of measurements reported varies between the publications.

| Keyword | Definition |
|---|---|
| **data** | observational data and source detection results |
| data:livetime | length of observation time |
| data:significance | statistical significance of observation (generally taking after taking trials into account |
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
| spec:chi2 | Chi2 of spectral model fit |
| spec:ndf | Number of degrees of freedom in spectral model fit |

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
| dnde_syserr/dnde_syserrn/dnde_syserrp | systematic error (average/lower/upper) differential photon flux |
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
| f_var | fractional variability |

