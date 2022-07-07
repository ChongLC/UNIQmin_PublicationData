# Dataset used for publications related to UNIQmin

### **Tool:** [UNIQmin](https://github.com/ChongLC/MinimalSetofViralPeptidome-UNIQmin) <br>
[![PyPI](https://img.shields.io/pypi/v/uniqmin?logo=pypi)](https://pypi.org/project/uniqmin/)  &nbsp; [![GitHub tag](https://img.shields.io/github/tag/ChongLC/MinimalSetofViralPeptidome-UNIQmin)](https://github.com/ChongLC/MinimalSetofViralPeptidome-UNIQmin/releases/?include_prereleases&sort=semver "View GitHub releases") <br>

## Table of contents
- [Protocol paper](#protocol-paper)
- [Application papers](#application-papers)
  * [UNIQmin application to all viruses](#mapping-the-minimal-set-of-the-viral-peptidome-across-major-viral-taxonomic-lineages)
  * [UNIQmin application to SARS-CoV-2](#negligible-peptidome-diversity-of-sars-cov-2-and-its-higher-taxonomic-ranks)
- [Citing resources](#citing-resources)
- [Found a bug](#found-a-bug)

## Protocol paper: 
### UNIQmin: an alignment-free tool to study viral sequence diversity across taxonomic lineages
<!-- 
example: [![DOI - 10.3390/biology10090853](https://img.shields.io/badge/DOI-10.3390%2Fbiology10090853-2ea44f)](https://doi.org/10.3390/biology10090853)
-->
<details>
<summary>Click to view description of the project</summary> 
<br> 

> Sequence changes in viral genomes generate protein sequence diversity that enable viruses to evade the host immune system, hindering the development of effective preventive and therapeutic interventions. Massive proliferation of sequence data provides unprecedented opportunities to study viral adaptation and evolution. Alignment-free approach removes various restrictions, otherwise posed by an alignment-dependent approach for the study of sequence diversity. The publicly available tool, UNIQmin offers an alignment-free approach for the study of viral sequence diversity at any given rank of taxonomy lineage and is big data ready. The tool performs an exhaustive search to determine the minimal set of sequences required to capture the peptidome diversity within a given dataset. This compression is possible through the removal of identical sequences and unique sequences that do not contribute effectively to the peptidome diversity pool. Herein, we describe a detailed four-part protocol (BP1-4) utilizing UNIQmin to generate the minimal set for the purpose of viral diversity analyses at any rank of the taxonomy lineage, using Monkeypox virus (hMPXV) as a case study. These protocols enable systematic diversity studies across the taxonomic lineage, which are much needed for our future preparedness of a viral epidemic, in particular when data is in abundance and freely available.

</details>
<br>

**Basic Protocols 1, 2 & 3:**

| Taxonomy lineage rank       | Retrieval dataset (r) | Deduplicated dataset (nr) | Minimal dataset | Link to download                          |
|-----------------------------|:---------------------:|:-------------------------:|:---------------:|:--------------------------------:|
| Species: hMPXV              | 19,423                | 1,245                     | 866             | [![Download](https://img.shields.io/badge/DL-Species-informational?style=flat&logo=docusign&color=0A66C2&link=https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Species_hMPXV)](https://github.com/ChongLC/UNIQmin_PublicationData/tree/main/ProtocolPaper/Species_hMPXV)                                             |
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
<!-- 
example: [![DOI - 10.3390/biology10090853](https://img.shields.io/badge/DOI-10.3390%2Fbiology10090853-2ea44f)](https://doi.org/10.3390/biology10090853)
-->
<br> 

### UNIQmin application to SARS-CoV-2: 
### Negligible peptidome diversity of SARS-CoV-2 and its higher taxonomic ranks 
<!-- 
example: [![DOI - 10.3390/biology10090853](https://img.shields.io/badge/DOI-10.3390%2Fbiology10090853-2ea44f)](https://doi.org/10.3390/biology10090853)
-->
<details>
<summary>Click to view description of the project</summary> 
<br> 

> {Description}

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
  Chong, L.C.; Lim, W.L.; Ban, K.H.K.; Khan, A.M. An Alignment-Independent Approach for the Study of Viral Sequence Diversity at Any Given Rank of Taxonomy Lineage. Biology 2021, 10, 853. https://doi.org/10.3390/biology10090853 
* For protocol paper, <br>
* For application paper to all viruses, <br> 
* For application paper to SARS-CoV-2, <br>

---
## Found a bug?
Or would like drop some feedback? <br>
Just [open a new issue](https://github.com/ChongLC/UNIQmin_PublicationData/issues) or send an email to us (lichuinchong@gmail.com).
