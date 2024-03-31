# Predicting heart disease using machine learning 🫀

This notebook looks into using various Python-based machine learning and data science librariesin an attempt to build a machine learning model capable of predictiong wheter or not someone has heart disease based on their medical attributes.

## 1. Problem Definition

In a statement, 
> Given clinical parameters about a patient, can we predict whether or not they have heart disease?

## 2. Data

The original data came from the [Cleveland database](https://archive.ics.uci.edu/ml/datasets/heart+Disease) from UCI Machine Learning Repository.

Howevever, I've downloaded it in a formatted way from [Kaggle](https://www.kaggle.com/datasets/sumaiyatasmeem/heart-disease-classification-dataset).

The original database contains 76 attributes, but here only 14 attributes will be used. **Attributes** (also called **features**) are the variables what I'll use to predict our **target variable**.

## 3. Evaluation

> If we can reach 95% accuracy at predicting whether or not a patient has heart disease during the proof of concept, we'll pursure this project.

## 4. Features

### Heart Disease Data Dictionary

The following are the features we'll use to predict our target variable (heart disease or no heart disease).

1. age - age in years 
2. sex - (1 = male; 0 = female) 
3. cp - chest pain type 
    * 0: Typical angina: chest pain related decrease blood supply to the heart
    * 1: Atypical angina: chest pain not related to heart
    * 2: Non-anginal pain: typically esophageal spasms (non heart related)
    * 3: Asymptomatic: chest pain not showing signs of disease
4. trestbps - resting blood pressure (in mm Hg on admission to the hospital)
    * anything above 130-140 is typically cause for concern
5. chol - serum cholestoral in mg/dl 
    * serum = LDL + HDL + .2 * triglycerides
    * above 200 is cause for concern
6. fbs - (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false) 
    * '>126' mg/dL signals diabetes
7. restecg - resting electrocardiographic results
    * 0: Nothing to note
    * 1: ST-T Wave abnormality
        - can range from mild symptoms to severe problems
        - signals non-normal heart beat
    * 2: Possible or definite left ventricular hypertrophy
        - Enlarged heart's main pumping chamber
8. thalach - maximum heart rate achieved 
9. exang - exercise induced angina (1 = yes; 0 = no) 
10. oldpeak - ST depression induced by exercise relative to rest 
    * looks at stress of heart during excercise
    * unhealthy heart will stress more
11. slope - the slope of the peak exercise ST segment
    * 0: Upsloping: better heart rate with excercise (uncommon)
    * 1: Flatsloping: minimal change (typical healthy heart)
    * 2: Downslopins: signs of unhealthy heart
12. ca - number of major vessels (0-3) colored by flourosopy 
    * colored vessel means the doctor can see the blood passing through
    * the more blood movement the better (no clots)
13. thal - thalium stress result
    * 1,3: normal
    * 6: fixed defect: used to be defect but ok now
    * 7: reversable defect: no proper blood movement when excercising 
14. target - have disease or not (1=yes, 0=no) (= the predicted attribute)

**Note:** No personal identifiable information (PPI) can be found in the dataset.

## Running the Code

To run the code, you'll need to set up a Python environment with the necessary dependencies. We recommend using Conda to manage your environment.

### Setting up the Environment

1. First, make sure you have [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) installed on your system.

2. Clone or download this repository to your local machine.

3. Navigate to the project directory in your terminal or command prompt.

4. Create a new Conda environment using the provided `environment.yml` file. Run the following command:

    ```
    conda env create -f environment.yml
    ```

5. Activate the newly created environment:

    ```
    conda activate <env_name>
    ```

    Replace `<env_name>` with the name of the environment specified in the `environment.yml` file.

### Running the Notebook

Once the environment is set up, you can now run the Jupyter notebook containing the code and analysis.

1. With the Conda environment activated, launch Jupyter Notebook:

    ```
    jupyter notebook
    ```

2. This will open a new browser window or tab with the Jupyter Notebook interface. Navigate to the directory where you saved the notebook file (`predicting_heart_disease.ipynb`) and open it by clicking on it.

3. Follow the instructions and execute the cells in the notebook to reproduce the analysis and results.

### Deactivating the Environment

After you've finished running the notebook, you can deactivate the Conda environment:




