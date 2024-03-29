# Boolean dynamic modeling of of MAP Kinase pathway
<p align="justify"> The most relevant model of MAP Kinase pathway was released almost a decade ago (Grieco et al., 2013, PLoS Comp. Bio.). Since then, a lot of new discoveries about cross talk between growth arrest, cell proliferation, and apoptosis have remained unconsolidated. For instance, the pivotal role of JNK cascades (through TNFR1, TNFR2 and TGFBR) was unknown when the previous model was developed. In our work, we have developed a Boolean dynamic network model for cellular decision-making by integrating all the information available till-date about growth arrest, proliferation, and apoptosis. In silico node perturbations were carried out and compared with relevant experimental observations to ensure accuracy of the model. The results of model simulations were in agreement with the gene knockout and constitutive expression studies reported in literature, underscoring the high precision of the deduced comprehensive network. The fidelity of our model makes it useful to understand the etiology of malignancy in mammalian cells. Furthermore, DUSP1 knockout under ‘Insulin and DNA damage’ signaling was found to universally enhance the proportion of cells undergoing apoptosis. We also focused on Bladder cancer models and discovered that in PI3K-gain-of-function Bladder Cancer model, under constitutive activity of MYC slight reduction in proliferation rate was observed suggesting that MYC can exert a self-control role when it is constitutively active. These observations will be useful in designing future experimental work in developing novel therapeutic interventions. </p>

## Requirements
1. Python 2
2. BooleanNet Library
3. Matplotlib Library

## How to use:
The baseline.py accepts only one command line arguement: --end_state, it has to be one of Proliferation, Apoptosis, or Growth_Arrest.

### Example:
python baseline.py --end_state Apoptosis


The simulations.py and simulations_Bladder_Cancer.py scripts accept two command line arguements: 1.) --end_state and 2.) --type. The second arguement refers to the type of perutbations to be considered, whether constitutive activity (CA) or knockout (KO).

### Example:
python simulations.py --end_state Apoptosis --type KO
