# cnc_base #

*Base image for CNC HPC pipeline*

This image is meant for use on [Peregrine HPC](https://www.rug.nl/society-business/centre-for-information-technology/research/services/hpc/facilities/peregrine-hpc-cluster), RuG 

Currently, I am working on a managed pipeline system with the following specifications:
- Source system: [XNAT 1.7](https://www.xnat.org)
- Python listener, which transports XNAT DICOM data to HPC
- Catalogue of Singularity images with software (spm, fsl, freesurfer, meica, qmri)
- The required image / pipeline is configured in XNAT as additional resource / input
- Pipeline output is stored on [iRODS](https://irods.org)
- Logfiles will be stored in electronic elabjournal via REST ([BIO-itech](https://www.bio-itech.nl/en/products/eln/))

If you are interested please contact me.

Jan-Bernard Marsman, PhD

Cognitive Neuroscience Center

Department of Neuroscience

University Medical Center Groningen

j.b.c.marsman [at] umcg.nl

