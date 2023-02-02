# emzo_azores_instance_segmentation
[![Build Status](https://jenkins.indigo-datacloud.eu/buildStatus/icon?job=Pipeline-as-code/DEEP-OC-org/UC-jb06098-marine_species_seg/master)](https://jenkins.indigo-datacloud.eu/job/Pipeline-as-code/job/DEEP-OC-org/job/UC-jb06098-marine_species_seg/job/master)

WIP : Identification of marine species from EMSO Azores deep-sea obervatory

To launch it, first install the package then run [deepaas](https://github.com/indigo-dc/DEEPaaS):
```bash
git clone https://gitlab.ifremer.fr/jb06098/marine_species_seg
cd marine_species_seg
pip install -e .
deepaas-run --listen-ip 0.0.0.0
```
The associated Docker container for this module can be found in https://gitlab.ifremer.fr/jb06098/DEEP-OC-marine_species_seg.

## Project structure
```
├── LICENSE                <- License file
│
├── README.md              <- The top-level README for developers using this project.
│
├── requirements.txt       <- The requirements file for reproducing the analysis environment, e.g.
│                             generated with `pip freeze > requirements.txt`
│
├── setup.py, setup.cfg    <- makes project pip installable (pip install -e .) so
│                             marine_species_seg can be imported
│
├── marine_species_seg    <- Source code for use in this project.
│   │
│   ├── __init__.py        <- Makes marine_species_seg a Python module
│   │
│   └── api.py             <- Main script for the integration with DEEP API
│
└── Jenkinsfile            <- Describes basic Jenkins CI/CD pipeline
```
