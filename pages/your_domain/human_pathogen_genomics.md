---
title: Human pathogen genomics
search_exclude: true
description: <!---REPLACE THIS with a one sentence description of the page--->
contributors: [Diana Pilvar, Espen Åberg, Wolmar Nyberg Åkerström, Rafael Andrade Buono]
page_id: human_pathogen_genomics
related_pages: 
  your_tasks:
    - data_brokering
    - metadata_management
    - data_transfer
    - data_protection
    - data_quality
  tool_assembly:
    - covid19_data_portal
  your_domain:
    - rare_disease_data
    - human_data
# More information on which page id you can use can be found at https://rdmkit.elixir-europe.org/website_overview
#training:
#  - name:
#    registry:
#    url:
# More information on how to fill in this metadata section can be found here https://rdmkit.elixir-europe.org/page_metadata
---

# Human Pathogen Genomics

## Introduction
The human pathogen genomics domain focuses on studying the genetic code of organisms that cause disease in humans. Studies to identify and understand pathogens are conducted across different types of organisations ranging from research institutes to regional public health authorities. And the aims can include urgent outbreak response and prevention measures and developing remedies such as treatments and vaccines.

Data management challenges in this domain include the potential urgency of data sharing and secondary use of data across initiatives emerging from research, public health and policy. And while the pathogenic organisms are the object of interest, there are many considerations to account for when dealing with samples collected from patients, pathogen surveillance, and human research subjects.

The genomic data can represent anything from the genetic sequence of a single pathogen isolate to various fragments of genetic materials from a flora of pathogens in larger population. Other data can represent a wide range of contextual information about the human host, the disease, and various environmental factors.

## Planning a study with pathogen genome data

### Description
While the object of interest in this domain are pathogens, the data is usually derived from samples originating from patients and human research subjects. This means that you must plan to either remove or to handle [human data](human_data) during your study.

### Considerations

* What legal and ethical aspects do you need to consider? 
  * Can you separate pathogen and human host material and data?
  * What data protection measures should be implemented in contracts and procedures dealing with suppliers and collaborators?
  * What is the appropriate scope for the legal and ethical agreements necessary for the study?
  * How should statements related to data processing be phrased to allow timely and relevant data sharing?
  * How much time would be required to negotiate access to the samples and data for the study?
* What public health and research initives should you consider aligning with?
  * What data could be shared with or reused from other initiatives during the project?
  * How will you align your practices with these initiatives to maximise the impact of the data and insight generated by the project? 
  * How will you share data with your collaborators and other initiatives?
* What conventions will you adopt when planning your study?
  * What existing protocols should you consider adopting for sample preparation, sequencing, variant calling etc? 
  * What conventions should you adopt for documenting your research? 

### Solutions

#### Working with human data
* Ensure that the project’s procedures conform with good practices for handling [human data](human_data). In particular, the following sections of the RDMkit:
  * [Planning for projects with human data](human_data#planning-for-projects-with-human-data)
  * [Processing and analysing human data](human_data#processing-and-analysing-human-data)

#### Isolate pathogen from host information
* Depending on the pathogen, how it interacts with the host, or the methods applied, it can be possible to generate clean isolates that do not contain host related material. Data produced from a clean isolate could potentially be handled with few restrictions, while other data will be considered to be personal and [sensitive](sensitive_data) that need [protection](data_protection).

#### Public health initiatives
* National and international recommendations from public health authorities, epidemic surveillance programs and research data communities should be considered when planning a new study or surveillance programme. In particular, you could consult conventions for relevant surveillance programs while considering widely adopted guidelines for research documentation, and instructions from the data sharing platforms.
  * [WHO genomic surveillance strategy](https://www.who.int/initiatives/genomic-surveillance-strategy)
  * [European Centre for Disease Prevention and Control](https://www.ecdc.europa.eu/en)
  * [ECDC’s Surveillance and study protocols](https://www.ecdc.europa.eu/en/covid-19/surveillance/study-protocols)
  * [Centers for Disease Control and Prevention (CDC)](https://www.cdc.gov/genomics/pathogen/index.htm)
  * [NCBI Pathogen Detection](https://www.ncbi.nlm.nih.gov/pathogens/)
  * [EMBL-EBI Pathogens](https://www.ebi.ac.uk/ena/pathogens/home)
  * [National resources \| RDMkit](national_resources)

#### Sequencing experiments
* Good practices for annotating sequencing experiments suggest that the documentation, at a minimum, should describe the design of the study or surveillance program, the collected specimens and how the samples were prepared, the experimental setup and protocols, and the analysis workflow.
  * [Minimal Information about a high throughput SEQuencing Experiment (MINSEQE)](https://fairsharing.org/FAIRsharing.a55z32)
  * The RDMkit page on [documentation and metadata](Documentation_and_metadata) provides a guide to how you can document data during a project.
  * This paper gives [Ten simple rules for annotating sequencing experiments](https://doi.org/10.1371/journal.pcbi.1008260) to help data producers collect and store high-quality metadata about sequencing experiments.
* The Genomic Standards Consortium (GSC) have defined a set of core and extended descriptors for genomes and metagenomes with associated samples and their environment to guide scientists on how to capture the metadata essential for high quality research. 
  * [GSC Minimum Information about any Sequence (MIxS)](https://fairsharing.org/FAIRsharing.9aa0zp)
* WHO offers some [guidance on implementation for maximum impact on public health](https://apps.who.int/iris/bitstream/handle/10665/338480/9789240018440-eng.pdf?sequence=1&isAllowed=y) and there are published reports that advise on [implementing Implementing Quality Management Systems in Public Health Laboratories](https://doi.org/10.1128/jcm.00261-19).
* ISO (the International Organization for Standardization) have several general guidelines relevant for both the laboratory and bioinformatic components of genome sequencing.
  * [ISO 20397-1:2022 Biotechnology — Massively parallel sequencing — Part 1: Nucleic acid and library preparation](https://www.iso.org/standard/74054.html)
  * [ISO 20397-2:2021 Biotechnology — Massively parallel sequencing — Part 2: Quality evaluation of sequencing data](https://www.iso.org/standard/67895.html)
  * [ISO/TS 20428:2017 Health informatics — Data elements and their metadata for describing structured clinical genomic sequence information in electronic health records](https://www.iso.org/standard/67981.html)
  * [ISO/TS 22692:2020 Genomics informatics — Quality control metrics for DNA sequencing](https://www.iso.org/standard/73693.html)
  * [ISO 23418:2022 Microbiology of the food chain — Whole genome sequencing for typing and genomic characterization of bacteria — General requirements and guidance](https://www.iso.org/obp/ui/#iso:std:iso:23418:ed-1:v1:en)

## Collecting and processing pathogen sequence data

### Considerations

* What information should you consider recording when collecting data?
  * What should you note when collecting, storing and preparing the samples?
  * How will you capture information about the configuration and quality of the sequencing results?
  * How will you ensure that the information captured is complete and correct?
* What data and file formats should you consider for your project?
  * What are the de-facto standards used for the experiemnt type and down-stream analysis-pipelines?
  * Where are the instrument specific aspects for the data and files formats documented?
* What existing data will you integrate or use as a reference in  your project?
  * What reference genome(s) will you need access to?
  * What is the recommended citation for the data and their versions?

### Solutions

#### Filtering genomic reads corresponding to human DNA fragments

* Data files with reads produced by sequencing experiments sometimes contain fragments of the host organism’s DNA. When the host is a human research subject or patient, these fragments can be masked or removed to produce files that could potentially be handled with fewer restrictions. The approach chosen to mask the host associated reads leads to different trade-offs. Make sure to include this as a factor in your risk assessment.
  * Mapping to (human) host reference genomes, [can inadvertedly leave some host associated reads unmasked](https://doi.org/10.1099%2Fmgen.0.000393). 
  * Mapping to pathogens reference genomes can inadvertedly mask some pathogen associated reads and still leave some host associated reads unmasked
  * [Removal of human reads from SARS-CoV-2 sequencing data \| Galaxy training](https://training.galaxyproject.org/training-material/topics/sequence-analysis/tutorials/human-reads-removal/tutorial.html)


#### Contextual information about the sample

* Information about the host phenotype, context and disease is often necessary to answer questions in a research study or policy perspective. Consider adopting common reporting checklists, terms and vocabularies that can simplify data sharing across initatives. Note: This information can contain personal and sensitive data.
* Other contextual information can include non-host related environmental factors, such as interactions with other pathogens, drugs and geographic proliferation. It can also include information about the sampled material and how it was processed for sequencing.
* Pathogens checklist(s) can be found among [ENA Sample checklists](https://www.ebi.ac.uk/ena/browser/checklists), including checklists derived from the [MIxS consortium](http://w3id.org/mixs). For example the [ENA virus pathogen reporting standard checklist](https://www.ebi.ac.uk/ena/browser/view/ERC000033) has been recurrently used for SARS-CoV-2 studies. Other ontologies and checklists include
  * [Phenotypic QualiTy Ontology](https://bioportal.bioontology.org/ontologies/PATO)
  * [NCBI Taxonomy](https://www.ncbi.nlm.nih.gov/taxonomy)
  * [Disease Ontology](https://disease-ontology.org)
  * [Chemical Entities of Biological Interest](https://bioportal.bioontology.org/ontologies/CHEBI/?p=summary)
  * [UBER anatomy ONtology](https://bioportal.bioontology.org/ontologies/UBERON)

#### Generating genomic data
* Establish protocols and document the steps taken in the lab to process the sample and in the computational workflow to prepare the resulting data. Make sure to keep information from quality assurance procedures and strive to make your labwork and computational process as reproducible as possible.
    * [High-Throughput Sequencing \| LifeScienceRDMLookUp](https://elixir.no/rdm-lookup/sequencing)
    * [The Beyond One Million Genomes (B1MG)](https://b1mg-project.eu) project provides guidelines that cover the minimum [quality requirements](https://zenodo.org/record/5018495) for the generation of genome sequencing data.
    * Data repositories generally have information about recommended [data file formats](Data_publication) and [metadata](metadata_management)
    * The [FAIR Cookbook](https://faircookbook.elixir-europe.org/content/home.html) provides instructions on [validation of file formats](https://faircookbook.elixir-europe.org/content/recipes/interoperability/fastq-file-format-validators.html)
    * A good place to look for scientific and technical information about data quality validation software tools for pathogenomics is  [Bio.Tools](https://bio.tools/t?page=1&q=validation&sort=score&topicID=%22topic_3168%22).
  * The [Infectious Diseases Toolkit (IDTk)](https://www.infectious-diseases-toolkit.org/) has a showcase on [An automated SARS-CoV-2 genome surveillance system built around Galaxy](https://www.infectious-diseases-toolkit.org/showcase/covid19-galaxy)
  * The Galaxy Training Network provides free on-line [training materials on quality control](https://training.galaxyproject.org/training-material/topics/sequence-analysis/tutorials/quality-control/tutorial.html).


## Sharing and preserving pathogen genomic data

### Considerations

* What data need to be preserved by the project and for how long?
* What is preserved by others and how would someone find and access the data?
* What databases should I use to share human pathogen genomics data?


### Solutions

#### Sharing host related and other contextual information
* ?? Something about links to non-sensitive pathogen genome data etc. Aggregate level information, data masking and access to detailed records. Reference human data. Some of this information can be used as metadata for genomic data. 
* ?? Something about federated solutions for data access.

#### Sharing pathogen genomic data
* You should adopt good practices for [data sharing](sharing) and identify which data sharing platforms to used to reach relevant stakeholders. You can use more than one platform but care should be taken to make sure that data is interconnected where possible to enable deduplication in downstream analyses.
  * European healthcare surveillance systems is administered and used by public health authorities such as [ECDC’s TESSy/EpiPulse](https://www.ecdc.europa.eu/en/publications-data/epipulse-european-surveillance-portal-infectious-diseases)
  * International research data exchanges such as [European Neucleotide Archive (ENA)](https://www.ebi.ac.uk/ena/browser/submit) for non-sensitive genomic data and the [Federated EGA](https://ega-archive.org/federated) network for sensitive data.
  * There are also pathogen specifc initiatives, such as GISAID for certain viruses.
* Investigate if there are [national resources](national_resources) or [Data brokering](data_brokering) organisation available to facilitate data sharing.
  * [EBI Pathogens data hubs](https://www.ebi.ac.uk/ena/pathogens/v2/)
  * [Submit new data \| European COVID-19 platform](https://www.covid19dataportal.org/submit-data)

