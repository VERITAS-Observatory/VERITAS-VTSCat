# VTSCat - the VERITAS data catalogue

1. [ Introduction. ](#intro)
2. [ Organisation and data format. ](#formats)
3. [ Publications. ](#publications)
4. [ Sources and Targets. ](#sources)
5. [ Licence. ](#licence)

<a name="intro"></a>
## Introduction

**VTSCat** is the catalog of high-level data products from all publications of the [VERITAS collaboration](https://veritas.sao.arizona.edu/).

VTSCat is currently in the pre-release state and tested. Please checkout [this branch](https://github.com/VERITAS-Observatory/VERITAS-VTSCat/tree/pre-release-v03a) for the data files.

The **VTSCat** data collection contains:

- high-level data like spectral flux points, light curves, spectral fits in human- and machine-readable yaml and ecsv file format
- tabled data like upper limits tables from dark matter searches or results on the extragalactic background in ecsv file format
- sky maps (wherever available) in FITS file format

The data collection contains results from gamma-ray measurements only. Multiwavelength data like X-ray light curves and spectra will probably be added in a future release.

VTSCat supplements the HEASARC catalogue of VERITAS results (to be published). It is inspired and derived from [gamma-cat](https://github.com/gammapy/gamma-cat).

**Access**:

- GitHub: https://github.com/VERITAS-Observatory/VERITAS-VTSCat 
- ZENODO: https://doi.org/10.5281/zenodo.4723219
- HEASARC (**link to be added**)

**Citation:** if you make use of VTSCat, please cite the orginal publication for the data, the DOI ([10.5281/zenodo.4723219](https://doi.org/10.5281/zenodo.4723219)) the following research note: (**link to be added**)

<a name="formats"></a>

## Organisation and data format

Data files are organised in VTSCat by year and publication, using ADS bibcodes as reference identifiers. Objects are identified by a running integer (labeled source id in data files) following the scheme developed by gamma-cat. The description files for objects can be found in the sources subdirectory and include the most relevant names for a given object (common name in the field, VERITAS object identifier, primary identifier by SIMBAD), and the object coordinates.

Units are given in the data files for reported data following conventions provided by [astropy](https://docs.astropy.org/en/stable/units/).

For a detailed description of data formats, file types, keywords, and spectral models see the [description here](Formats_and_Models.md).

## References

- VERITAS: https://veritas.sao.arizona.edu/
- VER Dictionary of Nomenclature: https://cds.u-strasbg.fr/cgi-bin/Dic-Simbad?/17350620
- gamma-cat: https://github.com/gammapy/gamma-cat

<a name="publications"></a>

## Publication list

| Object | Publication Title | ADS Reference | Repository |
|---|---|---|---|
|Crab nebula / VER J0534+220 | The throughput calibration of the VERITAS telescopes | [2021arXiv211104676A](http://adsabs.harvard.edu/abs/2021arXiv211104676A) | [data files](2021/2021arXiv211104676A) |
|3C 279 | Variability and Spectral Characteristics of Three Flaring Gamma-ray Quasars Observed by VERITAS and Fermi-LAT | [2021arXiv211013181A](http://adsabs.harvard.edu/abs/2021arXiv211013181A) | [data files](2021/2021arXiv211013181A) |
|PKS 1222+216 | Variability and Spectral Characteristics of Three Flaring Gamma-ray Quasars Observed by VERITAS and Fermi-LAT | [2021arXiv211013181A](http://adsabs.harvard.edu/abs/2021arXiv211013181A) | [data files](2021/2021arXiv211013181A) |
|Ton 599 | Variability and Spectral Characteristics of Three Flaring Gamma-ray Quasars Observed by VERITAS and Fermi-LAT | [2021arXiv211013181A](http://adsabs.harvard.edu/abs/2021arXiv211013181A) | [data files](2021/2021arXiv211013181A) |
|HESS J0632+057 / VER J0633+057 | Observation of the Gamma-Ray Binary HESS J0632+057 with the H.E.S.S., MAGIC, and VERITAS Telescopes | [2021ApJ...923..241A](http://adsabs.harvard.edu/abs/2021ApJ...923..241A) | [data files](2021/2021ApJ...923..241A) |
|HESS J0632+057 / VER J0633+057 | Multiwavelength Observation Campaign of the TeV Gamma-Ray Binary HESS J0632 + 057 with NuSTAR, VERITAS, MDM, and Swift | [2021ApJ...923...17T](http://adsabs.harvard.edu/abs/2021ApJ...923...17T) | [data files](2021/2021ApJ...923...17T) |
| x | An Archival Search for Neutron-star Mergers in Gravitational Waves and Very-high-energy Gamma Rays | [2021ApJ...918...66A](http://adsabs.harvard.edu/abs/2021ApJ...918...66A) | [data files](2021/2021ApJ...918...66A) |
|PSR B0355+54 | A Search for TeV Gamma-Ray Emission from Pulsar Tails by VERITAS | [2021ApJ...916..117B](http://adsabs.harvard.edu/abs/2021ApJ...916..117B) | [data files](2021/2021ApJ...916..117B) |
|PSR J0357+32 | A Search for TeV Gamma-Ray Emission from Pulsar Tails by VERITAS | [2021ApJ...916..117B](http://adsabs.harvard.edu/abs/2021ApJ...916..117B) | [data files](2021/2021ApJ...916..117B) |
|PSR J1740+1000 | A Search for TeV Gamma-Ray Emission from Pulsar Tails by VERITAS | [2021ApJ...916..117B](http://adsabs.harvard.edu/abs/2021ApJ...916..117B) | [data files](2021/2021ApJ...916..117B) |
|Galactic Centre / VER J1745-290 | VERITAS Observations of the Galactic Center Region at Multi-TeV Gamma-Ray Energies | [2021ApJ...913..115A](http://adsabs.harvard.edu/abs/2021ApJ...913..115A) | [data files](2021/2021ApJ...913..115A) |
|SNR G0.9+0.1 / VER J1747-281 | VERITAS Observations of the Galactic Center Region at Multi-TeV Gamma-Ray Energies | [2021ApJ...913..115A](http://adsabs.harvard.edu/abs/2021ApJ...913..115A) | [data files](2021/2021ApJ...913..115A) |
|VER J1746-289 / VER J1746-289 | VERITAS Observations of the Galactic Center Region at Multi-TeV Gamma-Ray Energies | [2021ApJ...913..115A](http://adsabs.harvard.edu/abs/2021ApJ...913..115A) | [data files](2021/2021ApJ...913..115A) |
|GC diffuse ridge / VER J1746-286 | VERITAS Observations of the Galactic Center Region at Multi-TeV Gamma-Ray Energies | [2021ApJ...913..115A](http://adsabs.harvard.edu/abs/2021ApJ...913..115A) | [data files](2021/2021ApJ...913..115A) |
|M 87 / VER J1230+123 | Broadband Multi-wavelength Properties of M87 during the 2017 Event Horizon Telescope Campaign | [2021ApJ...911L..11E](http://adsabs.harvard.edu/abs/2021ApJ...911L..11E) | [data files](2021/2021ApJ...911L..11E) |
|3C 264.0 / VER J1145+196 | VERITAS Discovery of VHE Emission from the Radio Galaxy 3C 264: A Multiwavelength Study | [2020ApJ...896...41A](http://adsabs.harvard.edu/abs/2020ApJ...896...41A) | [data files](2020/2020ApJ...896...41A) |
|Cassiopeia A / VER J2323+588 | Evidence for Proton Acceleration up to TeV Energies Based on VERITAS and Fermi-LAT Observations of the Cas A SNR | [2020ApJ...894...51A](http://adsabs.harvard.edu/abs/2020ApJ...894...51A) | [data files](2020/2020ApJ...894...51A) |
|1ES 1215+303 / VER J1217+301 | A Decade of Multiwavelength Observations of the TeV Blazar 1ES 1215+303: Extreme Shift of the Synchrotron Peak Frequency and Long-term Optical-Gamma-Ray Flux Increase | [2020ApJ...891..170V](http://adsabs.harvard.edu/abs/2020ApJ...891..170V) | [data files](2020/2020ApJ...891..170V) |
|Markarian 421 / VER J1104+382 | The Great Markarian 421 Flare of 2010 February: Multiwavelength Variability and Correlation Studies | [2020ApJ...890...97A](http://adsabs.harvard.edu/abs/2020ApJ...890...97A) | [data files](2020/2020ApJ...890...97A) |
|HESS J0632+057 / VER J0633+057 | Probing the Properties of the Pulsar Wind in the Gamma-Ray Binary HESS J0632+057 with NuSTAR and VERITAS Observations | [2020ApJ...888..115A](http://adsabs.harvard.edu/abs/2020ApJ...888..115A) | [data files](2020/2020ApJ...888..115A) |
|LS 5039 / VER J1826-148 | VERITAS Detection of LS 5039 and HESS J1825-137 | [2020APh...11702403A](http://adsabs.harvard.edu/abs/2020APh...11702403A) | [data files](2020/2020APh...11702403A) |
|HESS J1825-137 / VER J1825-138 | VERITAS Detection of LS 5039 and HESS J1825-137 | [2020APh...11702403A](http://adsabs.harvard.edu/abs/2020APh...11702403A) | [data files](2020/2020APh...11702403A) |
| x | Direct measurement of stellar angular diameters by the VERITAS Cherenkov telescopes | [2019NatAs...3..511B](http://adsabs.harvard.edu/abs/2019NatAs...3..511B) | [data files](2019/2019NatAs...3..511B) |
|3C 66A / VER J0222+430 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 0229+200 / VER J0232+202 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 0414+009 / VER J0416+011 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 0502+675 / VER J0507+676 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|RGB J0710+591 / VER J0710+591 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 1011+496 / VER J1015+494 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 1215+303 / VER J1217+301 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 1218+304 / VER J1221+301 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|MS1221.8+2452 / VER J1224+246 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|PKS 1424+240 / VER J1427+237 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|H 1426+428 / VER J1428+426 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|PG 1553+113 / VER J1555+111 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 1959+650 / VER J1959+651 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
|1ES 2344+514 / VER J2347+517 | Measurement of the Extragalactic Background Light Spectral Energy Distribution with VERITAS | [2019ApJ...885..150A](http://adsabs.harvard.edu/abs/2019ApJ...885..150A) | [data files](2019/2019ApJ...885..150A) |
| x | A Search for Pulsed Very High-energy Gamma-Rays from 13 Young Pulsars in Archival VERITAS Data | [2019ApJ...876...95A](http://adsabs.harvard.edu/abs/2019ApJ...876...95A) | [data files](2019/2019ApJ...876...95A) |
|TXS 0506+056 / VER J0509+057 | Multimessenger observations of a flaring blazar coincident with high-energy neutrino IceCube-170922A | [2018Sci...361.1378I](http://adsabs.harvard.edu/abs/2018Sci...361.1378I) | [data files](2018/2018Sci...361.1378I) |
|electron | Measurement of cosmic-ray electrons at TeV energies by VERITAS | [2018PhRvD..98f2004A](http://adsabs.harvard.edu/abs/2018PhRvD..98f2004A) | [data files](2018/2018PhRvD..98f2004A) |
|iron | Measurement of the iron spectrum in cosmic rays by VERITAS | [2018PhRvD..98b2009A](http://adsabs.harvard.edu/abs/2018PhRvD..98b2009A) | [data files](2018/2018PhRvD..98b2009A) |
|TeV J2032+4130 / VER J2031+415 | Periastron Observations of TeV Gamma-Ray Emission from a Binary System with a 50-year Period | [2018ApJ...867L..19A](http://adsabs.harvard.edu/abs/2018ApJ...867L..19A) | [data files](2018/2018ApJ...867L..19A) |
|PSR J2032+4127/MT91 213 / VER J2032+414 | Periastron Observations of TeV Gamma-Ray Emission from a Binary System with a 50-year Period | [2018ApJ...867L..19A](http://adsabs.harvard.edu/abs/2018ApJ...867L..19A) | [data files](2018/2018ApJ...867L..19A) |
|SNR G054.1+00.3 / VER J1930+188 | VERITAS and Fermi-LAT Observations of TeV Gamma-Ray Sources Discovered by HAWC in the 2HWC Catalog | [2018ApJ...866...24A](http://adsabs.harvard.edu/abs/2018ApJ...866...24A) | [data files](2018/2018ApJ...866...24A) |
|DA 495 / VER J1952+293 | VERITAS and Fermi-LAT Observations of TeV Gamma-Ray Sources Discovered by HAWC in the 2HWC Catalog | [2018ApJ...866...24A](http://adsabs.harvard.edu/abs/2018ApJ...866...24A) | [data files](2018/2018ApJ...866...24A) |
|HESS J1943+213 / VER J1943+213 | HESS J1943+213: An Extreme Blazar Shining through the Galactic Plane | [2018ApJ...862...41A](http://adsabs.harvard.edu/abs/2018ApJ...862...41A) | [data files](2018/2018ApJ...862...41A) |
|TXS 0506+056 / VER J0509+057 | VERITAS Observations of the BL Lac Object TXS 0506+056 | [2018ApJ...861L..20A](http://adsabs.harvard.edu/abs/2018ApJ...861L..20A) | [data files](2018/2018ApJ...861L..20A) |
|Gamma Cygni / VER J2019+407 | A Very High Energy γ-Ray Survey toward the Cygnus Region of the Galaxy | [2018ApJ...861..134A](http://adsabs.harvard.edu/abs/2018ApJ...861..134A) | [data files](2018/2018ApJ...861..134A) |
|TeV J2032+4130 / VER J2031+415 | A Very High Energy γ-Ray Survey toward the Cygnus Region of the Galaxy | [2018ApJ...861..134A](http://adsabs.harvard.edu/abs/2018ApJ...861..134A) | [data files](2018/2018ApJ...861..134A) |
|VER J2016+371 / VER J2016+371 | A Very High Energy γ-Ray Survey toward the Cygnus Region of the Galaxy | [2018ApJ...861..134A](http://adsabs.harvard.edu/abs/2018ApJ...861..134A) | [data files](2018/2018ApJ...861..134A) |
|VER J2019+368 / VER J2019+368 | A Very High Energy γ-Ray Survey toward the Cygnus Region of the Galaxy | [2018ApJ...861..134A](http://adsabs.harvard.edu/abs/2018ApJ...861..134A) | [data files](2018/2018ApJ...861..134A) |
|VER J2018+367 / VER J2018+367 | A Very High Energy γ-Ray Survey toward the Cygnus Region of the Galaxy | [2018ApJ...861..134A](http://adsabs.harvard.edu/abs/2018ApJ...861..134A) | [data files](2018/2018ApJ...861..134A) |
|VER J2020+368 / VER J2020+368 | A Very High Energy γ-Ray Survey toward the Cygnus Region of the Galaxy | [2018ApJ...861..134A](http://adsabs.harvard.edu/abs/2018ApJ...861..134A) | [data files](2018/2018ApJ...861..134A) |
|GRB 150323A | A Strong Limit on the Very-high-energy Emission from GRB 150323A | [2018ApJ...857...33A](http://adsabs.harvard.edu/abs/2018ApJ...857...33A) | [data files](2018/2018ApJ...857...33A) |
|BL Lacertae / VER J2202+422 | Multiwavelength Observations of the Blazar BL Lacertae: A New Fast TeV Gamma-Ray Flare | [2018ApJ...856...95A](http://adsabs.harvard.edu/abs/2018ApJ...856...95A) | [data files](2018/2018ApJ...856...95A) |
|Markarian 501 / VER J1653+397 | Extreme HBL behavior of Markarian 501 during 2012 | [2018A&A...620A.181A](http://adsabs.harvard.edu/abs/2018A&A...620A.181A) | [data files](2018/2018A&A...620A.181A) |
|Segue 1 | Dark matter constraints from a joint analysis of dwarf Spheroidal galaxy observations with VERITAS | [2017PhRvD..95h2001A](http://adsabs.harvard.edu/abs/2017PhRvD..95h2001A) | [data files](2017/2017PhRvD..95h2001A) |
|Draco | Dark matter constraints from a joint analysis of dwarf Spheroidal galaxy observations with VERITAS | [2017PhRvD..95h2001A](http://adsabs.harvard.edu/abs/2017PhRvD..95h2001A) | [data files](2017/2017PhRvD..95h2001A) |
|Ursa Minor | Dark matter constraints from a joint analysis of dwarf Spheroidal galaxy observations with VERITAS | [2017PhRvD..95h2001A](http://adsabs.harvard.edu/abs/2017PhRvD..95h2001A) | [data files](2017/2017PhRvD..95h2001A) |
|Bootes 1 | Dark matter constraints from a joint analysis of dwarf Spheroidal galaxy observations with VERITAS | [2017PhRvD..95h2001A](http://adsabs.harvard.edu/abs/2017PhRvD..95h2001A) | [data files](2017/2017PhRvD..95h2001A) |
|Willman 1 | Dark matter constraints from a joint analysis of dwarf Spheroidal galaxy observations with VERITAS | [2017PhRvD..95h2001A](http://adsabs.harvard.edu/abs/2017PhRvD..95h2001A) | [data files](2017/2017PhRvD..95h2001A) |
|1ES 2344+514 / VER J2347+517 | Very-High-Energy γ-Ray Observations of the Blazar 1ES 2344+514 with VERITAS | [2017MNRAS.471.2117A](http://adsabs.harvard.edu/abs/2017MNRAS.471.2117A) | [data files](2017/2017MNRAS.471.2117A) |
|HESS J0632+057 / VER J0633+057 | VHE Observations of Galactic binary systems with VERITAS | [2017ICRC...35..729M](http://adsabs.harvard.edu/abs/2017ICRC...35..729M) | [data files](2017/2017ICRC...35..729M) |
|LS I +61 303 / VER J0240+612 | Decadal VERITAS Observation of LS I +61°303: Detection of TeV emission around the entire orbit | [2017ICRC...35..712K](http://adsabs.harvard.edu/abs/2017ICRC...35..712K) | [data files](2017/2017ICRC...35..712K) |
| x | Discovery of Very-high-energy Emission from RGB J2243+203 and Derivation of Its Redshift Upper Limit | [2017ApJS..233....7A](http://adsabs.harvard.edu/abs/2017ApJS..233....7A) | [data files](2017/2017ApJS..233....7A) |
|1ES 1215+303 / VER J1217+301 | A Luminous and Isolated Gamma-ray Flare from the Blazar B2 1215+30 | [2017ApJ...836..205A](http://adsabs.harvard.edu/abs/2017ApJ...836..205A) | [data files](2017/2017ApJ...836..205A) |
|Tycho SNR / VER J0025+641 | Gamma-Ray Observations of Tycho’s Supernova Remnant with VERITAS and Fermi | [2017ApJ...836...23A](http://adsabs.harvard.edu/abs/2017ApJ...836...23A) | [data files](2017/2017ApJ...836...23A) |
| x | Search for Magnetically Broadened Cascade Emission from Blazars with VERITAS | [2017ApJ...835..288A](http://adsabs.harvard.edu/abs/2017ApJ...835..288A) | [data files](2017/2017ApJ...835..288A) |
|Markarian 421 / VER J1104+382 | A Search for Spectral Hysteresis and Energy-dependent Time Lags from X-Ray and TeV Gamma-Ray Observations of Mrk 421 | [2017ApJ...834....2A](http://adsabs.harvard.edu/abs/2017ApJ...834....2A) | [data files](2017/2017ApJ...834....2A) |
|Crab nebula / VER J0534+220 | Gamma-ray observations under bright moonlight with VERITAS | [2017APh....91...34A](http://adsabs.harvard.edu/abs/2017APh....91...34A) | [data files](2017/2017APh....91...34A) |
|HESS J0632+057 / VER J0633+057 | A decade of TeV observations of the gamma-ray binary HESS J0632+057 with VERITAS | [2017AIPC.1792d0023S](http://adsabs.harvard.edu/abs/2017AIPC.1792d0023S) | [data files](2017/2017AIPC.1792d0023S) |
|Markarian 501 / VER J1653+397 | Multiband variability studies and novel broadband SED modeling of Mrk 501 in 2009 | [2017A&A...603A..31A](http://adsabs.harvard.edu/abs/2017A&A...603A..31A) | [data files](2017/2017A&A...603A..31A) |
|1ES 1440+122 / VER J1443+120 | Discovery of very high energy gamma rays from 1ES 1440+122 | [2016MNRAS.461..202A](http://adsabs.harvard.edu/abs/2016MNRAS.461..202A) | [data files](2016/2016MNRAS.461..202A) |
|1ES 1741+196 / VER J1744+195 | VERITAS and multiwavelength observations of the BL Lacertae object 1ES 1741+196 | [2016MNRAS.459.2550A](http://adsabs.harvard.edu/abs/2016MNRAS.459.2550A) | [data files](2016/2016MNRAS.459.2550A) |
|LB 2136 | Very high-energy gamma-ray follow-up program using neutrino triggers from IceCube | [2016JInst..1111009I](http://adsabs.harvard.edu/abs/2016JInst..1111009I) | [data files](2016/2016JInst..1111009I) |
|PSR J1023+0038 | A Search for Very High Energy Gamma Rays from the Missing Link Binary Pulsar J1023+0038 with VERITAS | [2016ApJ...831..193A](http://adsabs.harvard.edu/abs/2016ApJ...831..193A) | [data files](2016/2016ApJ...831..193A) |
|V* V404 Cyg | Very High Energy Observations of the Binaries V 404 Cyg and 4U 0115+634 during Giant X-Ray Outbursts | [2016ApJ...831..113A](http://adsabs.harvard.edu/abs/2016ApJ...831..113A) | [data files](2016/2016ApJ...831..113A) |
|V* V635 Cas | Very High Energy Observations of the Binaries V 404 Cyg and 4U 0115+634 during Giant X-Ray Outbursts | [2016ApJ...831..113A](http://adsabs.harvard.edu/abs/2016ApJ...831..113A) | [data files](2016/2016ApJ...831..113A) |
|Galactic Centre / VER J1745-290 | TeV Gamma-Ray Observations of the Galactic Center Ridge by VERITAS | [2016ApJ...821..129A](http://adsabs.harvard.edu/abs/2016ApJ...821..129A) | [data files](2016/2016ApJ...821..129A) |
|SNR G0.9+0.1 / VER J1747-281 | TeV Gamma-Ray Observations of the Galactic Center Ridge by VERITAS | [2016ApJ...821..129A](http://adsabs.harvard.edu/abs/2016ApJ...821..129A) | [data files](2016/2016ApJ...821..129A) |
|VER J1746-289 / VER J1746-289 | TeV Gamma-Ray Observations of the Galactic Center Ridge by VERITAS | [2016ApJ...821..129A](http://adsabs.harvard.edu/abs/2016ApJ...821..129A) | [data files](2016/2016ApJ...821..129A) |
|Markarian 421 / VER J1104+382 | Multiwavelength Study of Quiescent States of Mrk 421 with Unprecedented Hard X-Ray Coverage Provided by NuSTAR in 2013 | [2016ApJ...819..156B](http://adsabs.harvard.edu/abs/2016ApJ...819..156B) | [data files](2016/2016ApJ...819..156B) |
| x | A Search for Brief Optical Flashes Associated with the SETI Target KIC 8462852 | [2016ApJ...818L..33A](http://adsabs.harvard.edu/abs/2016ApJ...818L..33A) | [data files](2016/2016ApJ...818L..33A) |
|LS I +61 303 / VER J0240+612 | Exceptionally Bright TeV Flares from the Binary LS I +61 303 | [2016ApJ...817L...7A](http://adsabs.harvard.edu/abs/2016ApJ...817L...7A) | [data files](2016/2016ApJ...817L...7A) |
| x | Upper Limits from Five Years of Blazar Observations with the VERITAS Cherenkov Telescopes | [2016AJ....151..142A](http://adsabs.harvard.edu/abs/2016AJ....151..142A) | [data files](2016/2016AJ....151..142A) |
|Markarian 501 / VER J1653+397 | Very high energy outburst of Markarian 501 in May 2009 | [2016A&A...594A..76A](http://adsabs.harvard.edu/abs/2016A&A...594A..76A) | [data files](2016/2016A&A...594A..76A) |
|PMN J0948+0022 | The most powerful flaring activity from the NLSy1 PMN J0948+0022 | [2015MNRAS.446.2456D](http://adsabs.harvard.edu/abs/2015MNRAS.446.2456D) | [data files](2015/2015MNRAS.446.2456D) |
|Crab nebula / VER J0534+220 | Six years of VERITAS observations of the Crab Nebula | [2015ICRC...34..792M](http://adsabs.harvard.edu/abs/2015ICRC...34..792M) | [data files](2015/2015ICRC...34..792M) |
|PKS 1441+25 / VER J1443+250 | Gamma-Rays from the Quasar PKS 1441+25: Story of an Escape | [2015ApJ...815L..22A](http://adsabs.harvard.edu/abs/2015ApJ...815L..22A) | [data files](2015/2015ApJ...815L..22A) |
|Markarian 501 / VER J1653+397 | First NuSTAR Observations of Mrk 501 within a Radio to TeV Multi-Instrument Campaign | [2015ApJ...812...65F](http://adsabs.harvard.edu/abs/2015ApJ...812...65F) | [data files](2015/2015ApJ...812...65F) |
|1ES 1727+502 / VER J1728+502 | VERITAS Detection of γ-Ray Flaring Activity From the BL Lac Object 1ES 1727+502 During Bright Moonlight Observations | [2015ApJ...808..110A](http://adsabs.harvard.edu/abs/2015ApJ...808..110A) | [data files](2015/2015ApJ...808..110A) |
|Geminga pulsar | A Search for Pulsations from Geminga above 100 GeV with VERITAS | [2015ApJ...800...61A](http://adsabs.harvard.edu/abs/2015ApJ...800...61A) | [data files](2015/2015ApJ...800...61A) |
|PG 1553+113 / VER J1555+111 | VERITAS Observations of the BL Lac Object PG 1553+113 | [2015ApJ...799....7A](http://adsabs.harvard.edu/abs/2015ApJ...799....7A) | [data files](2015/2015ApJ...799....7A) |
|Markarian 501 / VER J1653+397 | Multiwavelength observations of Mrk 501 in 2008 | [2015A&A...573A..50A](http://adsabs.harvard.edu/abs/2015A&A...573A..50A) | [data files](2015/2015A&A...573A..50A) |
|GRB 130427A | Constraints on Very High Energy Emission from GRB 130427A | [2014ApJ...795L...3A](http://adsabs.harvard.edu/abs/2014ApJ...795L...3A) | [data files](2014/2014ApJ...795L...3A) |
|Galactic Centre / VER J1745-290 | Very-high Energy Observations of the Galactic Center Region by VERITAS in 2010-2012 | [2014ApJ...790..149A](http://adsabs.harvard.edu/abs/2014ApJ...790..149A) | [data files](2014/2014ApJ...790..149A) |
|1ES 1218+304 / VER J1221+301 | Test of Models of the Cosmic Infrared Background with Multiwavelength Observations of the Blazar 1ES 1218+30.4 in 2009 | [2014ApJ...788..158A](http://adsabs.harvard.edu/abs/2014ApJ...788..158A) | [data files](2014/2014ApJ...788..158A) |
|VER J2016+371 / VER J2016+371 | Spatially Resolving the Very High Energy Emission from MGRO J2019+37 with VERITAS | [2014ApJ...788...78A](http://adsabs.harvard.edu/abs/2014ApJ...788...78A) | [data files](2014/2014ApJ...788...78A) |
|VER J2019+368 / VER J2019+368 | Spatially Resolving the Very High Energy Emission from MGRO J2019+37 with VERITAS | [2014ApJ...788...78A](http://adsabs.harvard.edu/abs/2014ApJ...788...78A) | [data files](2014/2014ApJ...788...78A) |
|MGRO J1908+06 / VER J1907+062 | Investigating the TeV Morphology of MGRO J1908+06 with VERITAS | [2014ApJ...787..166A](http://adsabs.harvard.edu/abs/2014ApJ...787..166A) | [data files](2014/2014ApJ...787..166A) |
|PKS 1424+240 / VER J1427+237 | Deep Broadband Observations of the Distant Gamma-Ray Blazar PKS 1424+240 | [2014ApJ...785L..16A](http://adsabs.harvard.edu/abs/2014ApJ...785L..16A) | [data files](2014/2014ApJ...785L..16A) |
|TeV J2032+4130 / VER J2031+415 | Observations of the Unidentified Gamma-Ray Source TeV J2032+4130 by VERITAS | [2014ApJ...783...16A](http://adsabs.harvard.edu/abs/2014ApJ...783...16A) | [data files](2014/2014ApJ...783...16A) |
|1ES 0229+200 / VER J0232+202 | A Three-year Multi-wavelength Study of the Very-high-energy γ-Ray Blazar 1ES 0229+200 | [2014ApJ...782...13A](http://adsabs.harvard.edu/abs/2014ApJ...782...13A) | [data files](2014/2014ApJ...782...13A) |
|Crab nebula / VER J0534+220 | A Search for Enhanced Very High Energy Gamma-Ray Emission from the 2013 March Crab Nebula Flare | [2014ApJ...781L..11A](http://adsabs.harvard.edu/abs/2014ApJ...781L..11A) | [data files](2014/2014ApJ...781L..11A) |
|HESS J0632+057 / VER J0633+057 | Long-term TeV and X-Ray Observations of the Gamma-Ray Binary HESS J0632+057 | [2014ApJ...780..168A](http://adsabs.harvard.edu/abs/2014ApJ...780..168A) | [data files](2014/2014ApJ...780..168A) |
|Cyg X-3 | VERITAS Observations of the Microquasar Cygnus X-3 | [2013ApJ...779..150A](http://adsabs.harvard.edu/abs/2013ApJ...779..150A) | [data files](2013/2013ApJ...779..150A) |
|1ES 1215+303 / VER J1217+301 | Long Term Observations of B2 1215+30 with VERITAS | [2013ApJ...779...92A](http://adsabs.harvard.edu/abs/2013ApJ...779...92A) | [data files](2013/2013ApJ...779...92A) |
|LS I +61 303 / VER J0240+612 | Multiwavelength Observations of the TeV Binary LS I +61° 303 with VERITAS, Fermi-LAT, and Swift/XRT during a TeV Outburst | [2013ApJ...779...88A](http://adsabs.harvard.edu/abs/2013ApJ...779...88A) | [data files](2013/2013ApJ...779...88A) |
|RGB J0521+212 / VER J0521+211 | Discovery of a New TeV Gamma-Ray Source: VER J0521+211 | [2013ApJ...776...69A](http://adsabs.harvard.edu/abs/2013ApJ...776...69A) | [data files](2013/2013ApJ...776...69A) |
|1ES 1959+650 / VER J1959+651 | Multiwavelength Observations and Modeling of 1ES 1959+650 in a Low Flux State | [2013ApJ...775....3A](http://adsabs.harvard.edu/abs/2013ApJ...775....3A) | [data files](2013/2013ApJ...775....3A) |
|Gamma Cygni / VER J2019+407 | Discovery of TeV Gamma-Ray Emission toward Supernova Remnant SNR G78.2+2.1 | [2013ApJ...770...93A](http://adsabs.harvard.edu/abs/2013ApJ...770...93A) | [data files](2013/2013ApJ...770...93A) |
|CTA 1 / VER J0006+729 | Discovery of TeV Gamma-Ray Emission from CTA 1 by VERITAS | [2013ApJ...764...38A](http://adsabs.harvard.edu/abs/2013ApJ...764...38A) | [data files](2013/2013ApJ...764...38A) |
|BL Lacertae / VER J2202+422 | Rapid TeV Gamma-Ray Flaring of BL Lacertae | [2013ApJ...762...92A](http://adsabs.harvard.edu/abs/2013ApJ...762...92A) | [data files](2013/2013ApJ...762...92A) |
|Segue 1 | VERITAS deep observations of the dwarf spheroidal galaxy Segue 1 | [2012PhRvD..85f2001A](http://adsabs.harvard.edu/abs/2012PhRvD..85f2001A) | [data files](2012/2012PhRvD..85f2001A) |
|Crab nebula / VER J0534+220 | Search for a Correlation between Very-high-energy Gamma Rays and Giant Radio Pulses in the Crab Pulsar | [2012ApJ...760..136A](http://adsabs.harvard.edu/abs/2012ApJ...760..136A) | [data files](2012/2012ApJ...760..136A) |
|RGB J0136+391 / VER J0136+390 | VERITAS Observations of Six Bright, Hard-spectrum Fermi-LAT Blazars | [2012ApJ...759..102A](http://adsabs.harvard.edu/abs/2012ApJ...759..102A) | [data files](2012/2012ApJ...759..102A) |
|RGB J0316+090 | VERITAS Observations of Six Bright, Hard-spectrum Fermi-LAT Blazars | [2012ApJ...759..102A](http://adsabs.harvard.edu/abs/2012ApJ...759..102A) | [data files](2012/2012ApJ...759..102A) |
|RGB J0909+231 | VERITAS Observations of Six Bright, Hard-spectrum Fermi-LAT Blazars | [2012ApJ...759..102A](http://adsabs.harvard.edu/abs/2012ApJ...759..102A) | [data files](2012/2012ApJ...759..102A) |
|RGB J1058+564 | VERITAS Observations of Six Bright, Hard-spectrum Fermi-LAT Blazars | [2012ApJ...759..102A](http://adsabs.harvard.edu/abs/2012ApJ...759..102A) | [data files](2012/2012ApJ...759..102A) |
|RGB J1243+364 | VERITAS Observations of Six Bright, Hard-spectrum Fermi-LAT Blazars | [2012ApJ...759..102A](http://adsabs.harvard.edu/abs/2012ApJ...759..102A) | [data files](2012/2012ApJ...759..102A) |
|RX J1436.9+5639 | VERITAS Observations of Six Bright, Hard-spectrum Fermi-LAT Blazars | [2012ApJ...759..102A](http://adsabs.harvard.edu/abs/2012ApJ...759..102A) | [data files](2012/2012ApJ...759..102A) |
|Coma Cluster | Constraints on Cosmic Rays, Magnetic Fields, and Dark Matter from Gamma-Ray Observations of the Coma Cluster of Galaxies with VERITAS and Fermi | [2012ApJ...757..123A](http://adsabs.harvard.edu/abs/2012ApJ...757..123A) | [data files](2012/2012ApJ...757..123A) |
|NGC 4889 | Constraints on Cosmic Rays, Magnetic Fields, and Dark Matter from Gamma-Ray Observations of the Coma Cluster of Galaxies with VERITAS and Fermi | [2012ApJ...757..123A](http://adsabs.harvard.edu/abs/2012ApJ...757..123A) | [data files](2012/2012ApJ...757..123A) |
|NGC 4874 | Constraints on Cosmic Rays, Magnetic Fields, and Dark Matter from Gamma-Ray Observations of the Coma Cluster of Galaxies with VERITAS and Fermi | [2012ApJ...757..123A](http://adsabs.harvard.edu/abs/2012ApJ...757..123A) | [data files](2012/2012ApJ...757..123A) |
|NGC 4921 | Constraints on Cosmic Rays, Magnetic Fields, and Dark Matter from Gamma-Ray Observations of the Coma Cluster of Galaxies with VERITAS and Fermi | [2012ApJ...757..123A](http://adsabs.harvard.edu/abs/2012ApJ...757..123A) | [data files](2012/2012ApJ...757..123A) |
|1ES 0414+009 / VER J0416+011 | Multiwavelength Observations of the AGN 1ES 0414+009 with VERITAS, Fermi-LAT, Swift-XRT, and MDM | [2012ApJ...755..118A](http://adsabs.harvard.edu/abs/2012ApJ...755..118A) | [data files](2012/2012ApJ...755..118A) |
|V407 Cyg | VERITAS Observations of the Nova in V407 Cygni | [2012ApJ...754...77A](http://adsabs.harvard.edu/abs/2012ApJ...754...77A) | [data files](2012/2012ApJ...754...77A) |
|RBS 0413 / VER J0319+187 | Discovery of High-energy and Very High Energy γ-Ray Emission from the Blazar RBS 0413 | [2012ApJ...750...94A](http://adsabs.harvard.edu/abs/2012ApJ...750...94A) | [data files](2012/2012ApJ...750...94A) |
|M 87 / VER J1230+123 | The 2010 Very High Energy γ-Ray Flare and 10 Years of Multi-wavelength Observations of M 87 | [2012ApJ...746..151A](http://adsabs.harvard.edu/abs/2012ApJ...746..151A) | [data files](2012/2012ApJ...746..151A) |
|M 87 / VER J1230+123 | VERITAS Observations of Day-scale Flaring of M 87 in 2010 April | [2012ApJ...746..141A](http://adsabs.harvard.edu/abs/2012ApJ...746..141A) | [data files](2012/2012ApJ...746..141A) |
|Crab pulsar / VER J0534+220 | Detection of Pulsed Gamma Rays Above 100 GeV from the Crab Pulsar | [2011Sci...334...69V](http://adsabs.harvard.edu/abs/2011Sci...334...69V) | [data files](2011/2011Sci...334...69V) |
| x | VERITAS Observations of Gamma-Ray Bursts Detected by Swift | [2011ApJ...743...62A](http://adsabs.harvard.edu/abs/2011ApJ...743...62A) | [data files](2011/2011ApJ...743...62A) |
|RX J0648.7+1516 / VER J0648+152 | Multiwavelength Observations of the Previously Unidentified Blazar RX J0648.7+1516 | [2011ApJ...742..127A](http://adsabs.harvard.edu/abs/2011ApJ...742..127A) | [data files](2011/2011ApJ...742..127A) |
|SWIFT J164449.3+573451 | VERITAS Observations of the Unusual Extragalactic Transient Swift J164449.3+573451 | [2011ApJ...738L..30A](http://adsabs.harvard.edu/abs/2011ApJ...738L..30A) | [data files](2011/2011ApJ...738L..30A) |
|1ES 2344+514 / VER J2347+517 | Multiwavelength Observations of the Very High Energy Blazar 1ES 2344+514 | [2011ApJ...738..169A](http://adsabs.harvard.edu/abs/2011ApJ...738..169A) | [data files](2011/2011ApJ...738..169A) |
|Markarian 421 / VER J1104+382 | TeV and Multi-wavelength Observations of Mrk 421 in 2006-2008 | [2011ApJ...738...25A](http://adsabs.harvard.edu/abs/2011ApJ...738...25A) | [data files](2011/2011ApJ...738...25A) |
|LS I +61 303 / VER J0240+612 | VERITAS Observations of the TeV Binary LS I +61° 303 During 2008-2010 | [2011ApJ...738....3A](http://adsabs.harvard.edu/abs/2011ApJ...738....3A) | [data files](2011/2011ApJ...738....3A) |
|1A 0535+262 | Gamma-Ray Observations of the Be/Pulsar Binary 1A 0535+262 During a Giant X-Ray Outburst | [2011ApJ...733...96A](http://adsabs.harvard.edu/abs/2011ApJ...733...96A) | [data files](2011/2011ApJ...733...96A) |
|Tycho SNR / VER J0025+641 | Discovery of TeV Gamma-ray Emission from Tycho's Supernova Remnant | [2011ApJ...730L..20A](http://adsabs.harvard.edu/abs/2011ApJ...730L..20A) | [data files](2011/2011ApJ...730L..20A) |
|Markarian 501 / VER J1653+397 | Spectral Energy Distribution of Markarian 501: Quiescent State Versus Extreme Outburst | [2011ApJ...729....2A](http://adsabs.harvard.edu/abs/2011ApJ...729....2A) | [data files](2011/2011ApJ...729....2A) |
|Markarian 501 / VER J1653+397 | Insights into the High-energy γ-ray Emission of Markarian 501 from Extensive Multifrequency Observations in the Fermi Era | [2011ApJ...727..129A](http://adsabs.harvard.edu/abs/2011ApJ...727..129A) | [data files](2011/2011ApJ...727..129A) |
|3C 66A / VER J0222+430 | Multi-wavelength Observations of the Flaring Gamma-ray Blazar 3C 66A in 2008 October | [2011ApJ...726...43A](http://adsabs.harvard.edu/abs/2011ApJ...726...43A) | [data files](2011/2011ApJ...726...43A) |
|Draco | VERITAS Search for VHE Gamma-ray Emission from Dwarf Spheroidal Galaxies | [2010ApJ...720.1174A](http://adsabs.harvard.edu/abs/2010ApJ...720.1174A) | [data files](2010/2010ApJ...720.1174A) |
|Ursa Minor | VERITAS Search for VHE Gamma-ray Emission from Dwarf Spheroidal Galaxies | [2010ApJ...720.1174A](http://adsabs.harvard.edu/abs/2010ApJ...720.1174A) | [data files](2010/2010ApJ...720.1174A) |
|Bootes 1 | VERITAS Search for VHE Gamma-ray Emission from Dwarf Spheroidal Galaxies | [2010ApJ...720.1174A](http://adsabs.harvard.edu/abs/2010ApJ...720.1174A) | [data files](2010/2010ApJ...720.1174A) |
|Willman 1 | VERITAS Search for VHE Gamma-ray Emission from Dwarf Spheroidal Galaxies | [2010ApJ...720.1174A](http://adsabs.harvard.edu/abs/2010ApJ...720.1174A) | [data files](2010/2010ApJ...720.1174A) |
|SNR G054.1+00.3 / VER J1930+188 | Discovery of Very High Energy γ-ray Emission from the SNR G54.1+0.3 | [2010ApJ...719L..69A](http://adsabs.harvard.edu/abs/2010ApJ...719L..69A) | [data files](2010/2010ApJ...719L..69A) |
|M 87 / VER J1230+123 | Veritas 2008-2009 Monitoring of the Variable Gamma-ray Source M 87 | [2010ApJ...716..819A](http://adsabs.harvard.edu/abs/2010ApJ...716..819A) | [data files](2010/2010ApJ...716..819A) |
|RGB J0710+591 / VER J0710+591 | The Discovery of γ-Ray Emission from the Blazar RGB J0710+591 | [2010ApJ...715L..49A](http://adsabs.harvard.edu/abs/2010ApJ...715L..49A) | [data files](2010/2010ApJ...715L..49A) |
|Cassiopeia A / VER J2323+588 | Observations of the Shell-type Supernova Remnant Cassiopeia A at TeV Energies with VERITAS | [2010ApJ...714..163A](http://adsabs.harvard.edu/abs/2010ApJ...714..163A) | [data files](2010/2010ApJ...714..163A) |
|1ES 1218+304 / VER J1221+301 | Discovery of Variability in the Very High Energy γ-Ray Emission of 1ES 1218+304 with VERITAS | [2010ApJ...709L.163A](http://adsabs.harvard.edu/abs/2010ApJ...709L.163A) | [data files](2010/2010ApJ...709L.163A) |
|PKS 1424+240 / VER J1427+237 | Discovery of Very High Energy Gamma Rays from PKS 1424+240 and Multiwavelength Constraints on Its Redshift | [2010ApJ...708L.100A](http://adsabs.harvard.edu/abs/2010ApJ...708L.100A) | [data files](2010/2010ApJ...708L.100A) |
|M 87 / VER J1230+123 | Radio Imaging of the Very-High-Energy γ-Ray Emission Region in the Central Engine of a Radio Galaxy | [2009Sci...325..444A](http://adsabs.harvard.edu/abs/2009Sci...325..444A) | [data files](2009/2009Sci...325..444A) |
|M 82 / VER J0955+696 | A connection between star formation activity and cosmic rays in the starburst galaxy M82 | [2009Natur.462..770V](http://adsabs.harvard.edu/abs/2009Natur.462..770V) | [data files](2009/2009Natur.462..770V) |
|W Comae / VER J1221+282 | Multiwavelength Observations of a TeV-Flare from W Comae | [2009ApJ...707..612A](http://adsabs.harvard.edu/abs/2009ApJ...707..612A) | [data files](2009/2009ApJ...707..612A) |
|NGC 1275 / VER J0319+415 | VERITAS Upper Limit on the Very High Energy Emission from the Radio Galaxy NGC 1275 | [2009ApJ...706L.275A](http://adsabs.harvard.edu/abs/2009ApJ...706L.275A) | [data files](2009/2009ApJ...706L.275A) |
|SNR G106.3+02.7 / VER J2227+608 | Detection of Extended VHE Gamma Ray Emission from G106.3+2.7 with Veritas | [2009ApJ...703L...6A](http://adsabs.harvard.edu/abs/2009ApJ...703L...6A) | [data files](2009/2009ApJ...703L...6A) |
|Markarian 421 / VER J1104+382 | Simultaneous Multiwavelength Observations of Markarian 421 During Outburst | [2009ApJ...703..169A](http://adsabs.harvard.edu/abs/2009ApJ...703..169A) | [data files](2009/2009ApJ...703..169A) |
|LS I +61 303 / VER J0240+612 | Multiwavelength Observations of LS I +61° 303 with Veritas, Swift, and RXTE | [2009ApJ...700.1034A](http://adsabs.harvard.edu/abs/2009ApJ...700.1034A) | [data files](2009/2009ApJ...700.1034A) |
|IC 443 / VER J0616+223 | Observation of Extended Very High Energy Emission from the Supernova Remnant IC 443 with VERITAS | [2009ApJ...698L.133A](http://adsabs.harvard.edu/abs/2009ApJ...698L.133A) | [data files](2009/2009ApJ...698L.133A) |
|HESS J0632+057 / VER J0633+057 | Evidence for Long-Term Gamma-Ray and X-Ray Variability from the Unidentified TeV Source HESS J0632+057 | [2009ApJ...698L..94A](http://adsabs.harvard.edu/abs/2009ApJ...698L..94A) | [data files](2009/2009ApJ...698L..94A) |
|1ES 1218+304 / VER J1221+301 | VERITAS Observations of the BL Lac Object 1ES 1218+304 | [2009ApJ...695.1370A](http://adsabs.harvard.edu/abs/2009ApJ...695.1370A) | [data files](2009/2009ApJ...695.1370A) |
|3C 66A / VER J0222+430 | Veritas Observations of a Very High Energy γ-Ray Flare From the Blazar 3C 66A | [2009ApJ...693L.104A](http://adsabs.harvard.edu/abs/2009ApJ...693L.104A) | [data files](2009/2009ApJ...693L.104A) |
|Markarian 421 / VER J1104+382 | The June 2008 Flare of Markarian 421 from Optical to TeV Energies | [2009ApJ...691L..13D](http://adsabs.harvard.edu/abs/2009ApJ...691L..13D) | [data files](2009/2009ApJ...691L..13D) |
|1ES 0806+524 / VER J0809+523 | Discovery of Very High Energy Gamma-ray Radiation from the BL Lac 1ES 0806+524 | [2009ApJ...690L.126A](http://adsabs.harvard.edu/abs/2009ApJ...690L.126A) | [data files](2009/2009ApJ...690L.126A) |
|W Comae / VER J1221+282 | VERITAS Discovery of &gt;200 GeV Gamma-Ray Emission from the Intermediate-Frequency-Peaked BL Lacertae Object W Comae | [2008ApJ...684L..73A](http://adsabs.harvard.edu/abs/2008ApJ...684L..73A) | [data files](2008/2008ApJ...684L..73A) |
|LS I +61 303 / VER J0240+612 | VERITAS Observations of the γ-Ray Binary LS I +61 303 | [2008ApJ...679.1427A](http://adsabs.harvard.edu/abs/2008ApJ...679.1427A) | [data files](2008/2008ApJ...679.1427A) |
|M 87 / VER J1230+123 | Observation of Gamma-Ray Emission from the Galaxy M87 above 250 GeV with VERITAS | [2008ApJ...679..397A](http://adsabs.harvard.edu/abs/2008ApJ...679..397A) | [data files](2008/2008ApJ...679..397A) |

<a name="sources"></a>
# Source and Target List

| ID | VERITAS Name | Common Name | ra (deg) | dec (deg) | Reference(s) |
|:--|:--|:--|:--|:--|:--|
| 1 | VER J0006+729 | CTA 1 | 1.65 | 72.783 | [2013ApJ...764...38A](2013/2013ApJ...764...38A)
| 3 | VER J0025+641 | Tycho SNR | 6.3397 | 64.1408 | [2017ApJ...836...23A](2017/2017ApJ...836...23A),[2011ApJ...730L..20A](2011/2011ApJ...730L..20A)
| 7 | VER J0136+390 | RGB J0136+391 | 24.1358267 | 39.0997773 | [2012ApJ...759..102A](2012/2012ApJ...759..102A)
| 11 | VER J0222+430 | 3C 66A | 35.66505 | 43.0355222 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2011ApJ...726...43A](2011/2011ApJ...726...43A),[2009ApJ...693L.104A](2009/2009ApJ...693L.104A)
| 13 | VER J0232+202 | 1ES 0229+200 | 38.202564 | 20.2881899 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2014ApJ...782...13A](2014/2014ApJ...782...13A)
| 14 | VER J0240+612 | LS I +61 303 | 40.131938163 | 61.229336515 | [2017ICRC...35..712K](2017/2017ICRC...35..712K),[2016ApJ...817L...7A](2016/2016ApJ...817L...7A),[2013ApJ...779...88A](2013/2013ApJ...779...88A),[2011ApJ...738....3A](2011/2011ApJ...738....3A),[2009ApJ...700.1034A](2009/2009ApJ...700.1034A),[2008ApJ...679.1427A](2008/2008ApJ...679.1427A)
| 17 | VER J0319+187 | RBS 0413 | 49.96585 | 18.7595556 | [2012ApJ...750...94A](2012/2012ApJ...750...94A)
| 18 | VER J0319+415 | NGC 1275 | 49.950667083 | 41.511695306 | [2009ApJ...706L.275A](2009/2009ApJ...706L.275A)
| 20 | VER J0416+011 | 1ES 0414+009 | 64.2187375 | 1.0899944 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2012ApJ...755..118A](2012/2012ApJ...755..118A)
| 22 | VER J0507+676 | 1ES 0502+675 | 76.9840583 | 67.6234056 | [2019ApJ...885..150A](2019/2019ApJ...885..150A)
| 23 | VER J0521+211 | RGB J0521+212 | 80.4415375 | 21.2142722 | [2013ApJ...776...69A](2013/2013ApJ...776...69A)
| 25 | VER J0534+220 | Crab nebula | 83.633083 | 22.0145 | [2021arXiv211104676A](2021/2021arXiv211104676A),[2017APh....91...34A](2017/2017APh....91...34A),[2015ICRC...34..792M](2015/2015ICRC...34..792M),[2014ApJ...781L..11A](2014/2014ApJ...781L..11A),[2012ApJ...760..136A](2012/2012ApJ...760..136A)
| 29 | VER J0616+223 | IC 443 | 94.51125 | 22.66 | [2009ApJ...698L.133A](2009/2009ApJ...698L.133A)
| 30 | VER J0633+057 | HESS J0632+057 | 98.24689375 | 5.80032722 | [2021ApJ...923..241A](2021/2021ApJ...923..241A),[2021ApJ...923...17T](2021/2021ApJ...923...17T),[2020ApJ...888..115A](2020/2020ApJ...888..115A),[2017AIPC.1792d0023S](2017/2017AIPC.1792d0023S),[2017ICRC...35..729M](2017/2017ICRC...35..729M),[2014ApJ...780..168A](2014/2014ApJ...780..168A),[2009ApJ...698L..94A](2009/2009ApJ...698L..94A)
| 32 | VER J0648+152 | RX J0648.7+1516 | 102.1984875 | 15.2735722 | [2011ApJ...742..127A](2011/2011ApJ...742..127A)
| 34 | VER J0710+591 | RGB J0710+591 | 107.625325 | 59.1390278 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2010ApJ...715L..49A](2010/2010ApJ...715L..49A)
| 36 | VER J0809+523 | 1ES 0806+524 | 122.454944708 | 52.31618075 | [2009ApJ...690L.126A](2009/2009ApJ...690L.126A)
| 40 | VER J0955+696 | M 82 | 148.9684583 | 69.6797028 | [2009Natur.462..770V](2009/2009Natur.462..770V)
| 43 | VER J1015+494 | 1ES 1011+496 | 153.767249167 | 49.433529083 | [2019ApJ...885..150A](2019/2019ApJ...885..150A)
| 49 | VER J1104+382 | Markarian 421 | 166.113808083 | 38.208833083 | [2020ApJ...890...97A](2020/2020ApJ...890...97A),[2017ApJ...834....2A](2017/2017ApJ...834....2A),[2016ApJ...819..156B](2016/2016ApJ...819..156B),[2011ApJ...738...25A](2011/2011ApJ...738...25A),[2009ApJ...691L..13D](2009/2009ApJ...691L..13D),[2009ApJ...703..169A](2009/2009ApJ...703..169A)
| 53 | VER J1217+301 | 1ES 1215+303 | 184.46700833 | 30.11684333 | [2020ApJ...891..170V](2020/2020ApJ...891..170V),[2019ApJ...885..150A](2019/2019ApJ...885..150A),[2017ApJ...836..205A](2017/2017ApJ...836..205A),[2013ApJ...779...92A](2013/2013ApJ...779...92A)
| 54 | VER J1221+282 | W Comae | 185.382043833 | 28.232916722 | [2009ApJ...707..612A](2009/2009ApJ...707..612A),[2008ApJ...684L..73A](2008/2008ApJ...684L..73A)
| 55 | VER J1221+301 | 1ES 1218+304 | 185.3414278125 | 30.1769891083 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2014ApJ...788..158A](2014/2014ApJ...788..158A),[2010ApJ...709L.163A](2010/2010ApJ...709L.163A),[2009ApJ...695.1370A](2009/2009ApJ...695.1370A)
| 57 | VER J1224+246 | MS1221.8+2452 | 186.100775925 | 24.6065282556 | [2019ApJ...885..150A](2019/2019ApJ...885..150A)
| 58 | VER J1230+123 | M 87 | 187.70593075 | 12.391123306 | [2021ApJ...911L..11E](2021/2021ApJ...911L..11E),[2012ApJ...746..151A](2012/2012ApJ...746..151A),[2012ApJ...746..141A](2012/2012ApJ...746..141A),[2010ApJ...716..819A](2010/2010ApJ...716..819A),[2009Sci...325..444A](2009/2009Sci...325..444A),[2008ApJ...679..397A](2008/2008ApJ...679..397A)
| 67 | VER J1427+237 | PKS 1424+240 | 216.751632458 | 23.800010444 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2014ApJ...785L..16A](2014/2014ApJ...785L..16A),[2010ApJ...708L.100A](2010/2010ApJ...708L.100A)
| 69 | VER J1428+426 | H 1426+428 | 217.1358706208 | 42.6725130889 | [2019ApJ...885..150A](2019/2019ApJ...885..150A)
| 71 | VER J1443+120 | 1ES 1440+122 | 220.701152425 | 12.0112152417 | [2016MNRAS.461..202A](2016/2016MNRAS.461..202A)
| 82 | VER J1555+111 | PG 1553+113 | 238.92935 | 11.19010167 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2015ApJ...799....7A](2015/2015ApJ...799....7A)
| 91 | VER J1653+397 | Markarian 501 | 253.4675695 | 39.760169139 | [2018A&A...620A.181A](2018/2018A&A...620A.181A),[2017A&A...603A..31A](2017/2017A&A...603A..31A),[2016A&A...594A..76A](2016/2016A&A...594A..76A),[2015A&A...573A..50A](2015/2015A&A...573A..50A),[2015ApJ...812...65F](2015/2015ApJ...812...65F),[2011ApJ...729....2A](2011/2011ApJ...729....2A),[2011ApJ...727..129A](2011/2011ApJ...727..129A)
| 101 | VER J1728+502 | 1ES 1727+502 | 262.07759958 | 50.219575 | [2015ApJ...808..110A](2015/2015ApJ...808..110A)
| 105 | VER J1744+195 | 1ES 1741+196 | 265.99096917 | 19.58583806 | [2016MNRAS.459.2550A](2016/2016MNRAS.459.2550A)
| 106 | VER J1745-290 | Galactic Centre | 266.416833 | -29.007806 | [2021ApJ...913..115A](2021/2021ApJ...913..115A),[2016ApJ...821..129A](2016/2016ApJ...821..129A),[2014ApJ...790..149A](2014/2014ApJ...790..149A)
| 110 | VER J1747-281 | SNR G0.9+0.1 | 266.825 | -28.15 | [2021ApJ...913..115A](2021/2021ApJ...913..115A),[2016ApJ...821..129A](2016/2016ApJ...821..129A)
| 118 | VER J1825-138 | HESS J1825-137 | 276.55441 | -13.58004 | [2020APh...11702403A](2020/2020APh...11702403A)
| 119 | VER J1826-148 | LS 5039 | 276.5627375 | -14.8484056 | [2020APh...11702403A](2020/2020APh...11702403A)
| 132 | VER J1907+062 | MGRO J1908+06 | 287.175 | 6.183 | [2014ApJ...787..166A](2014/2014ApJ...787..166A)
| 136 | VER J1930+188 | SNR G054.1+00.3 | 292.6292 | 18.867 | [2018ApJ...866...24A](2018/2018ApJ...866...24A),[2010ApJ...719L..69A](2010/2010ApJ...719L..69A)
| 137 | VER J1943+213 | HESS J1943+213 | 295.9792 | 21.30222 | [2018ApJ...862...41A](2018/2018ApJ...862...41A)
| 138 | VER J1959+651 | 1ES 1959+650 | 299.99938375 | 65.14851472 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2013ApJ...775....3A](2013/2013ApJ...775....3A)
| 141 | VER J2016+371 | VER J2016+371 | 304.0076 | 37.21476 | [2018ApJ...861..134A](2018/2018ApJ...861..134A),[2014ApJ...788...78A](2014/2014ApJ...788...78A)
| 143 | VER J2019+368 | VER J2019+368 | 304.0083 | 37.19778 | [2018ApJ...861..134A](2018/2018ApJ...861..134A),[2014ApJ...788...78A](2014/2014ApJ...788...78A)
| 144 | VER J2019+407 | Gamma Cygni | 305.557090982 | 40.256679158 | [2018ApJ...861..134A](2018/2018ApJ...861..134A),[2013ApJ...770...93A](2013/2013ApJ...770...93A)
| 146 | VER J2031+415 | TeV J2032+4130 | 308.025 | 41.567 | [2018ApJ...861..134A](2018/2018ApJ...861..134A),[2018ApJ...867L..19A](2018/2018ApJ...867L..19A),[2014ApJ...783...16A](2014/2014ApJ...783...16A)
| 148 | VER J2202+422 | BL Lacertae | 330.680380792 | 42.277772306 | [2018ApJ...856...95A](2018/2018ApJ...856...95A),[2013ApJ...762...92A](2013/2013ApJ...762...92A)
| 149 | VER J2227+608 | SNR G106.3+02.7 | 336.88 | 60.83 | [2009ApJ...703L...6A](2009/2009ApJ...703L...6A)
| 153 | VER J2323+588 | Cassiopeia A | 350.85 | 58.815 | [2020ApJ...894...51A](2020/2020ApJ...894...51A),[2010ApJ...714..163A](2010/2010ApJ...714..163A)
| 154 | VER J2347+517 | 1ES 2344+514 | 356.770153 | 51.704967 | [2019ApJ...885..150A](2019/2019ApJ...885..150A),[2017MNRAS.471.2117A](2017/2017MNRAS.471.2117A),[2011ApJ...738..169A](2011/2011ApJ...738..169A)
| 165 | VER J1746-289 | VER J1746-289 | 266.5821 | -28.966226 | [2021ApJ...913..115A](2021/2021ApJ...913..115A),[2016ApJ...821..129A](2016/2016ApJ...821..129A)
| 166 | VER J0534+220 | Crab pulsar | 83.63307625 | 22.014493278 | [2011Sci...334...69V](2011/2011Sci...334...69V)
| 167 | VER J1443+250 | PKS 1441+25 | 220.987051 | 25.029025 | [2015ApJ...815L..22A](2015/2015ApJ...815L..22A)
| 168 | VER J0509+057 | TXS 0506+056 | 77.358186 | 5.693148 | [2018Sci...361.1378I](2018/2018Sci...361.1378I),[2018ApJ...861L..20A](2018/2018ApJ...861L..20A)
| 170 | VER J2018+367 | VER J2018+367 | 304.5 | 36.7 | [2018ApJ...861..134A](2018/2018ApJ...861..134A)
| 171 | VER J2020+368 | VER J2020+368 | 305.0 | 36.8 | [2018ApJ...861..134A](2018/2018ApJ...861..134A)
| 172 | VER J1952+293 | DA 495 | 298.05708 | 29.41889 | [2018ApJ...866...24A](2018/2018ApJ...866...24A)
| 173 | VER J1145+196 | 3C 264.0 | 176.270871 | 19.606317 | [2020ApJ...896...41A](2020/2020ApJ...896...41A)
| 174 | VER J2032+414 | PSR J2032+4127/MT91 213 | 308.054687 | 41.456762 | [2018ApJ...867L..19A](2018/2018ApJ...867L..19A)
| 175 | VER J1746-286 | GC diffuse ridge | 308.054687 | 41.456762 | [2021ApJ...913..115A](2021/2021ApJ...913..115A)
| 100168 | (not detected) | V* V404 Cyg | 306.015917 | 33.867194 | [2016ApJ...831..113A](2016/2016ApJ...831..113A)
| 100169 | (not detected) | V* V635 Cas | 19.6325 | 63.7425 | [2016ApJ...831..113A](2016/2016ApJ...831..113A)
| 100171 | (not detected) | Cyg X-3 | 308.10742 | 40.95775 | [2013ApJ...779..150A](2013/2013ApJ...779..150A)
| 100172 | (not detected) | GRB 150323A | 128.178083 | 45.464639 | [2018ApJ...857...33A](2018/2018ApJ...857...33A)
| 100173 | (not detected) | Segue 1 | 151.7633 | 16.0736 | [2017PhRvD..95h2001A](2017/2017PhRvD..95h2001A),[2012PhRvD..85f2001A](2012/2012PhRvD..85f2001A)
| 100174 | (not detected) | Draco | 260.059728 | 57.921219 | [2017PhRvD..95h2001A](2017/2017PhRvD..95h2001A),[2010ApJ...720.1174A](2010/2010ApJ...720.1174A)
| 100175 | (not detected) | Ursa Minor | 227.29725 | 67.214361 | [2017PhRvD..95h2001A](2017/2017PhRvD..95h2001A),[2010ApJ...720.1174A](2010/2010ApJ...720.1174A)
| 100176 | (not detected) | Bootes 1 | 210.0 | 14.5 | [2017PhRvD..95h2001A](2017/2017PhRvD..95h2001A),[2010ApJ...720.1174A](2010/2010ApJ...720.1174A)
| 100177 | (not detected) | Willman 1 | 162.3375 | 51.05 | [2017PhRvD..95h2001A](2017/2017PhRvD..95h2001A),[2010ApJ...720.1174A](2010/2010ApJ...720.1174A)
| 100178 | (not detected) | PSR J1023+0038 | 155.948683 | 0.644724 | [2016ApJ...831..193A](2016/2016ApJ...831..193A)
| 100179 | (not detected) | LB 2136 | 178.351944 | 49.51912 | [2016JInst..1111009I](2016/2016JInst..1111009I)
| 100180 | (not detected) | Geminga pulsar | 98.4756375 | 17.7702528 | [2015ApJ...800...61A](2015/2015ApJ...800...61A)
| 100181 | (not detected) | PMN J0948+0022 | 147.238835 | 0.373767 | [2015MNRAS.446.2456D](2015/2015MNRAS.446.2456D)
| 100182 | (not detected) | GRB 130427A | 173.139 | 27.692 | [2014ApJ...795L...3A](2014/2014ApJ...795L...3A)
| 100183 | (not detected) | V407 Cyg | 315.540906 | 45.77576 | [2012ApJ...754...77A](2012/2012ApJ...754...77A)
| 100184 | (not detected) | Coma Cluster | 194.95291667 | 27.98055556 | [2012ApJ...757..123A](2012/2012ApJ...757..123A)
| 100185 | (not detected) | NGC 4889 | 195.0337375 | 27.977025 | [2012ApJ...757..123A](2012/2012ApJ...757..123A)
| 100186 | (not detected) | NGC 4874 | 194.8987875 | 27.95938889 | [2012ApJ...757..123A](2012/2012ApJ...757..123A)
| 100187 | (not detected) | NGC 4921 | 195.35884167 | 27.88600861 | [2012ApJ...757..123A](2012/2012ApJ...757..123A)
| 100189 | (not detected) | 1A 0535+262 | 84.727396 | 26.315789 | [2011ApJ...733...96A](2011/2011ApJ...733...96A)
| 100190 | (not detected) | SWIFT J164449.3+573451 | 251.205 | 57.581 | [2011ApJ...738L..30A](2011/2011ApJ...738L..30A)
| 100191 | (not detected) | RGB J0316+090 | 49.053054 | 9.078744 | [2012ApJ...759..102A](2012/2012ApJ...759..102A)
| 100192 | (not detected) | RGB J0909+231 | 137.252606 | 23.186938 | [2012ApJ...759..102A](2012/2012ApJ...759..102A)
| 100193 | (not detected) | RGB J1058+564 | 164.657199 | 56.46978 | [2012ApJ...759..102A](2012/2012ApJ...759..102A)
| 100194 | (not detected) | RGB J1243+364 | 190.803067 | 36.462222 | [2012ApJ...759..102A](2012/2012ApJ...759..102A)
| 100195 | (not detected) | RX J1436.9+5639 | 219.240498 | 56.656905 | [2012ApJ...759..102A](2012/2012ApJ...759..102A)
| 100196 | (not detected) | PSR B0355+54 | 59.723819 | 54.22048 | [2021ApJ...916..117B](2021/2021ApJ...916..117B)
| 100197 | (not detected) | PSR J0357+32 | 59.467338 | 32.089897 | [2021ApJ...916..117B](2021/2021ApJ...916..117B)
| 100198 | (not detected) | PSR J1740+1000 | 265.10794 | 10.00168 | [2021ApJ...916..117B](2021/2021ApJ...916..117B)
| 100199 | (not detected) | 3C 279 | 194.046527 | -5.789314 | [2021arXiv211013181A](2021/2021arXiv211013181A)
| 100200 | (not detected) | PKS 1222+216 | 186.22691 | 21.379551 | [2021arXiv211013181A](2021/2021arXiv211013181A)
| 100201 | (not detected) | Ton 599 | 179.882641 | 29.245507 | [2021arXiv211013181A](2021/2021arXiv211013181A)
| 300000 | (charged particle) | electron | 179.882641 | 29.245507 | [2018PhRvD..98f2004A](2018/2018PhRvD..98f2004A)
| 300026 | (charged particle) | iron | 179.882641 | 29.245507 | [2018PhRvD..98b2009A](2018/2018PhRvD..98b2009A)

<a name="licence"></a>

## Licence

Please cite this work: https://doi.org/10.5281/zenodo.4723219

<p xmlns:dct="http://purl.org/dc/terms/">
  <a rel="license"
     href="http://creativecommons.org/publicdomain/zero/1.0/">
    <img src="http://i.creativecommons.org/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
  </a>
  <br />
  To the extent possible under law,
  <span rel="dct:publisher" resource="[_:publisher]">the persons who associated CC0</span>
  with this work have waived all copyright and related or neighboring
  rights to this work.
</p>
