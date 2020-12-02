**This repository is not maintained any longer.**

# finc Solr schema

The [finc](https://finc.info) Solr schema is a derivative of the [VuFind standard Solr schema](https://github.com/vufind-org/vufind/tree/master/solr/vufind/biblio/conf). It is used by Solr cores that empower discovery systems for libraries of the finc user community, e.g.,  [Leipzig University Library]( http://www.ub.uni-leipzig.de/) (UBL) or [Saxon State and University Library Dresden](https://www.slub-dresden.de/) (SLUB). 
It mainly enables search and result display (i.e. results in the hit list) of bibliographic resources.

Since the finc Solr schema is largely compatible to the VuFind standard Solr schema, it should be easily usable by other [VuFind](https://github.com/vufind-org/vufind) or [TYPO3 Find](https://github.com/subugoe/typo3-find) instances as well.

## Usage

### Set up a Solr core

Simply copy the content, i.e. all files, from the folder [solr](solr) into the 'conf' folder of your Solr core that should be powered by the finc Solr schema.

### Apply csv2scldj schema definition of the finc Solr schema

([csv2scldj](https://github.com/slub/csv2scldj) is a commandline tool to convert CSV data into schema conform line-delimited-JSON data)

1. Download the csv2scldj schema file [finc_solr_schema.csv](csv2scldj/finc_solr_schema.csv)
2. Set the csv2scldj schema file path via the commandline parameter '-schema-file-name' of the commandline tool ```csv2scldj```, see the [README of csv2scldj](https://github.com/slub/csv2scldj/blob/master/README.md)
