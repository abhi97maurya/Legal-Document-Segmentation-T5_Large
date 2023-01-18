### Experiments

We considered the task of classifying sentences in Legal Documents based on their respective rhetorical roles.

In this model we have modified in the following way:
1. Bert-base-uncased model and tokenizer replaced with T5-large model and tokenizer

### 1 Data Download

There are two files:
- [Training Data](https://storage.googleapis.com/indianlegalbert/OPEN_SOURCED_FILES/Rhetorical_Role_Benchmark/Data/train.json)

- [Validation Data](https://storage.googleapis.com/indianlegalbert/OPEN_SOURCED_FILES/Rhetorical_Role_Benchmark/Data/dev.json)


### 2 Run Models on dev data
#### 2.1 Install Dependencies
Python 3.8

To install the requirements,follow the instructions
```
pip install -r requirements.txt
```

## 3 Training Baseline Model on train data

For training model on train data, follow steps

### 3.1 Preprocessing

  Go inside Project folder
  Run the following command

  ```
  python tokenize_files.py train.json dev.json
  ```

### 3.2 Run Training
Go inside Project folder
Run the following command
  ```
   python baseline_run.py
  ```
