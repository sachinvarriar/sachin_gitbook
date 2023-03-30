---
description: >-
  Before we start building a successful MLOps implementation we need to set up
  the necessary tools, libraries and folder structures for easy delivery of
  models. The current notes are for Windows OS
---

# Setting up your first MLOps project

* Set up a local instance of git. You can download the windows installer [here](https://git-scm.com/download/win)
* Install cookiecutter which will hep you get the folder structure template for a standard MLOps project.  The structure of your folder would look similar to this.&#x20;

```
.
├── LICENSE
├── README.md
├── data
│   └── README.md
├── metadata.yaml
├── models
│   └── README.md
├── notebooks
│   └── README.md
├── requirements.txt
├── results
│   └── README.md
└── src
    ├── scripts
    │   └── README.md
    └── tests
        ├── README.md
        └── test_australia_weather_prediction.py

7 directories, 11 files
```

pip could be used to install cookiecutter. It is recommended to install this in a virtual environment. Feel free to ignore --user if you are using your personal laptop

```
pip install --user cookiecutter
```

or

```
pip3 install --user cookiecutter
```

* Install poetry for better package management. Poetry helps in managing packages and sub-packages or dependencies better and makes it easier to add and remove python libraries. Follow the instruction [here ](https://python-poetry.org/docs/)for installation of poetry
