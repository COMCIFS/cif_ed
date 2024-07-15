# Recommended data to report in Zenodo deposition of NanED round-robin results

These tables provide examples of metadata that was required to be supplied in depositions to Zenodo of data sets from the NanED round-robin experiments
(original at https://zenodo.org/records/7092770) and could provide useful references for identifying mandatory metadata and appropriate ways to record them.

CIF data items useful for reporting this information are suggested. Normal typeface: exists in core dictionary; bold typeface: proposed as new item in cif_ed.dic; italic typeface: exists in imgCIF dictionary.

## (1) Continuous-rotation experiment

| General information:                  |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Project                               | NanED (www.naned.eu)                  |      |
| ESR Project                           | ESR4 & ESR5 - Round Robin             |      |
| Project Label                         | RR1                                   |      |
| Sample Label                          | RR1-S2_PRAHA                          |      |
| Data set Label                        | RR1-S2_PRAHA-CROT                     |      |

| Instrumental:                         |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Instrument                            | Transmission electron microscope <br>FEI Tecnai G2 20       |  `_diffrn_source.description`   |
| Radiation source                      | LaB6                                  |  `_diffrn_source.make`    |
| Accelerating voltage                  | 200 kV                                |  `_diffrn_source.voltage`   |
| Wavelength                            | 0.0251 Å                              |  `_diffrn_radiation.wavelength`   |
| Probe Type                            | Microdiffraction                      |  **`_diffrn_source.ed_probe_formation`**<br>*or* `_diffrn_source.device`<br>`_diffrn_source.details`    |
| Beam Diameter                         | 900                                   |  `_diffrn_source.size`   |
| Beam Convergence                      | Parallel beam, convergence <0.1mrad   |  **`_diffrn_source.convergence_angle`**   |
| Detector                              | Hybrid pixel detector ASI Cheetah (side-mounted)    |  `_diffrn_detector.make`<br>`_diffrn_detector.description`   |
| Number of pixels in the image         | 512 x 512                             |  *`_array_structure_list.index`*<br>*`_array_structure_list.dimension`*   |
| Pixel size                            | 55 µm x 55 µm                         |  *`_array_element_size.index`*<br>*`_array_element_size.size`*    |
| Pixel binning                         |                                       |  *`_array_intensities.pixel_binning_method`*    |
| Effective camera length               | 1000 mm [1]                           |  *`_diffrn_scan_axis.displacement_start`*<br>*`_diffrn_scan_axis.displacement_range`*    |
| Calibration constant                  | 0.008259 Å-1/pixel                    |  **`_diffrn_detector.ed_calibration_constant`**    |


| Sample description:                   |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Name                                  | Natrolite                             |  `_chemical.name_common`<br>`_chemical.name_mineral`<br>`_chemical.name_structure_type`<br>`_chemical.name_systematic`     |
| Chemical composition                  | Na2Al2Si3O10.2H2O                     |  `_chemical_formula.analytical`<br>`_chemical_formula.IUPAC`<br>`_chemical_formula.moiety`<br>`_chemical_formula.structural`<br>`_chemical_formula.sum`    |
| Sample source                         | Natural sample from Marianska Skala, Usti nad Labem, Czechia  |  `_chemical.compound_source`    |
| Sample preparation                    | Powder crushed in an agate mortar and deposited on a Cu grid with holey C film |  `_exptl_crystal.preparation`    |


| Experimental                          |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Data Type                             | Electron diffraction data - 3D ED     |  `_diffrn_radiation.probe`  |
| Data collection method                | Continuous rotation                   |  **`_diffrn_measurement.integration`**    |
| Temperature (K) used during data collection |   95 K                          |  `_diffrn.ambient_temperature`   |
| Number of crystals contributing to the data set      | 1                      |  `_exptl.crystals_number`    |
| Number of experimental frames         | 240                                   |  *`_diffrn_scan.frames`*    |
| tilt range, tilt step, tilt per frame | -60° to +60°, 0.5°, 0.5°              |  *`_diffrn_scan_axis.axis_id`*<br>*`_diffrn_scan_axis.angle_start`*<br>*`_diffrn_scan_axis.angle_range`*<br>*`_diffrn_scan_axis.angle_increment`*    |
| Exposure time per frame               | 482ms                                 |  *`_diffrn_scan.integration_time`*    |


| Software                              |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Software used for the data collection | RATS software                         |  `_computing.diffrn_collection`   |
| Software used for processing          | PETS2 (ver 2.2.20220701.0941)         |  `_computing.diffrn_reduction`   | 


| Authorship and bibliography           |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Author of the data                    | Hrushikesh Chintakindi (ESR 4)<br>& Ashwin Suresh (ESR 5)   | `_audit_author.address`<br>`_audit_author.id_ORCID`<br>`_audit_author.name` *etc.*     |
| Related data                          |                                       | `_database_related.entry_code`<br>`_database_related.relation`<br>`_database_related.special_details`     |
| Publication(s)                        |                                       | Use items in the CITATION and CITATION_AUTHOR categories     |


| Files and data formats                |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Image folder                          | dpcrot : Folder containing images of the diffraction pattern from each frame.    | *`_array_data_external_data.uri`*<br>*`_array_data_external_data.path`* *etc.*  |
| Image format                          | tiff_16bit                            |  *`_array_data_external_data.format`*    |
| Additional folders/files              | Crystal_image : image of the crystal<br>S2_C5-crot-050_petsdata : Log files of Pts2 processing<br>S2_C5-crot-050.pts2 :_input file for the program PETS2 used for processing the data   |     |


**Notes:**
 * The software, RATS used for data collection is an in-house software developed in FZU, Praha
 * Project Label "RR1" stands for Round Robin 1
 * Data set label "RR1-S2_PRAHA-CROT" stands for Round Robin 1 sample 2 from Praha, data collection method continuous rotation   
 * The additional files can be found in the folder NATROLITE_RR1-S2_PRAHA\Continunous_rotation\Data_collection_processing

[1] Understood as equivalent to 'sample-to-detector distance'.

## (2) Precession experiment

| General information:                  |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Project                               | NanED (www.naned.eu)                  |      |
| ESR Project                           | ESR4 & ESR5 - Round Robin             |      |
| Project Label                         | RR1                                   |      |
| Sample Label                          | RR1-S2_PRAHA                          |      |
| Data set Label                        | RR1-S2_PRAHA-PREC                     |      |

| Instrumental:                         |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Instrument                            | Transmission electron microscope<br>FEI Tecnai G2 20                  | `_diffrn_source.description`     |
| Radiation source                      | LaB6                                  |  `_diffrn_source.make`    |
| Accelerating voltage                  | 200 kV                                |  `_diffrn_source.voltage`    |
| Wavelength                            | 0.0251 Å                              |  `_diffrn_radiation.wavelength`    |
| Probe Type                            | Microdiffraction                      |   **`_diffrn_source.ed_probe_formation`**<br>*or* `_diffrn_source.device`<br>`_diffrn_source.details`    |
| Beam Diameter                         | 900                                   |  `_diffrn_source.size`    |
| Beam Convergence                      | Parallel beam, convergence <0.1mrad   |  *`_diffrn_source.convergence_semi_angle`*    |
| Detector                              | Hybrid pixel detector ASI Cheetah (side-mounted)    |  **`_diffrn_detector.make`**<br>**`_diffrn_detector.description`**    |
| Number of pixels in the image         | 512 x 512                             |  *`_array_structure_list.index`*<br>*`_array_structure_list.dimension`*   |
| Pixel size                            | 55 µm x 55 µm                         |  *`_array_element_size.index`*<br>*`_array_element_size.size`*    |
| Pixel binning                         |                                       |  *`_array_intensities.pixel_binning_method`*    |
| Effective camera length               | 1000 mm [1]                           |  *`_diffrn_scan_axis.displacement_start`*<br>*`_diffrn_scan_axis.displacement_range`*    |
| Calibration constant                  | 0.008259 Å-1/pixel                    |  **`_diffrn_detector.ed_calibration_constant`**    |

| Sample description:                   |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Name                                  | Natrolite                             |  `_chemical.name_common`<br>`_chemical.name_mineral`<br>`_chemical.name_structure_type`<br>`_chemical.name_systematic`    |
| Chemical composition                  | Na2Al2Si3O10.2H2O                     |  `_chemical_formula.analytical`<br>`_chemical_formula.IUPAC`<br>`_chemical_formula.moiety`<br>`_chemical_formula.structural`<br>`_chemical_formula.sum`    |
| Sample source                         | Natural sample from Marianska Skala, Usti nad Labem, Czechia  | `_chemical.compound_source`     |
| Sample preparation                    | Powder crushed in an agate mortar and deposited on a Cu grid with holey C film |  `_exptl_crystal.preparation`    |


| Experimental                          |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Data Type                             | Electron diffraction data - 3D ED     |  `_diffrn_radiation.probe`    |
| Data collection method                | Precession                            |  **`_diffrn_measurement.method_precession`**    |
| Temperature (K) used during data collection |   95 K                          |  `_diffrn.ambient_temperature`   |
| Number of crystals contributing to the data set       | 1                                     | `_exptl.crystals_number`      |
| Number of experimental frames         | 121                                   |  *`_diffrn_scan.frames`*    |
| tilt range, tilt step, tilt per frame | -60° to +60°, 1°, 0.99°               |  *`_diffrn_scan_axis.axis_id`*<br>*`_diffrn_scan_axis.angle_start`*<br>*`_diffrn_scan_axis.angle_range`*<br>*`_diffrn_scan_axis.angle_increment`*      |
| Precession angle                      |  1°                                   |  **`_diffrn.precession_angle`**    |
| Exposure time per frame               | 500ms                                 |  *`_diffrn_scan.integration_time`*     |


| Software                              |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Software used for the data collection | RATS software                         |  `_computing.diffrn_collection`   |
| Software used for processing          | PETS2 (ver 2.2.20220701.0941)         |  `_computing.diffrn_reduction`   |




| Authorship and bibliography           |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Author of the data                    | Hrushikesh Chintakindi (ESR 4)<br> & Ashwin Suresh (ESR 5)               | `_audit_author.address`<br>`_audit_author.id_ORCID`<br>`_audit_author.name` *etc.*     |
| Related data                          |                                       | `_database_related.entry_code`<br>`_database_related.relation`<br>`_database_related.special_details`     |
| Publication(s)                        |                                       | Use items in the CITATION and CITATION_AUTHOR categories     |


| Files and data formats                |                                       |      |
| ------------------------------------- | ------------------------------------- | ---- |
| Image folder                          | dp100 : Folder containing images of the diffraction pattern from each frame.    | *`_array_data_external_data.uri`*<br>*`_array_data_external_data.path`* *etc.*  |
| Image format                          | tiff_16bit                            | *`_array_data_external_data.format`*     |
| Additional folders/files              | Crystal_image : image of the crystal<br>S2_C5_prec-100_petsdata : Log files of Pts2 processing<br>S2_C5_prec-100.pts2 :_input file for the program PETS2 used for processing the data                              | *`_array_data_external_data.uri`*<br>*`_array_data_external_data.path`* *etc.*     |


**Notes:**                                                                   
 * The software, RATS used for data collection is an in-house software developed  in FZU, Praha 
 * Project Label "RR1" stands for Round Robin 1 
 * Data set label "RR1-S2_PRAHA-PREC" stands for Round Robin 1 sample 2 from Praha, data collection method Precession                                      |
 * The additional files can be found in the folder Precession\Data_collection_processing 

[1] Understood as equivalent to 'sample-to-detector distance'.
