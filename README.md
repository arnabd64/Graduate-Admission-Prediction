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

Create a cell, and add the following command:
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