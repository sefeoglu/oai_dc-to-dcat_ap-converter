# DCAT Converter
The project converts the oai_dc formatted meta data into dcat_ap format and save them in rdf format.


## Project Folder Structure
````
.
├── Dockerfile
├── LICENSE
├── README.md
├── compose.yaml
├── config.ini
├── data
│   └── sample.rdf
├── requirements.txt
└── src
    ├── converter_service.py
    ├── data_crawler.py
    ├── dcat_ap.py
    └── utils.py
````
## Run
* Create a conda environment

```
$ conda create -n dcat_env python=3.9
```

* Activate enviroment

```
$ conda activate dcat_env
```
* Install Requirements

```
pip install -r requirements.txt
```
WIP!
## Data Collection
* Give the parameters for the APIs in ```config.ini```
  
* Run the scprit below:
``` 
python data_crawler.py
```

## Repository APIs
* 1.) Refubium Repository

```
https://refubium.fu-berlin.de/oai/dnb?verb=ListRecords&resumptionToken=xMetaDissPlus////
```

* 2.) Depositonce Repository

```
https://api-depositonce.tu-berlin.de/server/oai/request?verb=ListRecords&resumptionToken=oai_dc////
```
* 3.) Edoc Repository

```
https://edoc.hu-berlin.de/oai/request/?verb=ListRecords&resumptionToken=oai_dc////
```

* Note:Poster paper from the project has been submitted and waiting for the review, so we will update the readme later. The project will be released, so the repository was updated.
