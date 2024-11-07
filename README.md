# Divvy Data FAIRification Project

## Project Overview
This repository contains the deliverables for the Divvy Data FAIRification project, which aims to enhance the FAIR (Findable, Accessible, Interoperable, Reusable) compliance of the Divvy bicycle-sharing data from Chicago. The project includes a semantic data model, metadata records, and RDF representations of the dataset.

## Project Deliverables
### 1. Project Report
- **Format**: PDF
- **Description**: A comprehensive report detailing the FAIRification process, including the methodology, challenges, and outcomes.

### 2. Semantic Data Model
- **Visual Diagram**: A diagram depicting the classes, relationships, and cardinalities.
- **RDF/OWL Version**: Contains classes and relationships defined for the dataset’s semantic model.
  - **Tool Used**: Protégé
  - **URI Standard**: The classes and relationships used in the semantic model are based on the existing URI from the Ciudades Abiertas Vocabulary for Public Bicycle Transport.

### 3. Semantic Metadata Model (SHACL)
- **Metadata Schemas**: Based on W3C DCAT, covering:
  - **Dataset Metadata**: Title, creator, description, license, etc.
  - **Original Dataset Distribution**: Metadata for the dataset’s original format.
  - **RDF Dataset Distribution**: Metadata for the RDF version of the dataset, with additional distributions for other formats as needed.
- **Tool Used**: FAIR Data Point (FDP) for creating and extracting metadata records.

### 4. Datasets
- **FAIRified Dataset (RDF)**: Available for download from this repository and referenced in distribution metadata using `downloadURL`.

## Repository Structure
```
/
|-- catalog.rdf                     # Metadata record for catalog
|-- dataset.rdf                     # Metadata record for dataset
|-- divvy-bikes.rdf                 # Semantic data model for bikes
|-- divvy-stations.rdf              # Semantic data model for stations
|-- divvy-trips.rdf                 # Semantic data model for trips
|-- original_distribution.rdf       # Metadata for original dataset distribution
|-- rdf_distribution.rdf            # Metadata for RDF dataset distribution
|-- semantic_data_model_general.rdf # Overall semantic data model
|-- shacl dataset.txt               # SHACL schema for dataset
|-- shacl distribution.txt          # SHACL schema for distribution
```

## How to Access the Data
- **Original Dataset**: The original data can be accessed and downloaded from [City of Chicago’s Open Data Portal](https://data.cityofchicago.org/Transportation/Divvy-Trips/fg6s-gzvg/about_data).
- **FAIRified Data**: The RDF version is hosted in this repository.
- **Metadata Records**: Metadata records are extracted from the FAIR Data Point and provided in RDF format.
