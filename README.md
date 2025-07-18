# A Dataset of Public Procurement Auction Results from Brazil’s ComprasNet Platform (2003–2023)

## Overview
This repository contains a dataset and a minimal exploratory analysis of public procurement auctions conducted on Brazil's ComprasNet platform between 2003 and 2023. The goal is to provide easy access to the raw data and accompanying Jupyter notebooks for minimal examples of potential usage.

## Repository Structure

- `A_Dataset_of_Public_Procurement_Auction_Results_from_Brazil_s_ComprasNet_Platform__2003__2023.pdf`  
  PDF document describing the dataset schema and metadata.
- `procurement_auction_data/`  
  Directory containing the raw CSV data files (ignored by Git due to size). Files include:
  - `Participantes.csv` (~1.9 GB)
  - `Itens.csv` (~297 MB)
  - `Empenhos.csv` (~180 MB)
  - `Licitações.csv` (~74 MB)
- `data_summary.ipynb`  
  Notebook that loads the CSV files, computes summary statistics, and generates LaTeX tables.
- `examples/`  
  Collection of additional Jupyter notebooks demonstrating how to work with each dataset:
  - `participants.ipynb`
  - `itens.ipynb`
  - `empenhos.ipynb`
  - `procurement_auction.ipynb`

## Data Description

The datasets include the following CSV files with semicolon (`;`) as the separator and `cp1252` encoding:

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

Refer to the provided PDF for full column descriptions and data dictionary.

## Installation & Setup

This project uses Python 3.13.1 (see `.procuror/pyvenv.cfg`). To set up a virtual environment and install dependencies:

```bash
# Create and activate virtual environment
python3.13 -m venv .venv
source .venv/bin/activate

# Install required packages
pip install pandas matplotlib notebook networkx
```

*Note: You may want to install additional packages (e.g., seaborn) as needed for your analysis.*

## Usage

1. Activate the virtual environment:

   ```bash
   source .venv/bin/activate
   ```

2. Start Jupyter Notebook or Lab:

   ```bash
   jupyter notebook  # or jupyter lab
   ```

3. Open and run `data_summary.ipynb` to reproduce the summary tables.
4. Explore the `examples/` notebooks for detailed usage patterns on each dataset.

## Contribution

Contributions are welcome! Please fork the repository and submit pull requests for bug fixes, enhancements, or additional examples.

## License

This project is released under the __Creative Commons Attribution 4.0__ license.

## Citation
TODO:

<!-- If you use this repository or the dataset in your work, please cite it as follows: -->

<!-- ### APA

Vicentim Perasolo, L. (2025). _A Dataset of Public Procurement Auction Results from Brazil's ComprasNet Platform (2003–2023)_ [Dataset]. GitHub repository. https://github.com/lperasolo/A-Dataset-of-Public-Procurement-Auction-Results-from-Brazil-s-ComprasNet-Platform-from-2003-to-2023/tree/master

### BibTeX

```bibtex
@misc{perasolo2025comprasnet,
  author       = {Vicentim Perasolo, L.},
  title        = {A Dataset of Public Procurement Auction Results from Brazil’s ComprasNet Platform (2003–2023)},
  year         = {2025},
  howpublished = {GitHub repository},
  url          = {https://github.com/lperasolo/A-Dataset-of-Public-Procurement-Auction-Results-from-Brazil-s-ComprasNet-Platform-from-2003-to-2023/tree/master},
}
```  -->