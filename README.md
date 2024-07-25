# cif_ed

Data names for describing electron diffraction. These are presented here as a CIF extension dictionary, but in practice many are equally applicable to X-ray or neutron studies, and so this draft, when approved by COMCIFS, might best be incorporated into the existing core CIF and possibly imgCIF dictionaries.

This project is best seen as an opportunity to focus on the new items required in the context of electron crystallography, and to invite content review from the user community.



This GitHub project contains:

* cif_ed.dic : a draft electron diffraction dictionary. This is currently set up as a new extension dictionary, but if in the end only few new data names are needed, it may be incorporated into the core dictionary.
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
