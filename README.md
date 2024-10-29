# Pathway-to-Machine-Learning-Mastery
Pathway to Machine Learning Mastery: Complete Machine Learning Course from Ground-Up to Greatness

## [Simplest Way to publish your Jupyter notebooks on the open web: Using jupyter-book and GitHub Pages](https://medium.com/@dr.junghoonson/simplest-way-to-publish-your-jupyter-notebooks-on-the-open-web-using-jupyter-book-and-github-pages-eea144031d6f)

### Step 01: Create your repository and add your notebooks

### Step 02: Use Github Codespaces for Editing

### Step 03: Install poetry

- `pip install -U poetry` from the Codespaces terminal

### Step 04: Initialize the repository with poetry

- `poetry init` from the Codespaces terminal

### Step 05: Install necessary python packages

- `poetry add jupyter-book ipykernel ghp-import numpy pandas scikit-learn matplotlib seaborn plotly rich`

### Step 06: Setup the basic template for jupyter-book

- `cd /workspaces/<your repository directory>/` $\implies$ `cd /workspaces/Pathway-to-Machine-Learning-Mastery`
- `poetry run jupyter-book create <your book name>/` $\implies$ `poetry run jupyter-book create Pathway-to-Machine-Learning-Mastery-Book`

### Step 07: Publish to GitHub Pages (using ghp-import)

- `cd /workspaces/<your repository directory>/` $\implies$ `cd /workspaces/Pathway-to-Machine-Learning-Mastery`
- `poetry run jupyter-book build <your book name>` $\implies$ `poetry run jupyter-book build Pathway-to-Machine-Learning-Mastery-Book`
- `git add -A`
- `git commit -m "<commit message>"`
- `git push`
- `poetry run ghp-import -n -p -f <your book name>/_build/html` $\implies$ `poetry run ghp-import -n -p -f Pathway-to-Machine-Learning-Mastery-Book/_build/html`

### Step 08: Check your website!

- Check https://<username>.github.io/<your repository directory> $\implies$ https://ancilcleetus.github.io/Pathway-to-Machine-Learning-Mastery
