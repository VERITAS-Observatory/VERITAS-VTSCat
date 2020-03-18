# Objects - TeV Sources

Description files for objects (*TeV sources*) in the VERITAS catalogue. 

Following the gamma-cat sheme without any format changes [1]. Many files are modified copies from gamma-cat. The number of objects has been extented compared to gamma-cat and discrepencies in the *source_id* descriptor is expected for numbers 169. 

## File structure

- one YAML file per object in the format `<source_id>.yaml`.
- non-detection (observations only) are indicated by source IDs > 100000
- cosmic-ray observations are indicated by source IDs > 300000

## File format

The following entries are required:

- *source_id*: unique identifier of an object (integer)
- *common_name*: common name as usually used in literature
- *gamma_name*: VER name (also MAGIC and HESS name)
- *pos*: position information from SIMBAD
  - *simbad_id*: SIMBAD name
  - *ra*, *dec*: J2000 coordinates from SIMBAD

All other entries in the object files are optional. Note that the lists of references (*reference_id*), the lists of names (*fermi_names*, *other_names*, *gamma_names*), the lists of observerving instruments (*observed_by*) are not complete. Identifiers from catalogues like TeVCat [2] are incomplete.

[1] https://github.com/gammapy/gamma-cat

[2] http://tevcat.uchicago.edu/