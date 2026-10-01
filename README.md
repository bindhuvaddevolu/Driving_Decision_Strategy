# Driving Decision Strategy (DDS) Based on Machine Learning for an Autonomous Vehicle

## Project Overview

Driving Decision Strategy (DDS) is a machine learning based project
designed to predict driving decisions for an autonomous vehicle.

The project analyzes internal vehicle data such as RPM and speed values
to predict different driving decision classes such as:

- Speed
- Lane Change
- Steering Angle

The project uses a historical vehicle trajectory dataset for training
and testing because real-time vehicle sensors are not available.

---

## Objective

The main objective of this project is to use vehicle internal data
and machine learning techniques to determine an appropriate driving
decision.

The project introduces a DDS approach based on Genetic Algorithm
for selecting optimal features and improving prediction performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Tkinter
- Matplotlib
- Random Forest
- Multilayer Perceptron (MLP)
- Genetic Algorithm
- Genetic Selection

---

## Dataset

The project uses a historical vehicle trajectory dataset.

The dataset contains vehicle-related features such as:

- RPM Average
- RPM Medium
- RPM Maximum
- RPM Standard Deviation
- Speed Average
- Speed Medium
- Speed Maximum
- Speed Standard Deviation

The dataset also contains a `labels` column representing the driving
decision class.

The documented dataset contains 977 trajectory records.

The application uses:

- 781 records for training
- 196 records for testing

---

## Methodology

The project follows these main steps:

1. Upload the historical trajectory dataset.
2. Remove unnecessary trajectory and timestamp fields.
3. Encode the driving decision labels.
4. Split the dataset into training and testing data.
5. Train machine learning models.
6. Evaluate Random Forest and MLP models.
7. Apply Genetic Algorithm based feature selection for DDS.
8. Compare prediction performance.
9. Use the trained model to predict driving decisions for test data.

---

## Machine Learning Models

### Random Forest

Random Forest is used as one of the baseline machine learning
classification algorithms.

The documented implementation uses Random Forest for training and
prediction.

### Multilayer Perceptron (MLP)

A Multilayer Perceptron classifier is used as another machine learning
approach for comparison.

### DDS with Genetic Algorithm

The proposed DDS approach uses Genetic Algorithm based feature
selection with a Random Forest classifier.

The Genetic Algorithm searches for an optimal set of features that
can be used for the driving decision prediction process.

---

## Performance

The documented project results are:

| Algorithm | Prediction Accuracy |
|-----------|----------------------|
| Random Forest | 67% |
| MLP | 48% |
| DDS with Genetic Algorithm | 73% |

The project documentation reports that the DDS approach achieved
73% prediction accuracy on the documented test setup.

---

## Prediction

The trained model can be used with unlabeled test data to predict
driving decisions.

The documented test examples include predictions such as:

- Lane Change
- Steering Angle
- Speed

---

## Project Interface

The project provides a Tkinter-based graphical user interface.

The interface provides options to:

- Upload Historical Trajectory Dataset
- Generate Train & Test Model
- Run Random Forest Algorithm
- Run MLP Algorithm
- Run DDS with Genetic Algorithm
- View Accuracy Comparison Graph
- Predict DDS Type

---

## Project Structure

```text
Driving_Decision_Strategy/
│
├── DDS.py
├── test.py
├── dataset.csv
├── test_data.txt
├── run.bat
├── SCREENSHOTS.docx
└── README.md
