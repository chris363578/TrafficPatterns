# AADT Traffic Pattern Analysis using Unsupervised Learning

This repository contains a set of Jupyter Notebooks that analyze Annual Average Daily Traffic (AADT) data using unsupervised machine learning techniques. The goal is to uncover patterns in traffic behavior and identify anomalous count stations using clustering and anomaly detection models.

## Project Structure

| File | Description |
|------|-------------|
| `data.ipynb` | Loads the original AADT dataset and provides an overview of its structure. |
| `clean.ipynb` | Cleans, preprocesses, and transforms the AADT data for downstream analysis. |
| `kmeans.ipynb` | Applies the K-Means clustering algorithm to group count stations based on traffic patterns. |
| `iforest.ipynb` | Uses the Isolation Forest algorithm to detect anomalies in the dataset. |
| `analysis.ipynb` | Contains visualizations and final interpretations combining both clustering and anomaly detection outputs. |

## Methodology

- **Data Cleaning**: Removal of missing values, irrelevant columns, and feature engineering for improved clustering.
- **K-Means Clustering**: Stations are grouped into clusters based on similarities in traffic counts and metadata.
- **Isolation Forest**: Outlier detection is used to highlight count stations with extremely high or low AADT values.
- **Visualization**: Includes cluster distribution by region and violin plots of log-scaled AADT.

## Key Insights

- Cluster patterns reveal geographical or volume-based groupings.
- Isolation Forest successfully detects both high-traffic hubs and underused locations as outliers.
- Combined analysis helps in identifying both common and exceptional traffic behavior across the state.

## Dependencies

- Python 3.8+
- Jupyter Notebook
- `pandas`
- `matplotlib`
- `scikit-learn`
- `seaborn`

To install required packages:

```bash
pip install -r requirements.txt
