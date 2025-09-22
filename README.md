# A Dataset of Public Procurement Auction Results from Brazil’s ComprasNet Platform (2003–2023)
We aim to facilitate access to a public dataset of procurement auctions conducted via Brazil's Compras.gov.br platform from 2003 to 2023. The dataset files are found under folder `procurement_auction_data/`. In addition, we also provide minimal examples on how to use the dataset. The examples are not curated / optimized (e.g. do not include preprocessing steps, etc ...). These examples are a short illustration of potential usages of the dataset only and must be enhanced/improved for real applicability. 

*Note:* Brazil's government purchases take form in multiple modalities beyond procurement/reverse auctions. The interested reader in modalities beyond the reverse auction modality, can use the same data collector as our, and do not filter for procurement auctions only (for more information, refer to A_Dataset_of_Public_Procurement_Auction_Results_from_Brazil_s_ComprasNet_Platform__2003__2023.pdf and/or contact owner of this repository).

---

## Repository structure
- `A_Dataset_of_Public_Procurement_Auction_Results_from_Brazil_s_ComprasNet_Platform__2003__2023.pdf`  
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

*Note:* Refer to the provided PDF for full column descriptions and data dictionary. In practice, when reading the .csv files, we used semicolon (`;`) as separator, and `ISO-8859-1` or `cp1252` encodings to address the special characters from the Portuguese language.

---

## Installation & setup
This project uses Python 3.13.1 (see `.procuror/pyvenv.cfg`). To set up a virtual environment and install dependencies:

```bash
# Create and activate virtual environment
python3.13 -m venv .venv
source .venv/bin/activate

# Install required packages (for examples)
pip install pandas matplotlib notebook networkx
```

*Note: You may want to install additional packages (e.g., seaborn) as needed for your analysis and/or do the installation/set up alternatively.*

---

## License
This project is released under the __Creative Commons Attribution 4.0__ license.

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
  note = {Last updated on 31.09.2025}
}
