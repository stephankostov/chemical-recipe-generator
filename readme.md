# Recipe Generator

Tool to create cooking recipes using data for the molecular composition of ingredients.

# Datasets 

- Recipes: [RecipeNLG](https://recipenlg.cs.put.poznan.pl/)
- Molecular Compositions: [FooDB](https://foodb.ca/)
- Density: [USDA FoodData Central](https://fdc.nal.usda.gov/)
- Molar Masses: [PubChem Compound](https://pubchem.ncbi.nlm.nih.gov/#query=)

Using these, a dataset was created for 1.5 million recipes with an entry of each ingredient with fields for the 5000 measured molecular compound concentrations.


# Development Process

1. Initial development (using small dataframe samples) [./notebooks](./notebooks)
2. Core functions automatically exported into modules using [nbdev](https://nbdev.fast.ai/getting_started.html)
2. Testing framework run [./tests](./full_tests)
3. Full dataframe pipelines [./full_runs](./full_runs)

# Progress

- [x] Dataset Compilation
    - [x] Ingredients -> Density DB's join
    - [x] Ingredients -> Molecule DB's join
    - [x] Final Dataset Formatting
- [ ] Dataset Analysis
- [ ] Model Training