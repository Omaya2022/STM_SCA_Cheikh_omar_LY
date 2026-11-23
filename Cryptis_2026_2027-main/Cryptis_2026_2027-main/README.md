<img src='images/logo_cryptis.png' style='width: 1200px; float:center'>


# Sécurité et implémentations sur cartes à puce
### ANNEE 2026-2027

-----------
# TPs XLIM Master Cryptis M2
-------------------


## Development Environment to Set

We will use Jupyter Lab with some open sources libraries. 
Feel free to use other environments like Visual Studio Code.

## How to Install the Tools Required for the Labs?

You have three options:

- **Use the conda or pip environment below**  
- **Using Docker**
- **Manual installation on your own**


-----------------------------------
## Create a conda environment


It is recommended you create a conda environment with:

````
$ conda create -n my_sca_env python=3.12
then
$ conda activate my_sca_env
ou $ source activate my_sca_env
then

be sure the .condarc file of your environment contain the right default channels path to access packages.

then

- $ conda install --file requirements.txt

````

Install jupyterlab using:

````
conda install jupyterlab 

or

pip install jupyterlab

````


#### Environment Uninstall if needed

check the environment name

````
conda env list
````

Remove the conda environment
````
conda deactivate

conda remove --name my_sca_env --all
````
check the conda env is indeed removed

````
conda env list
````


----------------------------
## Installation with Docker

The **dockerfile** and **docker-compose.yml** are in [this directory](./docker/)

Follow the procedure in the following PDF [installation with docker](./docker/docker_install.pdf)

--------------------------
## Manual Installation

1. Using pip requirements install the packages listed in requirements.txt file
 

2.  pip install jupyterlab (ou conda install jupyterlab)


3.  Installation of ChipWhisperer-Lite 32-bit
We will use this NewAE board to collect side-channel traces for the trainings.

    Install chipWhisperer by following the instruction given there

    https://chipwhisperer.readthedocs.io/en/latest/linux-install.html#quick-installation


    #### Please also install the following library with
    ````
    $ > pip install chipwhisperer
    ````
------------------

* Date last change: november 2026.