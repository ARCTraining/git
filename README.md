# Research Software Development (in Python) Course

SWD3: Research Software Development documentation and course notes.

[![DOI](https://zenodo.org/badge/1070653879.svg)](https://doi.org/10.5281/zenodo.20180993)

## How to deliver

The course is fully self-contained at [https://arctraining.github.io/git/](https://arctraining.github.io/git/) with no additional required delivery notebooks/answers. No installations are required. Familiarity with GitHub codespaces is required to deliver (running through the rpactical sessions beforehand will provide enough knowledge to deliver; ensure you rehearse this before delivering live).

The course material consists of:

- Presentations (which are also available printed out all-on-one-screen for learners to review between sessions/after the course)
- Practical sessions, which are designed to primarily be done independently by the students: they contain detailed instructions and screenshots, allowing the learners to work independently for a set time, and then regroup to run through the example/ask questions etc.

The entire course is searchable via the top bar.

## Contributing

You can add markdown and the page will automatically build when pushed to GitHub.

## Building instructions

*Note that this repository is also configured to build via a GitHub action. HTML pages are not tracked via version control*.

You can use pip to install the package `heading_converter` to run the scripts in this project. These scripts pull in the content from presentations and format them as an article. The environment with this package must be active before using Quarto to render the material.

You can install the locally stored version in this repo with the Conda 
`environment.yml`: 

```bash
cd heading_converter
conda env create -f environment.yml
conda activate heading-conv-env
quarto preview
```

Install the most recent development version (may not be stable):

```bash
pip install <PACKAGE_NAME>@git+https://github.com/<USER_NAME>/<REPO_NAME>
```

Or install a specific version (version 0.1.0 in this example; please check the releases page):

```bash
pip install https://github.com/<USER_NAME>/<REPO_NAME>/archive/refs/tags/v0.1.0.tar.gz

# or

pip install <PACKAGE_NAME>@git+https://github.com/m<USER_NAME>/<REPO_NAME>@v0.1.0
```

## Author

Below is a list of contributors (in chronological order of addition) with associated Contributor Role Taxonomy (CRediT) roles. Please see the [CRediT website](https://credit.niso.org/) for definitions of roles.

- [Maeve Murphy Quinlan](https://orcid.org/0000-0003-2958-1008): conceptualization, writing (original draft), writing (review and editing), data curation, methodology.
  - Creation of website, Python workflows, GitHub actions.
  - Redesign of course.
- [Sorrel Harriet](https://orcid.org/0000-0003-0143-6554): writing (original draft), writing (review and editing), vizualisation (addition and creation of graphics), supervision.

## Citation instructions

Please use the suggested citation in the sidebar (under "Cite this repository"), or view the CITATION.cff file.

## License

This material is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License](https://creativecommons.org/licenses/by-nc-sa/4.0/), and is copyrighted by the University of Leeds.
