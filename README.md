# File Reading
If reading through these notebooks, follow this order:
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
## Webscraping (/webscraping) -- independent of EDA and Modeling
1. Scraping Steam Bundles (./scrape_bundle_items.ipynb)
  * Selenium for scraping + bs4 for HTML parsing
  * Generates 2025 Steam Bundle data
  * Exports 2025 dataframe to csv (bundle1000.csv)
  * Side note: bundle1000.csv was renamed new_bundle.csv and moved to the import_data folder
## Data Imports (/import_data)
1. Datasets required for Google Colab notebook
  * Contains 4 csv files
  * Files are renamed copies of csv exports from the notebooks listed above
## Google Colab Notebook
Accessible [here](https://colab.research.google.com/drive/1IhdHvFRiEDOWrwkiVlP-bFe5f0kh1kyA?usp=sharing)
Note: You must download the 4 csv files from /import_data and add them to your run time environment if running the full notebook.
1. Modeling and Analysis
 * Logistic Regression, Random Forest and SVD approaches to bundles
 * Models trained on 2017 data
 * Models tested on 2017 data
 * Models tested on 2025 data
 * AUC plots + Accuracy metrics available for each model
