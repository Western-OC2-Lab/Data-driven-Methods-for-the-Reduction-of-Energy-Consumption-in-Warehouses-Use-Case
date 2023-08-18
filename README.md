# Data-driven-Methods-for-the-Reduction-of-Energy-Consumption-in-Warehouses-Use-Case
This is the repository that includes the code of the use case in the paper titled "Data-driven Methods for the Reduction of Energy Consumption in Warehouses: Use-Case Driven Analysis". All the code documentation and methods' definitions are similar to the content of the manuscript published in **Elsevier Internet of Things**: I. Shaer and A. Shami, Data-driven methods for the reduction of energy
consumption in warehouses: Use-case driven analysis, _Internet of Things_ (2023), doi: https://doi.org/10.1016/j.iot.2023.100882.

Before running the code, the following steps need to be followed: 

1. Create the `datasets` and `results` folders in the root directory (on the same levels as `notebooks`).
2. Create the `stats` and `figures` directories in the `results` directory and the `generated` directory in the `datasets` directory.
3. Download the dataset employed for this work, which can be found using this link: https://figshare.com/articles/dataset/CU-BEMS_Smart_Building_Electricity_Consumption_and_Indoor_Environmental_Sensor_Datasets/11726517. This link is included in the data availability subsection in the original manuscript. The `csv` files obtained should be extracted in the `datasets` folder. The path to any of these datasets should follow this convention: `/datasets/{dataset_name}`.

The explanation of each of the notebooks in the `notebook` directory is as follows:
- **preprocessing.ipynb**: The code splits the single-floor data into its constituent zones. Additionally, the data points are defined in frames of 60 continuous minutes. From this point onwards, the analysis is conducted on zone 2 of the 6th floor.
- **1D-CNN.ipynb**: This notebook executes the code that applies the **a1** method in the manuscript. It includes the feature construction process required to generate the inputs used by 1D-CNN models. The rest of the code applies the hyper-parameter optimization (HPO) process of 1D-CNN.
- **a2_method.ipynb**: This notebook executes the features engineering and HPO for the **a2** method, as per the process explained in the manuscript.
- **a3_method.ipynb**: This notebook executes the features engineering and HPO for the **a3** method, as per the process explained in the manuscript. The results for **a1**, **a2**, and **a3** methods are generated in the `results/stats` directory. The results of these methods are reported in **Table 5** in the original manuscript.
- **Best_methods_predictions.ipynb**: This notebook includes the code that executes **a1**, **a2**, and **a3** methods with the best hyper-parameters. The results depicted in **Figures 4 and 5** in the paper are obtained using this notebook.
- **Results_Analysis.ipynb**: This notebook includes the code that generates **Figures 4 and 5** in the original manuscript.
- **Prediction_Analysis.ipynb**: This notebook includes the code that generates the results in **Table 6**.

# Contact-Info

Please feel free to contact me for any questions or research opportunities. 
- Email: shaeribrahim@gmail.com
- Gihub: https://github.com/ibrahimshaer and https://github.com/Western-OC2-Lab
- LinkedIn: [Ibrahim Shaer](https://www.linkedin.com/in/ibrahim-shaer-714781124/)
- Google Scholar: [Ibrahim Shaer](https://scholar.google.com/citations?user=78fAJ_IAAAAJ&hl=en) and [OC2 Lab](https://scholar.google.com/citations?user=ICvnj9EAAAAJ&hl=en)
