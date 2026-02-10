# Netflix Shows EDA & Similarity Mapping

A simple data visualization project exploring the [Netflix shows dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows) through exploratory analysis and semantic mapping using Natural Language Processing (NLP).

## Overview
* This project analyzes content trends on Netflix through various visualisations. The last visualisation is an interactive scatterplot that groups similar shows together.
* Show descriptions were transformed into high-dimensional embeddings, and **UMAP** was applied to visualise content clusters in a 2D "Semantic Map" to discover similar shows.


## Techniques used
* **Geospatial Analysis:** Visualizing content distribution across the globe using `geopandas`.
* **Data Cleaning:** Handling mismatched categorical data and imputing missing values.
* **NLP Embeddings:** Leveraging `Sentence-Transformers` to encode semantic meaning from show descriptions.
* **Dimensionality Reduction:** Utilizing **UMAP** to project embeddings into 2D space for interactive visualization.
* **Medoid Analysis:** Identifying "Landmark Genres" as navigational anchors within the content clusters.

## Libraries used
* **Data:** Pandas, NumPy, Geopandas
* **Visuals:** Matplotlib, Seaborn, Plotly
* **ML/AI:** Sentence-Transformers, UMAP, Scikit-learn

## Project Structure
```text
.
├── requirements.txt         # Environment dependencies
├── .gitignore               # Files ignored by Git (e.g., venv)
├── data/                    # Dataset files
└── src/
    └── main.ipynb           # Main analysis and visualization notebook
```

## Getting Started

Follow these steps to set up the project environment and run the analysis on your local machine.

### Prerequisites
* Python 3.8 or higher
* `pip` (Python package installer)

### Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/corneliuschee/Netflix-Shows-Dataset-Data-Visualisations.git
   cd Netflix-Shows-Dataset-Data-Visualisations
    ```

2. **Create a virtual environment:**
    ```
    python -m venv netflix_venv
    ```

3. **Install dependencies:**
    ```
    pip install -r requirements.txt
    ```


### Running the Project

Once the dependencies are installed, you can explore the analysis:

1. Launch Jupyter Notebook or VS Code.

2. Open src/main.ipynb.

3. Ensure the Jupyter kernel is set to your virtual environment (netflix_venv).

4. Run all cells to generate the visualizations