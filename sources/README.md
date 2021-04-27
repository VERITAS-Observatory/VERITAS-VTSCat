# VERITAS Observations - gamma-ray sources and objects

Description files for objects (*TeV sources*) in the VERITAS catalogue. 

Following the gamma-cat sheme [1] without some format changes (mostly removal of keywords). Many files are modified copies from gamma-cat. The number of objects has been extented compared to gamma-cat and discrepencies in the *source_id* descriptor is expected for *source_id*s numbers above 169. 

## File structure

- one YAML file per object in the format `<tev-source_id>.yaml`.
- non-detection (observations only) are indicated by source IDs > 100000
- cosmic-ray observations are indicated by source IDs > 300000

## File format

The following entries are required:

| Keyword | Definition |
|---|---|
*source_id* | unique identifier of an object (integer) |
*common_name* | common name as frequently used in literature |
*gamma_names* | name assigned by gamma-ray observatory (e.g., VER, MAGIC, or HESS names) |
*other_names* | other names used in literature or from catalogues (not a complete list) |
*where* | galactic (gal) or extragalactic (egal) object |
*pos:simbad_id* | SIMBAD name |
*pos:ra*, *pos: dec* | J2000 coordinates from SIMBAD |
*reference_id* | list of references for this catalogue |

## References

[1] https://github.com/gammapy/gamma-cat
