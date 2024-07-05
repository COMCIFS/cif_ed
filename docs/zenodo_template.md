# Recommended data to report in Zenodo deposition of NanED round-robin results

These tables provide examples of metadata that was required to be supplied in depositions to Zenodo of data sets from the NanED round-robin experiments
(original at https://zenodo.org/records/7092770) and could provide useful references for identifying mandatory metadata and appropriate ways to record them

## (1) Continuous-rotation experiment

| General information:                  |                                       |
| ------------------------------------- | ------------------------------------- |
| Project                               | NanED (www.naned.eu)                  |
| ESR Project                           | ESR4 & ESR5 - Round Robin             |
| Project Label                         | RR1                                   |
| Sample Label                          | RR1-S2_PRAHA                          |
| Data set Label                        | RR1-S2_PRAHA-CROT                     |


| Experimental                          |                                       |
| ------------------------------------- | ------------------------------------- |
| Data Type                             | Electron diffraction data - 3D ED     |
| Data collection method                | Continuous rotation                   |
| Number of experimental frames         | 240                                   |
| tilt range, tilt step, tilt per frame | -60° to +60°, 0.5°, 0.5°              |
| Exposure time per frame               | 482ms                                 |
| Software used for the data collection | RATS software                         |


| Instrumental:                         |                                       |
| ------------------------------------- | ------------------------------------- |
| Instrument                            | Transmission electron microscope <br>FEI Tecnai G2 20                  |
| Radiation source                      | LaB6                                  |
| Accelerating voltage                  | 200 kV                                |
| Wavelength                            | 0.0251 Å                              |
| Probe Type                            | Microdiffraction                      |
| Beam Diameter                         | 900                                   |
| Beam Convergence                      | Parallel beam, convergence <0.1mrad   |
| Detector                              | Hybrid pixel detector ASI Cheetah     |
| Number of pixels in the image         | 512 x 512                             |
| Pixel size                            | 55 µm x 55 µm                         |
| Effective camera length               | 1000 mm                               |
| Calibration constant                  | 0.008259 Å-1/pixel                    |


| Sample description:                   |                                       |
| ------------------------------------- | ------------------------------------- |
| Name                                  | Natrolite                             |
| Chemical composition                  | Na2Al2Si3O10.2H2O                     |
| Sample source                         | Natural sample from Marianska Skala,  |
| Number of crystals contributing to the data set      | 1                                     |



| Authorship and bibliography           |                                       |
| ------------------------------------- | ------------------------------------- |
| Author of the data                    | Hrushikesh Chintakindi (ESR 4)<br>& Ashwin Suresh (ESR 5)               |
| Related data                          |                                       |
| Publication(s)                        |                                       |


| Files and data formats                |                                       |
| ------------------------------------- | ------------------------------------- |
| Image format                          | tiff_16bit                            |
| Additional folders/files              | dpcrot : Folder containing images of the diffraction pattern from each frame. <br>Crystal_image : image of the crystal<br>S2_C5-crot-050_petsdata : Log files of Pts2 processing<br>S2_C5-crot-050.pts2 :_input file for the program PETS2 used for processing the data                              |


**Notes:**
 * The software, RATS used for data collection is an in-house software developed in FZU, Praha
 * Project Label "RR1" stands for Round Robin 1
 * Data set label "RR1-S2_PRAHA-CROT" stands for Round Robin 1 sample 2 from Praha, data collection method continuous rotation   
 * The additional files can be found in the folder NATROLITE_RR1-S2_PRAHA\Continunous_rotation\Data_collection_processing

## (2) Precession experiment

| General information:                  |                                       |
| ------------------------------------- | ------------------------------------- |
| Project                               | NanED (www.naned.eu)                  |
| ESR Project                           | ESR4 & ESR5 - Round Robin             |
| Project Label                         | RR1                                   |
| Sample Label                          | RR1-S2_PRAHA                          |
| Data set Label                        | RR1-S2_PRAHA-PREC                     |


| Experimental                          |                                       |
| ------------------------------------- | ------------------------------------- |
| Data Type                             | Electron diffraction data - 3D ED     |
| Data collection method                | Precession                            |
| Number of experimental frames         | 121                                   |
| tilt range, tilt step, tilt per frame | -60° to +60°, 1°, 0.99°               |
| Exposure time per frame               | 500ms                                 |
| Software used for the data collection | RATS software                         |


| Instrumental:                         |                                       |
| ------------------------------------- | ------------------------------------- |
| Instrument                            | Transmission electron microscope<br>FEI Tecnai G2 20                  |
| Radiation source                      | LaB6                                  |
| Accelerating voltage                  | 200 kV                                |
| Wavelength                            | 0.0251 Å                              |
| Probe Type                            | Microdiffraction                      |
| Beam Diameter                         | 900                                   |
| Beam Convergence                      | Parallel beam, convergence <0.1mrad   |
| Detector                              | Hybrid pixel detector ASI Cheetah     |
| Number of pixels in the image         | 512 x 512                             |
| Pixel size                            | 55 µm x 55 µm                         |
| Effective camera length               | 1000 mm                               |
| Calibration constant                  | 0.008259 Å-1/pixel                    |


| Sample description:                   |                                       |
| ------------------------------------- | ------------------------------------- |
| Name                                  | Natrolite                             |
| Chemical composition                  | Na2Al2Si3O10.2H2O                     |
| Sample source                         | Natural sample from Marianska Skala,   Usti nad Labem, Czechia               |
| Number of crystals contributing to the data set       | 1                                     |


| Authorship and bibliography           |                                       |
| ------------------------------------- | ------------------------------------- |
| Author of the data                    | Hrushikesh Chintakindi (ESR 4)<br> & Ashwin Suresh (ESR 5)               |
| Related data                          |                                       |
| Publication(s)                        |                                       |


| Files and data formats                |                                       |
| ------------------------------------- | ------------------------------------- |
| Image format                          | tiff_16bit                            |
| Additional folders/files              | dp100 : Folder containing images of the diffraction pattern from each frame.<br>Crystal_image : image of the crystal<br>S2_C5_prec-100_petsdata : Log files of Pts2 processing<br>S2_C5_prec-100.pts2 :_input file for the program PETS2 used for processing the data                              |


**Notes:**                                                                   
 * The software, RATS used for data collection is an in-house software developed  in FZU, Praha 
 * Project Label "RR1" stands for Round Robin 1 
 * Data set label "RR1-S2_PRAHA-PREC" stands for Round Robin 1 sample 2 from Praha, data collection method Precession                                      |
 * The additional files can be found in the folder Precession\Data_collection_processing 
