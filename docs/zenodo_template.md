# Recommended data to report in Zenodo deposition of NanED round-robin results

These tables provide examples of metadata that was required to be supplied in depositions to Zenodo of data sets from the NanED round-robin experiments
(original at https://zenodo.org/records/7092770) and could provide useful references for identifying mandatory metadata and appropriate ways to record them.

CIF data items useful for reporting this information are suggested. Normal typeface: exists in core dictionary; bold typeface: proposed as new item in cif_ed.dic; italic typeface: exists in ingCIF dictionary.

## (1) Continuous-rotation experiment

| General information:                  |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Project                               | NanED (www.naned.eu)                  |      |
| ESR Project                           | ESR4 & ESR5 - Round Robin             |      |
| Project Label                         | RR1                                   |      |
| Sample Label                          | RR1-S2_PRAHA                          |      |
| Data set Label                        | RR1-S2_PRAHA-CROT                     |      |


| Experimental                          |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Data Type                             | Electron diffraction data - 3D ED     |      |
| Data collection method                | Continuous rotation                   |  **`_diffrn_measurement.integration`**    |
| Number of experimental frames         | 240                                   |  *`_diffrn_scan.frames`*    |
| tilt range, tilt step, tilt per frame | -60° to +60°, 0.5°, 0.5°              |  *`_diffrn_scan_axis.axis_id`*<br>*`_diffrn_scan_axis.angle_start`*<br>*`_diffrn_scan_axis.angle_range`*<br>*`_diffrn_scan_axis.angle_increment`*    |
| Exposure time per frame               | 482ms                                 |  *`_diffrn_scan.integration_time`*    |
| Software used for the data collection | RATS software                         |  `_computing.diffrn_collection`   |


| Instrumental:                         |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Instrument                            | Transmission electron microscope <br>FEI Tecnai G2 20       |  `_diffrn_source.description`   |
| Radiation source                      | LaB6                                  |  `_diffrn_source.make`    |
| Accelerating voltage                  | 200 kV                                |  `_diffrn_source.voltage`   |
| Wavelength                            | 0.0251 Å                              |  `_diffrn_radiation.wavelength`   |
| Probe Type                            | Microdiffraction [1]                  |  `_diffrn_radiation.probe`   |
| Beam Diameter                         | 900                                   |  `_diffrn_source.size`   |
| Beam Convergence                      | Parallel beam, convergence <0.1mrad   |  *`_diffrn_source.convergence_semi_angle`*   |
| Detector                              | Hybrid pixel detector ASI Cheetah     |  **`_diffrn_detector.make`**<br>**`_diffrn_detector.description`**   |
| Number of pixels in the image         | 512 x 512                             |      |
| Pixel size                            | 55 µm x 55 µm                         |      |
| Effective camera length               | 1000 mm                               |      |
| Calibration constant                  | 0.008259 Å-1/pixel                    |      |


| Sample description:                   |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Name                                  | Natrolite                             |  `_chemical.name_common`<br>`_chemical.name_mineral`<br>`_chemical.name_structure_type`<br>`_chemical.name_systematic`     |
| Chemical composition                  | Na2Al2Si3O10.2H2O                     |  `_chemical_formula.analytical`<br>`_chemical_formula.IUPAC`<br>`_chemical_formula.moiety`<br>`_chemical_formula.structural`<br>`_chemical_formula.sum`    |
| Sample source                         | Natural sample from Marianska Skala,  |  `_chemical.compound_source`    |
| Number of crystals contributing to the data set      | 1                      |  `_exptl.crystals_number`    |



| Authorship and bibliography           |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Author of the data                    | Hrushikesh Chintakindi (ESR 4)<br>& Ashwin Suresh (ESR 5)   | `_audit_author.address`<br>`_audit_author.id_ORCID`<br>`_audit_author.name` *etc.*     |
| Related data                          |                                       | `_database_related.entry_code`<br>`_database_related.relation`<br>`_database_related.special_details`     |
| Publication(s)                        |                                       | Use items in the CITATION and CITATION_AUTHOR categories     |


| Files and data formats                |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Image format                          | tiff_16bit                            |  *`_array_data_external_data.format`*    |
| Additional folders/files              | dpcrot : Folder containing images of the diffraction pattern from each frame.<br>Crystal_image : image of the crystal<br>S2_C5-crot-050_petsdata : Log files of Pts2 processing<br>S2_C5-crot-050.pts2 :_input file for the program PETS2 used for processing the data   |  *`_array_data_external_data.uri`*<br>*`_array_data_external_data.path`* *etc.*    |


**Notes:**
 * The software, RATS used for data collection is an in-house software developed in FZU, Praha
 * Project Label "RR1" stands for Round Robin 1
 * Data set label "RR1-S2_PRAHA-CROT" stands for Round Robin 1 sample 2 from Praha, data collection method continuous rotation   
 * The additional files can be found in the folder NATROLITE_RR1-S2_PRAHA\Continunous_rotation\Data_collection_processing
 * [1] Should be 'electron' as a permitted value of `_diffrn_radiation.probe`

## (2) Precession experiment

| General information:                  |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Project                               | NanED (www.naned.eu)                  |      |
| ESR Project                           | ESR4 & ESR5 - Round Robin             |      |
| Project Label                         | RR1                                   |      |
| Sample Label                          | RR1-S2_PRAHA                          |      |
| Data set Label                        | RR1-S2_PRAHA-PREC                     |      |


| Experimental                          |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Data Type                             | Electron diffraction data - 3D ED     |      |
| Data collection method                | Precession                            |  **`_diffrn_measurement.method_precession`**    |
| Number of experimental frames         | 121                                   |  *`_diffrn_scan.frames`*    |
| tilt range, tilt step, tilt per frame | -60° to +60°, 1°, 0.99°               |  *`_diffrn_scan_axis.axis_id`*<br>*`_diffrn_scan_axis.angle_start`*<br>*`_diffrn_scan_axis.angle_range`*<br>*`_diffrn_scan_axis.angle_increment`*      |
| Exposure time per frame               | 500ms                                 |  *`_diffrn_scan.integration_time`*     |
| Software used for the data collection | RATS software                         |  `_computing.diffrn_collection`    |


| Instrumental:                         |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Instrument                            | Transmission electron microscope<br>FEI Tecnai G2 20                  | `_diffrn_source.description`     |
| Radiation source                      | LaB6                                  |  `_diffrn_source.make`    |
| Accelerating voltage                  | 200 kV                                |  `_diffrn_source.voltage`    |
| Wavelength                            | 0.0251 Å                              |  `_diffrn_radiation.wavelength`    |
| Probe Type                            | Microdiffraction [1]                  |  `_diffrn_radiation.probe`    |
| Beam Diameter                         | 900                                   |  `_diffrn_source.size`    |
| Beam Convergence                      | Parallel beam, convergence <0.1mrad   |  *`_diffrn_source.convergence_semi_angle`*    |
| Detector                              | Hybrid pixel detector ASI Cheetah     |  **`_diffrn_detector.make`**<br>**`_diffrn_detector.description`**    |
| Number of pixels in the image         | 512 x 512                             |      |
| Pixel size                            | 55 µm x 55 µm                         |      |
| Effective camera length               | 1000 mm                               |      |
| Calibration constant                  | 0.008259 Å-1/pixel                    |      |


| Sample description:                   |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Name                                  | Natrolite                             |  `_chemical.name_common`<br>`_chemical.name_mineral`<br>`_chemical.name_structure_type`<br>`_chemical.name_systematic`    |
| Chemical composition                  | Na2Al2Si3O10.2H2O                     |  `_chemical_formula.analytical`<br>`_chemical_formula.IUPAC`<br>`_chemical_formula.moiety`<br>`_chemical_formula.structural`<br>`_chemical_formula.sum`    |
| Sample source                         | Natural sample from Marianska Skala,   Usti nad Labem, Czechia  | `_chemical.compound_source`     |
| Number of crystals contributing to the data set       | 1                                     | `_exptl.crystals_number`      |


| Authorship and bibliography           |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Author of the data                    | Hrushikesh Chintakindi (ESR 4)<br> & Ashwin Suresh (ESR 5)               | `_audit_author.address`<br>`_audit_author.id_ORCID`<br>`_audit_author.name` *etc.*     |
| Related data                          |                                       | `_database_related.entry_code`<br>`_database_related.relation`<br>`_database_related.special_details`     |
| Publication(s)                        |                                       | Use items in the CITATION and CITATION_AUTHOR categories     |


| Files and data formats                |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Image format                          | tiff_16bit                            | *`_array_data_external_data.format`*     |
| Additional folders/files              | dp100 : Folder containing images of the diffraction pattern from each frame.<br>Crystal_image : image of the crystal<br>S2_C5_prec-100_petsdata : Log files of Pts2 processing<br>S2_C5_prec-100.pts2 :_input file for the program PETS2 used for processing the data                              | *`_array_data_external_data.uri`*<br>*`_array_data_external_data.path`* *etc.*     |


**Notes:**                                                                   
 * The software, RATS used for data collection is an in-house software developed  in FZU, Praha 
 * Project Label "RR1" stands for Round Robin 1 
 * Data set label "RR1-S2_PRAHA-PREC" stands for Round Robin 1 sample 2 from Praha, data collection method Precession                                      |
 * The additional files can be found in the folder Precession\Data_collection_processing 
 * [1] Should be 'electron' as a permitted value of `_diffrn_radiation.probe`
