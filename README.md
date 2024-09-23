# 2024 Sri Lankan Presidential Election Dataset

![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![BeautifulSoup4](https://img.shields.io/badge/BeautifulSoup4-4.12.2-orange?style=for-the-badge&logo=python&logoColor=white)
![Polars](https://img.shields.io/badge/Polars-1.7.1-blue?style=for-the-badge&logo=polars&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-v0.5.4-gold?style=for-the-badge&logo=ruff&logoColor=white)
![UV](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/uv/main/assets/badge/v0.json&style=for-the-badge)

## 📊 Project Overview

This project scrapes and processes data from the 2024 Sri Lankan Presidential Election, creating a comprehensive dataset for analysis. It captures detailed voting information across districts and divisions, offering insights into candidate performance and party standings.

The dataset includes candidate level data for each polling division and the postal votes.
However, [district totals](https://results.elections.gov.lk/district_results.php?district=Colombo) or the [preference vote counts](https://results.elections.gov.lk/district_preference.php?district=Colombo) haven't been included.

## 📁 Dataset Schema

The final dataset (`divisional_results.csv`) includes the following columns:

- `district`: Name of the electoral district
- `division`: Name of the polling division
- `candidate`: Candidate's name
- `party`: Political party abbreviation
- `votes_count`: Number of votes received, in the corresponding polling division, in the corresponding district
- `votes_percentage`: Percentage of votes received, in the corresponding polling division, in the corresponding district

## 🛠️ Stack Breakdown

- **Python**: Core programming language
- **BeautifulSoup4**: Web scraping library
- **Polars**: Fast, efficient dataframes and manipulation library
- **Ruff**: High-performance Python linter
- **UV**: Fast Python package installer and resolver

## 🚀 Getting Started

1. **Clone the repository:**
   ```
   git clone https://github.com/yourusername/2024-lka-pres-election-dataset.git
   cd 2024-lka-pres-election-dataset
   ```

2. **Set up a virtual environment (optional, but recommended):**
   ```
   python -m venv venv
   venv\Scripts\activate 
   ```
   On Unix or Mac, use `source venv/bin/activate`

3. **Install dependencies (using uv as it's much faster than pip):**
   ```
   pip install uv
   uv pip install -r requirements.txt
   ```

4. **Run the Jupyter notebook:**
   ```
   jupyter notebook scrape.ipynb
   ```
   Or open the folder with VSCode and run the cells in the notebook.

5. **Execute the cells to scrape data and generate the dataset.**

6. **The Dataset will be saved as `divisional_results.csv` in the same directory as the notebook.**

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Sri Lanka Elections Commission](https://elections.gov.lk/) for providing the source data.
- The developers of BeautifulSoup4, Polars, Ruff, and UV for their excellent tools.

## 👤 Author

[Govarthenan Rajadurai](https://www.linkedin.com/in/govarthenan)

## 📞 Contact

For any queries or feedback, please open an issue in this repository.

---

⭐ If you find this project useful, please consider giving it a star!
