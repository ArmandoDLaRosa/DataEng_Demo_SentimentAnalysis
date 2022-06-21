
# DataEng ETL - Sentiment Analysis: Hotel Reviews
Context: Have many sources connectors and be able to create ETL for them

## Project Design 
---
[link]()

## Tools 
---
  > :warning: **If you are using ML Models**: Be very careful here! Don't use LFS files for the models.pkl


### Dev Environment
* WSL (Ubuntu 20.04)
* Vscode (Remote Wsl, Python Extension)

## IDEAS
---
- Scrap relevant information and move it to an email
- CDC pattern
- Events
- Stream
- Data Factory
- Create Datasets
  
## VSCODE
### VIRTUAL ENV
0) Make sure you've WSL working in VSCODE and your USER/Root passwords in hand. 
1) Create python environment (venv files should be good inside the project folder)
    ```
    sudo apt install python3-virtualenv
    virtualenv repoName_env
    ```
2) Activate python environment
    ``` 
    source repoName_env/bin/activate
    ```
3) Change in vscode the interpreter `ctrl+shift+p` to the python inside repoName_env/bin/python3.8 
   1) This way you can run the .py with the extension RUN button with the env activated.
   2) Otherwise, you'll have to run it like `python3 fileName.py` and the env activated.

4) Add the folder of the environment to `.gitignore` as `repoName_env_env/`, the requirements you share in git should just be in `requirements.txt`

## .env, config.json file - enviroment variables
1) use the .env.template to create
   * .env.development
   * .env.test
2) You can list the not secret info in config.json

## REQUIREMENTS
Always have your **virtual env** activated
### Load requirements from requirements.txt
* You'll need:
  
    CMD: `sudo apt install python3-pip`

* Load Requirements
  
    CMD: `pip install -r requirements.txt`

### Add new requirements to requirements.txt
[pipreqs documentation](https://github.com/bndr/pipreqs)
* You'll need:
  
    CMD: `pip install pipreqs`

* Load Requirements, while in Project Root    
  
    CMD: `pipreqs ../RepoName/src/folder/config/`

    https://medium.datadriveninvestor.com/complete-data-analytics-solution-using-etl-pipeline-in-python-edd6580de24b?source=user_profile---------0----------------------------

