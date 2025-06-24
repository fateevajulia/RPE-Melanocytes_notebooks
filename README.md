# 🧬 Evolutionary Homology Between RPE and Melanocytes

This repository is for the manuscript:

**"Melanocytes and photosensory organs share a common ancestry that illuminates the origins of the neural crest"**  
Yuliia Fatieieva, Rozalina Galimullina, Sergei Isaev, Alexander Klimovich, Laurence A. Lemaire and Igor Adameyko

We provide a multi-modal comparative analysis supporting the homology between neural crest-derived melanocytes and retinal pigment epithelium (RPE). Leveraging single-cell transcriptomics, chromatin accessibility, spatial gene expression, and evolutionary inference, we identify a conserved regulatory and transcriptional core tracing back to a photosensory ancestor.

---

## 🔬 Summary of Findings

- RPE and melanocytes share a deeply conserved gene regulatory and transcriptional program.
- Evolutionary tree reconstruction places them as closest relatives among pigment cell types.
- Ciona's pigmented ocellus expresses overlapping TFs with vertebrate RPE/melanocytes.
- Phylostratigraphy shows that melanocytes and RPE each gained new genes after they split from a common ancestor.
- The findings suggest that pigment cells in the neural crest evolved from an earlier photosensory cell type.

---

## 📁 Repository Contents

| Notebook | Description |
|----------|-------------|
| `Notebook1_a.ipynb`, `1_b.ipynb` | Murine anterior eye chamber scRNA-seq (GSM5560840), RPE/melanocyte subclustering |
| `Notebook2.ipynb` | Shared gene program identification and GO/STRING enrichment |
| `Notebook3_a.ipynb` – `3_e.ipynb` | TF-only dimensionality reduction, CASSIOPEIA tree construction, and SCENIC regulon analysis |
| `Notebook4_a.ipynb` – `4_d2.ipynb` | Human eye development (GSE155121, GSE210543) and mouse spatial Stereo-seq (CNP0001543) |
| `Notebook5_a.ipynb` – `5_c.ipynb` | Tunicate (Ciona intestinalis) pigmented ocellus subclustering and TF-based homology |
| `Notebook6_a.ipynb`, `6_b.ipynb` | Phylostratigraphic analysis of gene age and innovation |
| `Notebook7_a.ipynb` – `7_e.ipynb` | Pinealocyte comparisons and additional skin melanocyte integration |
| `Notebook8_a.ipynb`, `8_b.ipynb` | Auxiliary or intermediate processing (not directly shown in main figures) |
| `Notebook9_a.ipynb`, `9_b.ipynb` | Exploratory or validation analyses not featured in final manuscript |
| `Notebook10_a.ipynb`, `10_a(1).ipynb`, `10_b.ipynb`, `10_b(1).ipynb` | Gene evolutionary age (phylostratigraphy); linked to Figure 10 |
| `Notebook12.ipynb` | Combined dendrogram (RPE, melanocytes, pinealocytes, retina, immune cells) |
| `Notebook_suppl3_j.ipynb` | Supplementary quality controls, batch effect checks, and GO validation |

---

## 📊 Datasets Used

| Dataset | Accession | Description |
|--------|-----------|-------------|
| Murine anterior eye | [GSM5560840](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM5560840) | RPE, melanocytes, and anterior ocular structures |
| Mouse skin melanocytes | [GSE131498](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE131498) | P0 back skin |
|  | [GSE181390](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE181390) | P4 skin |
|  | [GSE203051](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE203051) | Anagen II melanocyte stem cells |
|  | [GSE147298](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE147298) | Quiescent melanocyte stem cells |
| Human fetal eye (early) | [GSE155121](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE155121) | Weeks 4–8 eye development |
| Human fetal eye (late) | [GSE210543](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE210543) | Weeks 12–21 foveal tissue |
| Mouse spatial (Stereo-seq) | [CNP0001543](https://db.cngb.org/search/project/CNP0001543/) | E14.5 and E16.5 mouse embryonic eye |
| Tunicate (Ciona intestinalis) | [GSE131155](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE131155) | Pigmented ocellus and brain primordium |

---

## 🛠️ Tools and Packages

- R: `Seurat`, `DoubletFinder`, `STRINGdb`
- Python: `Scanpy`, `SCENIC`, `Squidpy`, `CASSIOPEIA`, `biomaRt`
- TF classification: AnimalTFDB
- Enrichment: `ShinyGO v0.75`, `STRING v11.5`
- Visualization: `iTOL`, `ggtree`

---

## 🧠 Biological Significance

Our study highlights a developmental and evolutionary link between melanocytes and RPE, two pigment-producing cell types previously thought to have arisen independently. This work supports a scenario in which pigment cells derive from ancestral photosensory lineages, with implications for the origin of the neural crest and evolution of sensory systems in chordates.

---

