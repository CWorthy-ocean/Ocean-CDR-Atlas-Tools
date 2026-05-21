# Ocean CDR Atlas Tools

Analysis tools and example notebooks for working with [**[C]Worthy**'s Ocean CDR Atlas](https://source.coop/cworthy) datasets.

> [!NOTE]
> **Work in progress.** This repository is under active development. APIs, notebook layouts, and dataset paths may change without notice.

## Notebooks

| Notebook | Description | Open in Colab |
| --- | --- | --- |
| [`notebooks/ace-efficiency.ipynb`](notebooks/ace-efficiency.ipynb) | Combines OAE and DOR efficiency maps to estimate the ocean response of **combined Alkalinity and CO₂ Enhancement (ACE)** interventions — i.e. enhanced rock weathering (ERW), river alkalinity enhancement (RAE), and accelerated weathering of limestone (AWL). Computes $\gamma_\mathrm{ACE}(t) = \gamma_\mathrm{OAE}(t) - R \cdot \gamma_\mathrm{DOR}(t)$ for a user-selected DIC-to-alkalinity ratio $R$. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CWorthy-ocean/Ocean-CDR-Atlas-Tools/blob/main/notebooks/ace-efficiency.ipynb) |

The notebooks pull data on-demand from Source Cooperative via `s3fs` (anonymous), so no local data setup is required — they run identically on Colab and on a local Python environment.

## Data

Interactive web tools:
- [OAE Efficiency Map](https://carbonplan.org/research/oae-efficiency)
- [DOR Efficiency Map](https://carbonplan.org/research/dor-efficiency)

Datasets:
- [Ocean CDR Atlas: OAE Efficiency Map](https://source.coop/cworthy/oae-efficiency-atlas)
- [Ocean CDR Atlas: DOR Efficiency Map](https://source.coop/cworthy/dor-efficiency-atlas)

## References

- M. Long et al. (2024) "Mapping the efficiency of ocean alkalinity enhancement." CarbonPlan. <https://carbonplan.org/research/oae-efficiency-explainer>
- Chay et al. (2025) "Mapping the efficiency of direct ocean removal." CarbonPlan. <https://carbonplan.org/research/dor-efficiency-explainer>
- Zhou, M., M. Timmermans, E. Yankovsky, M. Tyka, & M. C. Long. *Mapping and intercomparison of ocean-based geochemical carbon dioxide removal efficiency.* Nature Communications, In Review. ([Pre-print](https://drive.google.com/file/d/1Y5Lo7dd-xkY_lAz0Nu9G9zx4INfE3qQi/view?usp=sharing))
- Zhou, M., Tyka, M. D., Ho, D. T., Yankovsky, E., Bachman, S., Nicholas, T., Karspeck, A. R., & Long, M. C. (2025). Mapping the global variation in the efficiency of ocean alkalinity enhancement for carbon dioxide removal. *Nature Climate Change*, 15, 59–65. <https://doi.org/10.1038/s41558-024-02179-9>
- Yankovsky, E., Zhou, M., Tyka, M., Bachman, S., Ho, D. T., Karspeck, A., & Long, M. C. (2025). Impulse response functions as a framework for quantifying ocean-based carbon dioxide removal. *Biogeosciences*, 22, 5723–5739. <https://doi.org/10.5194/bg-22-5723-2025>
