# File Reading
Corresponding [slides](https://docs.google.com/presentation/d/1qnDHp74mJa0tDyCRuuzW7TOgqrZeq8LlD3c5zvNxfxw/edit?usp=sharing)  
If reading through these notebooks, follow this order:
# Task 1
## EDA (/eda)
1. Data extraction (./data_extraction.ipynb)
  * Converts 2017 Steam Bundle Data json to csv
2. Explore bundle (./explore_bundle.ipynb)
  * Removes unnecessary columns
  * Exports updated 2017 dataframe to csv
3. Task scratch work (./bundle_task.ipynb)
  * Genre is converted from a string to list
  * Exports updated 2017 dataframe to csv
## Modeling (/modeling)
1. Modeling (./model.ipynb)
  * Generates negative samples for the 2017 data
  * Scratch work for modeling approaches
## Webscraping (/webscraping) 
1. Scraping Steam Bundles (./scrape_bundle_items.ipynb)
  * Selenium for scraping + bs4 for HTML parsing
  * Generates 2025 Steam Bundle data
  * Exports 2025 dataframe to csv (bundle1000.csv)
  * Side note: bundle1000.csv was renamed new_bundle.csv and moved to the import_data folder
# Task 2 
## EDA (/task_2)
1. Data Extraction (./task_2.ipynb)
  * Converts 2018 Steam User and Item Data json to csv
2. Feature Visualization (./task_2_modeling.ipynb)
  * Scatter plots and summary statistics for numeric features
# Data Imports (/import_data)
1. Datasets required for Google Colab notebook
  * Contains 5 csv files
  * Files are renamed copies of csv exports from the notebooks above
# Google Colab Notebook
Accessible [here](https://colab.research.google.com/drive/1IhdHvFRiEDOWrwkiVlP-bFe5f0kh1kyA?usp=sharing)  
Note: You must download the 5 csv files from /import_data and add them to your runtime environment if running the full notebook.
1. Task 1 - Modeling and Analysis
 * Word Embeddings
 * Logistic Regression, Random Forest and SVD approaches to bundles
 * Models trained on 2017 data
 * Models tested on 2017 data
 * Models tested on 2025 data
 * AUC plots + Accuracy metrics available for each model
2. Task 2 - Modeling and Analysis
 * Linear Regression, Ridge Regression and Matrix Factorization approaches to all-time playtime prediction
 * Models trained on 2018 data
 * Prediction Plots + RMSE available for each model
