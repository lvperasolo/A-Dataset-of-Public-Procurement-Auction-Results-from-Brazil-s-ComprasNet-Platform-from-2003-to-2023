# A Dataset of Public Procurement Auction Results from Brazil’s ComprasNet Platform (2003–2023)
We aim to facilitate access to a public dataset of procurement auctions conducted via Brazil's Compras.gov.br platform from 2003 to 2023. The data set contains information on auctioned items (detailed description), suppliers' data, dates, and other information that have been extracted from [Data Source: Portal da Transparência](https://portaldatransparencia.gov.br/download-de-dados/licitacoes). We provide a short overview of the data accompanied with unofficial English translation to support accessibility and usability, refer to the .pdf file in this repository for more.

The dataset files are found under the folder `procurement_auction_data/`. Additionally, we provide minimal examples illustrating potential uses of the data. The examples are not curated/optimized (e.g., do not include preprocessing steps, etc) and, thus, must be enhanced/improved for real applicability. 

**Note:** Public procurement in Brazil follows several modalities beyond the focus of this repository, which focuses exclusively on the procurement (reverse) auction modality. Readers interested in other modalities can refer to the same source of information we use ([Data Source: Portal da Transparência](https://portaldatransparencia.gov.br/download-de-dados/licitacoes)) and work with the complete dataset and/or filter for a different modality since the original files have all modalities.

---

## Repository structure
- `Dataset_of_Public_Procurement_Auction_Results_from_Brazil_s_ComprasNet_Platform__2003__2023.pdf`  
  PDF document describing the dataset structure and other information. 
- `procurement_auction_data/`  
  Directory containing the raw CSV data files. Files include:
  - `Participantes.csv` (~1.9 GB)
  - `Itens.csv` (~297 MB)
  - `Empenhos.csv` (~180 MB)
  - `Licitações.csv` (~74 MB)
- `examples/`  
  Collection of additional Jupyter notebooks demonstrating how to work with each dataset:
  - `participants.ipynb`
  - `itens.ipynb`
  - `empenhos.ipynb`
  - `procurement_auction.ipynb`
  
---

## Short data description
The datasets include the following CSV files:

1. **Participantes.csv**
   - ~9.3 M rows, 13 columns
   - Contains information about auction participants and winner flags.

2. **Itens.csv**
   - ~1.36 M rows, 14 columns
   - Details items purchased in each auction, quantities, unit values, and winners.

3. **Empenhos.csv**
   - ~0.74 M rows, 10 columns
   - Commitment (empenho) records indicating approved budget amounts for auctions.

4. **Licitações.csv**
   - ~0.17 M rows, 17 columns
   - Master auction table with metadata such as process numbers, dates, status, and values.

---

## Installation & setup
Setup and installation are not unique. In this section, we explain one way, to make use of this project, other ways also exist-so feel free to play around. 

1. Clone the repository
```bash
git clone https://github.com/lvperasolo/A-Dataset-of-Public-Procurement-Auction-Results-from-Brazil-s-ComprasNet-Platform-from-2003-to-2023.git
cd <your-location> # location in your machine
```
2. (optional) Create our virtual environment 
```python -m venv comprasVENV```

3. (optional) Activate the virtual environment:
```source comprasVENV/bin/activate  # for linux/mac OS```,  or 
```.\comprasVENV\Scripts\Activate.ps1 # for windows OS```

4. (optional) Install our dependencies
```pip install -r requirements.txt```

---
## License
This project is released under the __Creative Commons Attribution 4.0__, __Open Data Commons Open Database License (ODbL) v1.0__ and __Database Contents License (DbCL) v1.0__ licenses.

---
## Citation
If you use this repository or the dataset in your work, please cite it as follows:

### BibTeX
```bibtex
@misc{data2025comprasnet,
  author       = {Vicentim Perasolo, L. and Liepold, C.},
  title        = {A Dataset of Public Procurement Auction Results from Brazil’s ComprasNet Platform (2003–2023)},
  year         = {2025},
  url          = {https://github.com/lperasolo/A-Dataset-of-Public-Procurement-Auction-Results-from-Brazil-s-ComprasNet-Platform-from-2003-to-2023/tree/master},
  version      = {1.0},
  note = {Last updated on 24.09.2025}
}
```

---
## Disclaimer
This repository is a personal project and is not affiliated with, endorsed by, or officially associated with any institution or organization.

---
## Contact
For any inquiries regarding the dataset, code, project feedback or other requests, feel free to reach out to me at my [email](lucas.vicentim-perasolo@tum.de). I will do my best to get back to you in time.
