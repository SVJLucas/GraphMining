


## Introduction
The intersection of genetics and disease pathology represents a critical area of biomedical research, with the potential to significantly advance our understanding of disease mechanisms and inform the development of targeted therapies. The Stanford Biomedical Network Dataset Collection provides a comprehensive resource for exploring this intersection, offering detailed datasets on gene-disease associations, disease classifications, and gene annotations. This work utilizes Graph Neural Networks (GNNs) to delve into the intricate relationships captured within these datasets and the _Knowledge Graph_ we constructed from them. Our primary focus is on the disease-gene association network, aiming to perform **Knowledge Graph Completion**. Through this process, we strive to discover new connections between diseases and genes, enriching our understanding of their relationships.

The Graph Neural Networks (GNNs), a class of deep learning models designed for graph data, are well-suited to model the intricate, non-linear relationships present in biological data. By representing genes and diseases as nodes and their associations as edges, GNNs can learn from the topology of the network as well as node and edge attributes, enabling the identification of novel gene-disease links and the prediction of disease phenotypes based on genetic data.

This study aims to harness the disease-gene association network dataset, containing information on 7,813 nodes and 21,357 edges, to uncover patterns and associations that may not be immediately apparent through traditional analysis methods.

## The Dataset

<p align="center">
  <img src="https://github.com/user-attachments/assets/532bdfca-4c5b-4ebc-a88a-27f52032ca27" alt="SNAP Logo" height="300px" />
</p>

The Stanford Biomedical Network Dataset Collection encompasses a rich compilation of biomedical datasets, containing information of drugs, proteins, cells, tissues, etc. We will focus on gene-disease connections. This section elaborates on the composition of the disease and gene datasets within the collection.

### Disease Datasets

The disease datasets are comprehensive, incorporating disease names, definitions, synonyms, and mappings to disease categories. These datasets serve as a fundamental resource for understanding the molecular basis and classification of various diseases:

- **Disease Descriptions and Synonyms**: Derived from the Disease Ontology, this dataset (1.7MB, `D-DoMiner_miner-diseaseDOID`) contains detailed descriptions and features of diseases. It is an essential tool for annotating disease-related information with standardized ontology terms.
- **Disease Descriptions**: Focusing on molecular diseases and environmentally influenced medical conditions, this dataset (3.3MB, `D-MeshMiner_miner-disease`) provides synopses, including names, definitions, and synonyms of diseases. It draws references from the Comparative Toxicogenomics Database and the MINER network, highlighting its utility in understanding disease mechanisms and associations.
- **Classification of Diseases into Disease Categories**: This dataset (15KB, `D-DoPathways_diseaseclasses`) offers a mapping of diseases to their respective categories, based on etiology and anatomical location. It includes diverse examples such as Marfan syndrome (monogenic diseases), rheumatoid arthritis (musculoskeletal system diseases), and liver neoplasms (cancers), facilitating a structured approach to disease classification.

### Gene Datasets
- **Gene Names, Descriptions, and Synonyms**: This dataset (12MB, `G-SynMiner_miner-geneHUGO`) comprises information on 35,000 human genes, including their names, descriptions, synonyms, familial relationships, and chromosomal locations. It forms the backbone of our gene-centric analyses, enabling the exploration of gene functions, relationships, and their roles in diseases.

### Disease-gene Association Network
This dataset (`DG-AssocMiner_miner-disease-gene`, 818KB) represents a disease-gene association network that encapsulates information on genes associated with diseases. In the first sketch of our Knowledge Graph (KG), we define that genes and disease correspond to nodes, and edges denote the associations between them. It provides a structured means to analyze the network of disease-gene interactions.

#### Dataset Statistics
- Number of Nodes: 7,813
  - Disease Nodes: 519
  - Gene Nodes: 7,294
- Number of Edges: 21,357

This collection provides a comprehensive framework for our study. The disease datasets, with their rich descriptive and classificatory information, combined with the gene datasets' extensive coverage of gene attributes, offer an opportunity to explore and predict gene-disease relationships.













# Large Scale Graph Mining

## Overview
The proliferation of complex networked data across diverse domains such as biology, social networks, economics, and communication systems has challenged conventional data analysis methods. This complexity, characterized by intricate connections and dynamic interactions among network components, necessitates the development of new analytical frameworks. Enter network science, an interdisciplinary field that leverages mathematical, computational, and social science theories to understand and analyze these complex structures. It focuses on creating algorithms and models that can map network topologies, assess node influence, and interpret the evolution of these networks over time, thus providing insights into the fundamental processes shaping these interconnected systems.

Central to network science is the exploration of centrality measures, random walks, PageRank algorithms, and the application of machine learning techniques like Graph Neural Networks (GNNs) for advanced network analysis. These tools are instrumental in identifying key nodes, predicting network behaviors, and uncovering community structures within networks. Moreover, network science addresses critical problems such as community detection and influence maximisation, aiming to delineate natural groupings within networks and optimize the spread of information. As networked systems become increasingly integral to various aspects of life and technology, the contributions of network science are invaluable for deciphering and leveraging the complexities of these vast data landscapes.

## Main Topics
- Foundations of network science
- Centrality metrics, Random Walk & PageRank
- Classical algorithms for community detection and influence maximisation
- Machine learning with Graph Neural Networks (GNNs)


## Mini-Project 
The purpose of the project is to compare traditional and ML approaches for community detection and influence maximisation problems on real datasets.
