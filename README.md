# DEBBIE dictionaries annotation

The DEBBIE dictionaries annotator is part of the Biomaterials Annotator system; a lexical resource for performing annotations on the biomaterials literature. The main project and the documentation of the Biomaterials Annotator is available at https://github.com/ProjectDebbie/Biomaterials_annotator.

The DEBBIE dictionaries annotation detect relevant entities related to the biomaterials domain in the text based on several resources detailed below. Is also responsible to execution JAPE rules for post-processing functions, such as the removal of false positives and the addition of information to each annotation. In addition, JAPE rules were run to identify entities using lexical constraints and address the concept recognition of abbreviations.

For a more complete explanation please refer to the [Biomaterials Annotator](https://github.com/ProjectDebbie/Biomaterials_annotator) main page. 

## Resources used for the DEBBIE dictionaries annotator 

1. [DEB](https://bioportal.bioontology.org/ontologies/DEB)
2. [GMDN](https://www.gmdnagency.org/)
3. [CHEBI](https://bioportal.bioontology.org/ontologies/CHEBI)
4. [IOBC](https://bioportal.bioontology.org/ontologies/IOBC)
5. [NCIT](https://bioportal.bioontology.org/ontologies/NCIT)
6. [NPO](https://bioportal.bioontology.org/ontologies/NPO)
7. [OBI](https://bioportal.bioontology.org/ontologies/OBI)
8. [ONTOTOXNUC](https://bioportal.bioontology.org/ontologies/ONTOTOXNUC)
9. [UBERON](https://bioportal.bioontology.org/ontologies/UBERON)
10. [PREMEDONTO](https://bioportal.bioontology.org/ontologies/PREMEDONTO)
11. [EDAM Bioimaging Ontology](https://bioportal.bioontology.org/ontologies/EDAM-BIOIMAGING)
12. [CHMO](https://bioportal.bioontology.org/ontologies/CHMO)
 

Internally, the DEBBIE_dictionaries_annotations component uses the generic nlp-gate-generic-component https://gitlab.bsc.es/inb/text-mining/generic-tools/nlp-gate-generic-component. This library is a generic component that annotate text with parametrices GATE-formatted gazetters/dictionaries. In other words, the DEBBIE_dictionaries_annotations component is an instance of the nlp-gate-generic-component with the umls dictionaries relevant for the biomaterial domain. This component uses the flexible gazetter option of the nlp-gate-generic-component; the terms of the gazetter are annotated using the words present in the text and also using the words lemma (morphological root value).

## Actual Version: 1.0.0, 2021-03-23
## [Changelog](https://github.com/ProjectDebbie/DEBBIE_dictionaries_annotations/blob/main/CHANGELOG) 

## Docker

projectdebbie/debbie_dictionaries_annotations

## Built With

* [Docker](https://www.docker.com/) - Docker Containers
* [Maven](https://maven.apache.org/) - Dependency Management

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/ProjectDebbie/DEBBIE_dictionaries_annotations/tags). 

## Authors

**Javier Corvi and Osnat Hakimi** 

## License

This project is licensed under the GNU License - see the [LICENSE](LICENSE) file for details

## Funding
<img align="left" width="75" height="50" src="eu_emblem.png"> This project has received funding from the European Union’s Horizon 2020 research and innovation programme under the Marie Sklodowska-Curie grant agreement No 751277
		
		
