# Post-Graduation Admission Predictor

Kaggle Dataset Card: [Kaggle](https://www.kaggle.com/datasets/mohansacharya/graduate-admissions)

## Objective

* Develop a predictive model to estimate the likelihood of a student's post-graduation application being accepted.

* Identify the key factors that can enhance a student's chances of acceptance.

* Determine if there is a singular decisive factor that can influence the acceptance or rejection of a student's application.

## Getting the Dataset

1. Visit [Kaggle](https://www.kaggle.com/datasets/mohansacharya/graduate-admissions)

2. _Sign Up_ or _Sign In_ to your Kaggle Account and simply download the CSV file named __Admission_Predict_Ver1.1.csv__.

3. _(Optional)_ Rename the dataset to something simple like `dataset.csv`

## About the Dataset

The CSV file contains 500 rows columns with 9 columns. First column is the Serial Number of the application so we can discard it. The remaining 8 columns are as follows:

1. _GRE Score_ (out of 340)
2. _TOEFL Score_ (out of 120)
3. _University Rating_ (out of 5)
4. _Statement of Puropose Rating_ (out of 5)
5. _Letter of Recommendation Rating_ (out of 5)
6. _GPA Score_ (out of 10)
7. _Research Experience_ (0 for `No` and 1 for `Yes`)
8. _Chance of Admit_ (a decimal value between 0 and 1)

Columns 1 through 7 are the predictors or features of our model and Column 8 is our target variable.

> [!TIP]
> You can change the datatypes of the features to reduce your memory footprint while developing the model.

## Notebooks

|    Notebook                          |    Description                    |
| ------------------------------------ | --------------------------------- |
| [scikit-learn](./scikit-learn.ipynb) | Using only `scikit-learn` package |

## Setup Environment

I have used __Python 3.11__ on a Ubuntu 22.04 machine.

### Method 1: Setup environment on your local machine

1. Clone the repository:
```bash
git clone https://github.com/arnabd64/Graduate-Admission-Prediction.git
cd Graduate-Admission-Prediction
```

2. Setup a python virtual environment using `virtualenv` or `conda`.
```bash
# using virtualenv
python -m venv .venv

# using conda
conda create -n predict python=3.11

# activate the environment
conda activate predict      # when using conda
source .venv/bin/activate   # virtualenv on GNU/Linux or MacOS
.venv/Scripts/Activate.ps1  # virtualenv on Windows
```

3. Install the python packages from `requirements.txt` by executing `pip install -r requirements.txt`

4. Your environment is ready

### Method 2: Using Google Colab or Kaggle

At the beginning of the notebook, add the following command in a new cell and execute it:
```jupyter
!pip install scikit-learn seaborn
```

### Method 3: Using Dev Containers on VS Code

> [!IMPORTANT]
> This method requires the following prerequisites:
> * __Docker__ installed on your local machine.
> * Extensions: __GitHub__ and __Dev Containers__ installed on your Visual Studio Code.
> * Your Visual Studio Code installation being connected with your Github account for seamless git pull/push operations.

1. Open VS Code and press: `Ctrl` + `Shift` + `P` and type in _Clone Repository in a Named Container_.
2. First select _Github_ as the source and then `arnabd64/Graduate-Admission-Prediction` as the name of the repo.
3. Follow the steps provided by VS code and environment will be setup for you.  