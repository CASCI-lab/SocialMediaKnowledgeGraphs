# Social Media Knowledge Graphs for Epilepsy Discourse
## Overview
We provide four social media knowledge graphs (KGs) capturing online epilepsy discourse from the following platforms:
- **X (formerly Twitter)** [Download](https://github.com/CASCI-lab/SocialMediaKnowledgeGraphs/blob/main/X_KG.graphml)
- **Instagram** [Download](https://github.com/CASCI-lab/SocialMediaKnowledgeGraphs/blob/main/Instagram_KG.graphml)
- **Reddit (r/Epilepsy)** [Download](https://github.com/CASCI-lab/SocialMediaKnowledgeGraphs/blob/main/Reddit_KG.graphml)
- **Epilepsy Foundation Forums (EFA)** [Download](https://github.com/CASCI-lab/SocialMediaKnowledgeGraphs/blob/main/EFA_KG.graphml)

## Reference Paper
The methodology and results are described in the following paper:

> **Selecting Focused Digital Cohorts from Social Media Using the Metric Backbone of Biomedical Knowledge Graphs**  
> _arXiv preprint_ [arXiv:2405.07072](https://arxiv.org/abs/2405.07072)

## Network Overview
The image **`KGOverview.png`** provides an overview of the four social media KGs and their corresponding metric backbones.

<img src="KGOverview.png" alt="Network Overview" width="100%">

- **Left Side:** The full knowledge graph for each data source, where all edges are considered.
- **Right Side:** The **metric backbone subgraph**, where only edges with the attribute `'is_metric' = True` are retained.

You can generate these visualizations using the provided KGs.

## Data Availability and Copyright Considerations
### MedDRA & DrugBank Terms
Due to copyright restrictions, we **redacted specific term names** sourced from **MedDRA** (v15.0) and **DrugBank** (v.5.1.0) but provided the **source ID** to allow retrieval for users with appropriate access.

#### Example:
For a node with index `9169`, the attributes are as follows:
```json
{
  "parent": "Redacted",
  "type": "Drug",
  "parent original id": "DB11266",
  "original id source": "DrugBank"
}
```
- The `parent` attribute is a high-level term we used to build KG.
- The `parent original id` corresponds to the DrugBank ID (`DB11266`).
- Users with access to DrugBank can map this ID to the actual term name.

## Fully Available Terms
For sources that **do not** have copyright restrictions, we provide the full term names directly.

## Reproducing the `NetworkPanel` Image
To facilitate reproducibility, we intentionally retained the following key nodes in the provided KGs:

[View the Network Panel Image](NetworklPannel.pdf)

- `Epilepsy`
- `Migraine`
- `Depression`
- `Anxiety`
- `Topiramate`
- `Decreased Appetite`

## Contact and Support
If you encounter any issues using the provided **GraphML** files to generate knowledge graphs, feel free to reach out:
**[zguo29@binghamton.edu](mailto:zguo29@binghamton.edu)**
