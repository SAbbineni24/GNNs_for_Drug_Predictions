# CPSC 483 Final Project
Final Project for CPSC 483: Deep-Learning on Graph Structured Data

In this project, I implement the GCNMLP architecture to predict links between drugs and side effects and the NEDD architecture to predict links between drugs and diseases.

## Setup
Clone this GitHub repository containing the code for the GCNMLP architecture and NEDD architecture, as well as the datasets.

```bash
git clone https://github.com/SAbbineni24/cpsc483finalproject.git
```

## Install Packages
Install the packages listed in the `requirements.txt` file.
```bash
pip install -r requirements.txt
```

## Run the Project

### Running GCNMLP
To run the GCNMLP model, navigate to the ``DSE-Prediction`` folder and run all of the cells in the ``GCNMLP_for_DSE.ipynb`` notebook.

### Running NEDD
To run the NEDD model, navigate to the ``DD-Prediction`` folder and run all of the cells in the ``NEDD_for_DD.ipynb`` notebook. The results will be replicated using the pretrained vec file ``nodeVec_pretrained.txt``.

#### Any Issues with ```hin2vec.c``` (NOT NECESSARY if trying to replicate results)
If you would like to reuse the NEDD procedure in the notebook or generate new embeddings, you must compile the ``hin2vec.c`` file for your machine, as the source binary for ```hin2vec``` in this repository is made for Linux. To do this, simply cd to the src folder using 
```bash
cd ./DD-Prediction/hin2vec/model_c/src
```
and follow this command with
```bash
make
```
Again, this is NOT NECESSARY if you would like to just replicate the results. This is only needed if you would like to generate new embeddings and you are not on a Linux machine.
