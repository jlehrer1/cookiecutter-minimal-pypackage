# Cookiecutter Minimal PyPackage

A quick way to get started on writing simple PyPi packages.

To use, run
```
cookiecutter https://github.com/jlehrer1/cookiecutter-minimal-pypackage
```

I highly recommend aliasing the above command.

Generated file strucure
```
.
├── LICENSE										<-- Project License
├── Makefile									<-- Makefile for cleaning up package files and generating new ones quickly
├── README.md
├── requirements_dev.txt						<-- Used to generate a dev env with `conda install (FIX)`
├── setup.cfg									<-- Required for PyPi, setup when project structure is generated
├── setup.py									<-- Similar to above
├── tests										<-- pytest test files 
│   ├── __init__.py
│   └── test_{{cookiecutter.project_slug}}.py
├── tox.ini
└── {{\ cookiecutter.project_slug\ }}			<-- Source code for project	
    ├── __init__.py
    └── {{\ cookiecutter.project_slug\ }}.py

```
