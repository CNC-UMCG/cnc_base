# Singularity image catalogue for CNC HPC pipeline #
_cnc_base_

---

This image is meant for use on [Peregrine HPC](https://www.rug.nl/society-business/centre-for-information-technology/research/services/hpc/facilities/peregrine-hpc-cluster), RuG 

Currently, I am working on a managed pipeline system with the following specifications:
- Source system: [XNAT 1.7](https://www.xnat.org)
- Python listener, which transports XNAT DICOM data to HPC
- Catalogue of Singularity images with software (see below)
- The required image / pipeline is configured in XNAT as additional resource / input
- Pipeline output is stored on [iRODS](https://irods.org)
- Logfiles will be stored in electronic elabjournal via REST ([BIO-itech](https://www.bio-itech.nl/en/products/eln/))

## Planned catalogue ##

| Name | Description |
--- | --- 
| **cnc_base** | ubuntu 16.04 image with dcm2niix and datalab. Additionally, our conversion script using dcm2niix with additional organization of files |
| **[cnc_spm](https://github.com/CNC-UMCG/cnc_spm)** | cnc_base + standalone SPM version for SPM pipelines |
| **[cnc_fsl](https://github.com/CNC-UMCG/cnc_fsl)** | cnc_base + FSL version ... |
| **[cnc_spm-fsl](https://github.com/CNC-UMCG/cnc_spm-fsl)** | cnc_spm + FSL version ...? |
| **[cnc_meica](https://github.com/CNC-UMCG/cnc_meica)** | cnc_base + AFNI comprising meica (conversion of multi-echo data) |
| **[cnc_freesurfer](https://github.com/CNC-UMCG/cnc_freesurfer)** | cnc_base + freesurfer version:?? |
| **[cnc_qmri](https://github.com/CNC-UMCG/cnc_qmri)** | cnc_spm-fsl + ANTS + ... |

--- 

If you are interested please contact me.

Jan-Bernard Marsman, PhD

Cognitive Neuroscience Center

Department of Neuroscience

University Medical Center Groningen

j.b.c.marsman [at] umcg.nl

