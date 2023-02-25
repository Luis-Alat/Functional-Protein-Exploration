# Functional-Protein-Exploration

Repository containing the files used to process and generate the file to visualize the transcriptional regulatory networks of six organisms on Tableau. The final visualization can be consulted on my respective Tableau [profile](https://public.tableau.com/app/profile/luisr3415)

On the other hand, the genomes fasta files and tsv networks used here can be downloaded/obtained according to [Homology-based reconstruction of regulatory networks for bacterial and archaeal genomes](https://www.frontiersin.org/articles/10.3389/fmicb.2022.923105/full) or directly from the genomes and networks folders in this repository.

---

## Getting started

<br/>

### Requeriments

Here, the technologies/tools used are the following:

* [Python](https://www.python.org/): Programming lenguage

* [Jupyter-Notebooks](https://jupyter.org/): Web-based interactive computing platform

* Bash/Linux: Unix Shell

* [CytoScape](https://cytoscape.org/): Software for visualizing and analysis of complex networks

* [Interproscan](https://interproscan-docs.readthedocs.io/en/latest/): Database integrating predictive information about proteins’ function from a number of partner resources,

**_Note that you will have to download CytoScape manually along with the *yFiles* extention. In addition, you will need interproscan too_**

### Environment

In order to run the notebooks presented here locally, a conda environment yml file is provided; therefore, you will need to download [conda](https://www.anaconda.com/) or [mamba](https://mamba.readthedocs.io/en/latest/index.html).

By default, this environment is named **analyzeNets**, if you want another name for it. You will have to change the value of the **name:** line at the beginning of the file to the name you want.

Once you have downloaded conda or mamba and optionally renamed the environment. You can run one of the following commands to install the yml file

    conda env create -f environment.yml

<br/>

    mamba env create -f environment.yml

and one of the following to activate the environment

    conda activate <name-of-your-environment>

<br/>

    mamba activate <name-of-your-environment>

---

## Contents

<br/>

* CoordinatesNetworks/: Coordinates *x* and *y* from yFiles in CytoScape

* Data/: Data to load into Tableau

* genomes/: Genomes used in fasta file format

* InterproFullMerge/: TSV files joined with XML files from interproscan

* InterproParsedXML/: Processed XML files into TSV format from interproscan

* InterproResults/: Output from interproscan

* networks/: Transcriptional regulatory networks in tsv format

