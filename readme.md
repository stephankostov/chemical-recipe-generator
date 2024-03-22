# Recipe Generator

Tool to create cooking recipes using data for the molecular composition of ingredients.

# Datasets 

- Recipes: [RecipeNLG](https://recipenlg.cs.put.poznan.pl/)
- Molecular Compositions: [FooDB](https://foodb.ca/)
- Density: [USDA FoodData Central](https://fdc.nal.usda.gov/)
- Molar Masses: [PubChem Compound](https://pubchem.ncbi.nlm.nih.gov/#query=)

Using these, a dataset was created for 1.5 million recipes with an entry of each ingredient with fields for the 5000 measured molecular compound concentrations.

# Development Process

See readme of each section for information.

# Progress

- [x] [Dataset Creation](https://github.com/stephankostov/recipe-generator-dataset)
    - [x] Ingredients -> Density DB's matching
    - [x] Ingredients -> Molecule DB's matching
    - [x] Final Dataset Formatting
    - [x] Dataset analysis
- [ ] [Model Training](https://github.com/stephankostov/recipe-generator)