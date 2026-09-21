CSC2042S 2026: Assignment 2 Logistic Regression News Topic Classification

MasakhaNEWS: News Topic Classification

This project uses the MasakhaNEWS dataset to classify news articles by topic. sI focuses on three languages: English (`eng`), isiXhosa (`xho`) and chiShona (`sna`).

The project implements multinomial logistic regression in PyTorch and investigates different text feature extraction methods, hyperparameters, class imbalance and bilingual training.

Setup

The project was developed in Python using Jupyter Notebook.

The main libraries used are:

* NumPy
* pandas
* scikit-learn
* PyTorch
* matplotlib
* joblib

Install the required packages with:

```bash
pip install numpy pandas scikit-learn torch matplotlib joblib
```

Then open `Assignment.ipynb` in Jupyter Notebook or JupyterLab and run the cells in order.

The project uses the [MasakhaNEWS dataset](https://huggingface.co/datasets/masakhane/masakhanews). The dataset contains news articles from multiple African languages. This project uses English, isiXhosa and chiShona.

## Submitted Files

- Assignment.ipynb:

The main Jupyter Notebook containing the code and analysis for the assignment. It covers data processing, multinomial logistic regression, model training, feature extraction, hyperparameter tuning, weight analysis, isiXhosa class imbalance and bilingual training.

- Project_files:

Contains the data used for the relevant few-shot experiments, feature extraction code used to convert the news text into numerical representations for the models, including Bag-of-Words and TF-IDF features.

- grid_search_results.csv

Contains the results from the hyperparameter search, including the different parameter combinations tested and their development-set performance.

- grid_search_summary.csv

Contains a summary of the selected hyperparameter configuration for each language and feature extraction method.

- README.md

This file contains the setup instructions and descriptions of the submitted files.

- Main Experiments

- The assignment investigates:
Text preprocessing and feature extraction
Multinomial logistic regression using PyTorch
Bag-of-Words and TF-IDF representations
Hyperparameter tuning
Analysis of learned model weights
Upsampling and downsampling for isiXhosa class imbalance
Bilingual training using isiXhosa with chiShona and English
Model evaluation using accuracy, precision, recall and F1 scores

- Dataset

This repository does not include the dataset. The detailed description of the dataset can be found here: https://github.com/masakhane-io/masakhane-news/tree/main

- Citation

If using the MasakhaNEWS dataset, please cite:

```bibtex
@inproceedings{Adelani2023MasakhaNEWSNT,
  title={MasakhaNEWS: News Topic Classification for African languages},
  author={David Ifeoluwa Adelani and Marek Masiak and Israel Abebe Azime and Jesujoba Oluwadara Alabi and Atnafu Lambebo Tonja and Christine Mwase and Odunayo Ogundepo and Bonaventure F. P. Dossou and Akintunde Oladipo and Doreen Nixdorf and Chris Chinenye Emezue and Sana Al-Azzawi and Blessing K. Sibanda and Davis David and Lolwethu Ndolela and Jonathan Mukiibi and Tunde Oluwaseyi Ajayi and Tatiana Moteu Ngoli and Brian Odhiambo and Abraham Toluwase Owodunni and Nnaemeka C. Obiefuna and Shamsuddeen Hassan Muhammad and Saheed Salahudeen Abdullahi and Mesay Gemeda Yigezu and Tajuddeen Rabiu Gwadabe and Idris Abdulmumin and Mahlet Taye Bame and Oluwabusayo Olufunke Awoyomi and Iyanuoluwa Shode and Tolulope Anu Adelani and Habiba Abdulganiy Kailani and Abdul-Hakeem Omotayo and Adetola Adeeko and Afolabi Abeeb and Anuoluwapo Aremu and Olanrewaju Samuel and Clemencia Siro and Wangari Kimotho and Onyekachi Raphael Ogbu and Chinedu E. Mbonu and Chiamaka I. Chukwuneke and Samuel Fanijo and Jessica Ojo and Oyinkansola F. Awosan and Tadesse Kebede Guge and Sakayo Toadoum Sari and Pamela Nyatsine and Freedmore Sidume and Oreen Yousuf and Mardiyyah Oduwole and Ussen Abre Kimanuka and Kanda Patrick Tshinu and Thina Diko and Siyanda Nxakama and Abdulmejid Tuni Johar and Sinodos Gebre and Muhidin Mohamed and Moges Ahmed Mehamed and Evrard Ngabire and Pontus Stenetorp},
  year={2023}
}
```
