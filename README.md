[![CIF dictionary check](https://github.com/COMCIFS/cif_ed/actions/workflows/main.yml/badge.svg)](https://github.com/COMCIFS/cif_ed/actions)

# cif_ed

Data names for describing electron diffraction. These are presented here as a CIF extension dictionary, although in practice many are equally applicable to X-ray or neutron studies. This draft, when approved by COMCIFS, will be incorporated periodically into the existing core CIF and possibly imgCIF dictionaries.

This project is best seen as an opportunity to focus on the new items required in the context of electron crystallography, and to invite content review from the user community.

The first set of data definitions incorporated into the core CIF dictionary are those in **release 1.0.0** of 24 March 2025. Any definitions in cif_ed.dic with latest revision later than that date should be considered work in progress, and should not be used in production software.


This GitHub project contains:

* cif_ed.dic : a draft electron diffraction dictionary. This was initially set up as a new extension dictionary, but because relatively few new data names are needed, many of which are of general relevance to diffraction experiments, its content has been incorporated into the core dictionary.
* draft_new_items.dic: a file containing additional definitions that are more likely to be incorporated in the future in the imgCIF dictionary 
* docs : a folder containing supporting documentation.
  * docs/ed.pdf : a PDF typeset representation of the draft dictionary to facilitate review by people unfamiliar with DDL formalism.
  * docs/proposal.md : the initial proposals of the NanED standardisation committee, with suggested enhancements.
  * docs/electron_examples.md : a survey of current usage in CIFs reporting 3DED structure determinations.
  * docs/recommendations.md : draft recommendations to authors to harmonise their use of CIF items.
  * docs/platon_checks.pdf: summary of all checks currently available to _PLATON_, to allow consideration of others that might need to be altered or suppressed.
  * docs/zenodo_template.md: examples of metadata for Zenodo deposition of round-robin data sets with suggested mappings to CIF data names, potentially useful for identifying mandatory requirements
  * docs/frames_example.cif: an example CIF structured following the imgCIF dictionary to indicate how per-frame data (including orientations) could be recorded, and also how to provide links to individual images stored in an external repository. Numeric values are illustrative - for example, axis definitions should be chosen to be compatible with imgCIF definitions - but the general structure is presented. Compare with imgCIF files associated with published articles in *Raw Data Letters*: https://doi.org/10.1107/S2414314622008525/he4557img.cif, 
https://doi.org/10.1107/S2414314623001141/iq4001img1.cif,
https://doi.org/10.1107/S2414314623001141/iq4001img2.cif,
https://doi.org/10.1107/S2414314622010598/ii4001img.cif
