# Project Name

A short description of the project. (e.g. *Exploring the iris dataset with scikit-learn*.)

## Features

* [pipenv] for managing packages and virtualenvs in a modern way.
* Batteries included: [pandas], [numpy], and [scipy] already installed.
* ML and statistical learning with [statsmodels] and [scikit-learn].
* Plotting libraries [matplotlib] and [seaborn] included.
* Data testing and validation with [pandera].
* And the [jupyter] metapackage.
* A couple utility packages; [openpyxl] for reading excel file formats, and [ipykernel] to make use of VSCode's Jupyter functionality.

## Quickstart

The only prerequisites for working with this template are `git`, and `pipenv`.

within the project folder run the following to install all dependencies listed in the `pipenv` file:

    pipenv install 

Next, within the project folder run the following to activate the virtualenv:

    pipenv shell

Lastly to ensure the repository level .gitconfig is included:

    git config --local include.path ../.gitconfig


## Directory structure

```
.
├── notebooks            # A directory to place all notebooks files.
│   ├── *.ipynb
│   └── README.md
├── data                 # A directory to place all input and output data files.
│   ├── input/
│   │    └── .gitignore
│   ├── output/
│   │    └── .gitignore
│   └── README.md
├── .gitignore           # Standard python .gitignore
├── .gitattributes
├── .gitconfig
├── pipfile              # The pipfile for reproducing the package environment
├── pipfile.lock 
└── README.md            # This readme.md
```


[pipenv]: https://pipenv.pypa.io/en/latest/
[pandas]: https://pandas.pydata.org/
[numpy]: https://numpy.org/
[scipy]: https://www.scipy.org/
[seaborn]: https://seaborn.pydata.org/
[statsmodels]: https://www.statsmodels.org/stable/index.html
[scikit-learn]: https://scikit-learn.org/stable/index.html
[matplotlib]: https://matplotlib.org/
[pandera]: https://pandera.readthedocs.io/en/stable/
[ipykernel]: https://pypi.org/project/ipykernel/
[openpyxl]: https://pypi.org/project/openpyxl/
[jupyter]: https://pypi.org/project/jupyter/

## Safety

This repo uses a `.gitattributes` and `.gitconfig` to clean all `*.ipynb` cell outputs within the `notebooks/` directory, here's a [link](https://zhauniarovich.com/post/2020/2020-10-clearing-jupyter-output-p3/) to how this is done.

The `data/*` folders both contain a `.gitignore` with a bunch of common data formats listed such as multiple different Excel extensions, csv, parquet extensions, hfd extensions, json, and txt, among others. **You may need to add your extensions here if they're less common.**

This is to ensure the only content commited to a repository is code, and not data.

## Resources

See [this](https://stackoverflow.com/a/54776118) link for naming conventions of notebook files which may work for you.

The following are unofficial third party resources I've found which may be helpful, feel free to add if you come across any!

* [awesome-python-data-science](https://github.com/krzjoa/awesome-python-data-science) - A curated list of packages and resources related to python datascience and multiple subfields.
