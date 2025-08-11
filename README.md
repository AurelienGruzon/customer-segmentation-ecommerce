# Customer Segmentation for Olist (E-commerce)

## Project Overview
This project was carried out as part of a data science mission for **Olist**, a Brazilian e-commerce marketplace solution.  
The goal was to segment customers into actionable groups based on their purchasing behavior and satisfaction, enabling the marketing team to target campaigns more effectively.

In addition to the segmentation, an **analysis of the update frequency** was performed to recommend how often the model should be refreshed to remain relevant.

---

## Objectives
- Import and store data from CSV files into a **PostgreSQL** database.
- Write SQL queries to extract relevant features from customer data.
- Apply **unsupervised learning techniques** (e.g., clustering) to segment customers.
- Combine RFM metrics with satisfaction scores and other relevant features.
- Provide actionable segment descriptions for the marketing team.
- Recommend an optimal frequency for model updates.

---

## Data
The dataset contains anonymized information from January 2017, including:
- Order history
- Purchased products
- Customer satisfaction reviews
- Customer location

---

## Tech Stack
- **Languages**: Python (PEP8 compliant), SQL
- **Database**: PostgreSQL
- **Libraries**: pandas, numpy, scikit-learn, SQLAlchemy, matplotlib, seaborn
- **Tools**: Jupyter Notebook, pgAdmin, Poetry for dependency management

---

## Methodology
1. **Data Ingestion**
   - Imported CSV data into PostgreSQL.
   - Verified data integrity and applied necessary cleaning.

2. **SQL Feature Extraction**
   - Created queries to aggregate and prepare features for clustering.
   - Implemented RFM metrics and additional behavioral variables.

3. **Exploratory Data Analysis (EDA)**
   - Visualized distributions and relationships.
   - Identified patterns and outliers.

4. **Clustering**
   - Tested different algorithms (e.g., K-Means) and hyperparameters.
   - Selected the most stable and interpretable model.

5. **Segment Profiling**
   - Labeled segments with actionable descriptions.
   - Compared performance against marketing needs.

6. **Model Update Simulation**
   - Simulated how segment composition changes over time.
   - Recommended an update frequency to maintain accuracy.

---

## Deliverables
- **Notebook 1**: SQL queries for dashboard integration
- **Notebook 2**: EDA and clustering approach trials
- **Notebook 3**: Model update simulation
- **Presentation**: Segmentation logic and marketing recommendations

---

## Repository Structure
data/             # Raw CSV files (ignored in .gitignore)
notebooks/        # Jupyter notebooks
src/              # Python scripts (data loading, SQL queries, clustering)
livrables/        # Final reports, presentations, exports
.env              # Environment variables (DB connection string)
pyproject.toml    # Poetry dependencies
poetry.lock       # Locked dependency versions

---

## How to Run
1. **Clone the repository**
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>

2. **Install dependencies**
   poetry install

3. **Set environment variables**
   - Create a `.env` file with your database connection string:
     DATABASE_URL=postgresql+psycopg2://user:password@localhost:5432/olist

4. **Run notebooks**
   poetry run jupyter notebook

---

## Contact
For questions or collaboration, feel free to connect:  
[LinkedIn](www.linkedin.com/in/aurelien-gruzon-0b07a62b3) | [Email](mailto:aureliengruzon@gmail.com)
