 ## * הסבר בעברית כיצד להשתמש במודלים הסופיים ולהוריד את המודלים מהדרייב מוצג בתחתית

-----

# Advanced Deep Learning Final Project: COVID-19 Tweet Sentiment Classification

This repository contains the final project for the **Advanced Deep Learning** course, focusing on training a language model for sentiment classification of COVID-19-related tweets. The project explores various training methodologies, model compression techniques, and model selection to achieve an efficient and accurate final model.

## 📁 Repository Structure

The repository is organized into the following main components:

  - **`notebooks/`**: Contains all the Jupyter Notebooks used for the project's development.
  - **`notebooks/final_models/`**: Stores the trained model weights and compressed models.
  - **`notebooks/data/`**: Holds the various datasets used for training, validation, and testing.

## 🚀 Getting Started

To run the notebooks and use the models, please install the required libraries listed in `requirements.txt`.

```bash
pip install -r requirements.txt
```

## 📝 Project Notebooks

The project's workflow is documented across six Jupyter Notebooks, each serving a specific purpose:

1.  **`1-EDA.ipynb`**: This notebook covers the complete Exploratory Data Analysis (EDA) process, including data cleaning, visualization, and initial insights.
2.  **`2-Training_exc_4.ipynb`**: This notebook trains the models using the methodology from Exercise 4 of the course.
3.  **`3-Training_exc_5.ipynb`**: This notebook trains the models using the methodology from Exercise 5 of the course.
4.  **`4-models_compression.ipynb`**: This notebook details the process of compressing (kivutz) the trained models to reduce their size and computational requirements.
5.  **`5-models_selection.ipynb`**: This notebook is dedicated to selecting the best-performing models based on various evaluation metrics.
6.  **`6-load_final_models.ipynb`**: This notebook provides a simple code example for loading and using the final, selected models for inference.

## 💾 Models and Data

### Models

The base models are saved as `.pt` weight files. For each base model, several compression methods were applied, with the resulting checkpoints saved in dedicated folders within the `final_models/` directory. You can use the `6-load_final_models.ipynb` notebook as a guide to load and use these models.

### Datasets

The `data/` folder contains various `.csv` files for different stages of the project. The primary dataset used for final model selection and evaluation is **`test_clean.csv`**.


### הסבר בעברית לשימוש במודלים הסופיים והורדה מהדרייב של המודלים.
כנס לקישור הורדת המודלים למטה ותוריד את כל התיקייה - תחלץ את התיקייה לתוך התיקייה notebooks
צריך שתיהיה תיקייה בשם final_models שמכילה את כל הקבצים שבקישור בתוך תיקיית notebooks - כלומר notebooks/final_models/

קישור להורדת המודלים:  https://drive.google.com/drive/folders/13-JSc4De9HwPZ-rNOMpybMISRcGoh8E6?usp=sharing 

לאחר שסיימת להוריד את הקבצים כנס לתיקייה notebooks ותפתח את הקובץ  load_final_models.ipynb

כנס לקובץ load_final_models.ipynb יש שם קוד מוכן לפתיחת המודלים. וודא שיש לך את כל החבילות והגרסאות הנכונות כמו ב- requrments.txt וזהו אפשר להריץ את הקוד והוא ידפיס בתחתית העמוד דאטהפריים של כל המודלים והתוצאות שלהם על הטסט.
קובץ הטסט נמצא בתיקייה data בשם train_clean.csv (אפשר להשתמש בקובץ אחר אבל צריך לשים לב שיהיו עמודות text ו- label בלבד!)
