# Composition of this archive

- a **training notebook** (`1744946_1753403_notebook_training.ipynb`) that contains the code to train and save the
  models to `dbfs`
- a **demo notebook** (`1744946_1753403_notebook_demo.ipynb`) that loads the models from `dbfs` and performs evaluation,
  runs the search engine on a random image and so on
- a **presentation** (`1744946_1753403_presentation.pdf`) that briefly shows workflow and results although, for brevity
  purposes, you can more find more informations into the notebooks
- this file

# How to run the notebooks

Make sure to do everything on [DataBricks](https://databricks.com/) because these notebooks relies on `dbfs` and an
Internet connection to work

- import and run `1744946_1753403_notebook_training.ipynb` that:
    - will download the required parts of the dataset
    - will train the `base_model` and save it to `dbfs`
    - will pseudo-label the unlabeled part of the dataset
    - will train the `final_model` and save it to `dbfs`
- import and run `1744946_1753403_notebook_demo.ipynb`
    - if you've properly done the previous step, you'll have the models saved to `dbfs` as the two folders `base_model`
      and `final_model`
    - run the notebook
- if you've done everything correctly, you can successfully check the output cells
