# Recipe Generator

Tool to create cooking recipes using data for the molecular composition of ingredients.

# Project Outline

- [Data Engineering](https://github.com/stephankostov/recipe-generator-dataset)
    - Dataset Wrangling in Pandas
        - Homogenising quantity units
        - Structuring appropriately
        - Handling NA values
    - Fuzzy Matching datasets by food name
        - Recipe -> Density DB
        - Recipe -> Molecule DB
        - Created generalised framework for Fuzzy Matching Datasets
    - Feature Engineering 
        - Parsing ingredient features from unstructured ingredient strings with Named Entity Recognition model
        - Feature selection of most relevant molecule compounds based on various criteria
    - Parallelisation of all data processing with distributed data library [Dask](https://www.dask.org/) 
    - Recipe ingredient tokenisation through similarity of their word embedded vectors
- [ML Modelling](https://github.com/stephankostov/recipe-generator-models)
    - Analysis of possible models for the problem
        - Problem split into two: token generation and weight prediction
    - Custom implementation of both autoregressive (GPT) and nonautoregressive (BERT) models in PyTorch
        - Use of moleculer compound dataset in vectorisation of food tokens
        - Change of outputs to suit each problem
    - Model training 
        - Implementation of typical cross-validation training procedure
        - Experiment tracking setup through [Weights & Biases](https://wandb.ai/stephankostov/recipe-generator-tokens-gpt) tooling

# Dataset References

- Recipes: [RecipeNLG](https://recipenlg.cs.put.poznan.pl/)
- Molecular Compositions: [FooDB](https://foodb.ca/)
- Density: [USDA FoodData Central](https://fdc.nal.usda.gov/)
- Molar Masses: [PubChem Compound](https://pubchem.ncbi.nlm.nih.gov/#query=)


# Development Process

See readme of each section for information.



