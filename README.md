# Dataset used for publications related to UNIQmin

### **Tool:** [UNIQmin](https://github.com/ChongLC/MinimalSetofViralPeptidome-UNIQmin) <br>
[![PyPI](https://img.shields.io/pypi/v/uniqmin?logo=pypi)](https://pypi.org/project/uniqmin/)  &nbsp; [![GitHub tag](https://img.shields.io/github/tag/ChongLC/MinimalSetofViralPeptidome-UNIQmin)](https://github.com/ChongLC/MinimalSetofViralPeptidome-UNIQmin/releases/?include_prereleases&sort=semver "View GitHub releases") &nbsp; [![DOI - 10.3390/biology10090853](https://img.shields.io/badge/DOI-10.3390%2Fbiology10090853-2ea44f)](https://doi.org/10.3390/biology10090853) <br>

## Table of contents
- [Protocol paper](#protocol-paper)
  - UNIQmin, an alignment-free tool to study viral sequence diversity across taxonomic lineages: a case study of monkeypox virus
- [Application papers](#application-papers)
  * [UNIQmin application to all viruses](#mapping-the-minimal-set-of-the-viral-peptidome-across-major-viral-taxonomic-lineages)
  * [UNIQmin application to SARS-CoV-2](#negligible-peptidome-diversity-of-sars-cov-2-and-its-higher-taxonomic-ranks)
    - Negligible peptidome diversity of SARS-CoV-2 and its higher taxonomic ranks
- [Citing resources](#citing-resources)
- [Found a bug](#found-a-bug)

## Protocol paper: 
### UNIQmin, an alignment-free tool to study viral sequence diversity across taxonomic lineages: a case study of monkeypox virus
Publication: &nbsp; [![Preprint - bioRxiv](https://img.shields.io/badge/preprint-bioRxiv-brightgreen)](https://www.biorxiv.org/content/10.1101/2022.08.09.503271v2.full)

<!-- 
example: [![DOI - 10.3390/biology10090853](https://img.shields.io/badge/DOI-10.3390%2Fbiology10090853-2ea44f)](https://doi.org/10.3390/biology10090853)
-->
<details>
<summary>Click to view description of the project</summary> 
<br> 

> Sequence changes in viral genomes generate protein sequence diversity that enable viruses to evade the host immune system, hindering the development of effective preventive and therapeutic interventions. Massive proliferation of sequence data provides unprecedented opportunities to study viral adaptation and evolution. Alignment-free approach removes various restrictions, otherwise posed by an alignment-dependent approach for the study of sequence diversity. The publicly available tool, UNIQmin offers an alignment-free approach for the study of viral sequence diversity at any given rank of taxonomy lineage and is big data ready. The tool performs an exhaustive search to determine the minimal set of sequences required to capture the peptidome diversity within a given dataset. This compression is possible through the removal of identical sequences and unique sequences that do not contribute effectively to the peptidome diversity pool. Herein, we describe a detailed four-part protocol (BP1-4) utilizing UNIQmin to generate the minimal set for the purpose of viral diversity analyses at any rank of the taxonomy lineage, using Monkeypox virus (MPX) as a case study. These protocols enable systematic diversity studies across the taxonomic lineage, which are much needed for our future preparedness of a viral epidemic, in particular when data is in abundance and freely available.

</details>
<br>

**Basic Protocols 1, 2 & 3:**

| Taxonomy lineage rank       | Retrieval dataset (r) | Deduplicated dataset (nr) | Minimal dataset | Link to download                 |
|-----------------------------|:---------------------:|:-------------------------:|:---------------:|:--------------------------------:|
| Species: MPX                | 19,423                | 1,245                     | 866             | [![Download](https://img.shields.io/badge/DL-Species-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Species_MPX)](https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Species_MPX)                                               |
| Genus: Orthopoxvirus        | 83,088                | 15,523                    | 9,146           | [![Download](https://img.shields.io/badge/DL-Genus-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Genus_Orthopoxvirus)](https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Genus_Orthopoxvirus)                                       |
| Family: Poxiviridae        | 163,793                | 34,782                    | 25,618          | [![Download](https://img.shields.io/badge/DL-Family-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Family_Poxiviridae)](https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Family_Poxiviridae)                                        |

**Basic Protocol 4:**
| Diversity spectrum              | Virus and selected protein | Link to download |
|---------------------------------|:--------------------------:|------------------|
| Highly conserved (*H* < 1)      | Avian H5N1 PA              | [![Download](https://img.shields.io/badge/DL-Avian_H5N1_PA-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/H5N1_Avian_PA.fasta)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/H5N1_Avian_PA.fasta)    |
| Semi-conserved (1 <= *H* < 2)   | DENV NS3                   | [![Download](https://img.shields.io/badge/DL-DENV_NS3-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/DENV_NS3.fasta)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/DENV_NS3.fasta)         |
| Diverse (2 <= *H* < 3)          | DENV NS2a                  | [![Download](https://img.shields.io/badge/DL-DENV_NS2a-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/DENV_NS2a.fasta)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/DENV_NS2a.fasta)        |
| Extremely diverse (*H* >= 3)    | HIV-1 clade B Nef          | [![Download](https://img.shields.io/badge/DL-HIV_1_clade_B_Nef-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/HIV_1_cladeB_Nef.fasta)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ProtocolPaper/BP4_FactorAnalysis/HIV_1_cladeB_Nef.fasta) |

--- 
## Application papers: 
### UNIQmin application to all viruses: 
### Mapping the minimal set of the viral peptidome across major viral taxonomic lineages
![Status - In progress](https://img.shields.io/badge/status-In%20progress-red)
<!-- 
example: [![DOI - 10.3390/biology10090853](https://img.shields.io/badge/DOI-10.3390%2Fbiology10090853-2ea44f)](https://doi.org/10.3390/biology10090853)
-->
<br> 

### UNIQmin application to SARS-CoV-2: 
### Negligible peptidome diversity of SARS-CoV-2 and its higher taxonomic ranks 
<!-- 
Publication: &nbsp; ![Preprint - Coming soon!](https://img.shields.io/badge/preprint-Coming%20Soon!-yellow)
-->
Publication: &nbsp; [![Preprint - bioRxiv](https://img.shields.io/badge/preprint-bioRxiv-brightgreen)](https://www.biorxiv.org/content/10.1101/2022.10.31.513750v1.full)

<details>
<summary>Click to view description of the project</summary> 
<br> 

> The unprecedented increase in SARS-CoV-2 sequence data limits the application of alignment-dependent approaches to study viral diversity. Herein, we applied our recently published UNIQmin, an alignment-free tool to study the protein sequence diversity of SARS-CoV-2 (sub-species) and its higher taxonomic lineage ranks (species, genus, and family). Only less than 0.5% of the reported SARS-CoV-2 protein sequences are required to represent the inherent viral peptidome diversity, which only increases to a mere ~2% at the family rank. This is expected to remain relatively the same even with further increases in the sequence data. The findings have important implications in the design of vaccines, drugs, and diagnostics, whereby the number of sequences required for consideration of such studies is drastically reduced, short-circuiting the discovery process, while still providing for a systematic evaluation and coverage of the pathogen diversity.

</details>
<br>

**Compression of SARS-CoV-2 datasets across taxonomy lineage ranks, namely sub-species (proteins), species (with and without SARS-CoV-2), genus, and family:**
|    Taxonomy lineage rank: Virus     | Retrieval dataset (r) | Deduplicated dataset (% of r) |                           Minimal dataset (% of r)                          |
|-------------------------------------|-----------------------|-------------------------------|-----------------------------------------------------------------------------|
| Subspecies: SARS-CoV-2 (GISAID)     |      56,340,320       |       1,780,901 (~3.2)        | 273,851 (~0.5) &nbsp; [![Download](https://img.shields.io/badge/DL-Subspecies-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ApplicationPaper_SARS-CoV-2/MinSet_GISAID_SARSCoV2.zip)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ApplicationPaper_SARS-CoV-2/MinSet_GISAID_SARSCoV2.zip)      |
| Species: *SARS-related coronavirus* |      4,669,400        |        480,112 (~10.3)        |      61,819 (~1.3)                                   |
| Genus: *Betacoronavirus*            |      4,689,400        |        485,220 (~10.3)        |      65,117 (~1.3) &nbsp; [![Download](https://img.shields.io/badge/DL-Genus-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ApplicationPaper_SARS-CoV-2/MinSet_NCBI_Betacoronavirus.zip)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ApplicationPaper_SARS-CoV-2/MinSet_NCBI_Betacoronavirus.zip)                               |
| Family: *Coronaviridae*             |      4,733,200        |        506,374 (~10.7)        |      79,414 (~1.7) &nbsp; [![Download](https://img.shields.io/badge/DL-Family-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ApplicationPaper_SARS-CoV-2/MinSet_NCBI_Coronaviridae.zip)](https://github.com/ChongLC/UNIQmin_PublicationData/blob/main/ApplicationPaper_SARS-CoV-2/MinSet_NCBI_Coronaviridae.zip)                                 |

---
## Citing resources
* For original paper, please refer to our MDPI Biology paper: <br>
  [Chong, L.C.; Lim, W.L.; Ban, K.H.K.; Khan, A.M. An Alignment-Iindependent Approach for the Study of Viral Sequence Diversity at Any Given Rank of Taxonomy Lineage. *Biology* 2021, 10, 853. doi: 10.3390/biology10090853](https://www.mdpi.com/2079-7737/10/9/853) 
* For protocol paper, please refer to our preprint: <br> 
  [Chong, L.C.; Khan, A.M. UNIQmin, An Alignment-free Tool to Study Viral Sequence Diversity across Taxonomic Lineages: A Case Study of Monkeypox Virus. *bioRxiv* 2022.08.09.503271. doi: 10.1101/2022.08.09.503271](https://www.biorxiv.org/content/10.1101/2022.08.09.503271v3.full)
* For application paper to all viruses, <br> 
* For application paper to SARS-CoV-2, please refer to our preprint: <br> 
  [Chong, L.C.; Khan, A.M. Negligible Peptidome Diversity of SARS-CoV-2 and its Higher Taxonomic Ranks. *bioRxiv* 2022.10.31.513750. doi: 10.1101/2022.10.31.513750](https://www.biorxiv.org/content/10.1101/2022.10.31.513750v1.full)

---
## Found a bug?
Or would like drop some feedback? <br>
Just [open a new issue](https://github.com/ChongLC/UNIQmin_PublicationData/issues) or send an email to us (lichuinchong@gmail.com).
