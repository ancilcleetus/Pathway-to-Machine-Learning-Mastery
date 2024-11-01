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

**Note:** Step 01 to 06 need to be done only once

### Step 07: Update repo

- Add content to repo
- Add new packages to poetry (`poetry add <new-package-name>`)
- Update requirements.txt
- Update README.md
- Update Table of Contents

### Step 08: Pull latest changes to Code spaces

- `cd /workspaces/<your repository directory>/` $\implies$ `cd /workspaces/Pathway-to-Machine-Learning-Mastery`
- `git pull origin main`

### Step 09: Publish to GitHub Pages (using ghp-import) $\implies$ 

- `cd /workspaces/<your repository directory>/` $\implies$ `cd /workspaces/Pathway-to-Machine-Learning-Mastery`
- `poetry run jupyter-book build <your book name>` $\implies$ `poetry run jupyter-book build Pathway-to-Machine-Learning-Mastery-Book`
- `git add -A`
- `git commit -m "<commit message>"`
- `git push -u origin main`
- `poetry run ghp-import -n -p -f <your book name>/_build/html` $\implies$ `poetry run ghp-import -n -p -f Pathway-to-Machine-Learning-Mastery-Book/_build/html`

### Step 10: Check your website!

- Check `https://<username>.github.io/<your repository directory>` $\implies$ https://ancilcleetus.github.io/Pathway-to-Machine-Learning-Mastery
