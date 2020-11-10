
---

<div align="center">    
 
# Seatizen

[![Paper](http://img.shields.io/badge/paper-arxiv.1001.2234-B31B1B.svg)](https://www.nature.com/articles/nature14539)
[![Conference](http://img.shields.io/badge/NeurIPS-2019-4b44ce.svg)](https://papers.nips.cc/book/advances-in-neural-information-processing-systems-31-2018)
[![Conference](http://img.shields.io/badge/ICLR-2019-4b44ce.svg)](https://papers.nips.cc/book/advances-in-neural-information-processing-systems-31-2018)
[![Conference](http://img.shields.io/badge/AnyConference-year-4b44ce.svg)](https://papers.nips.cc/book/advances-in-neural-information-processing-systems-31-2018)  
<!--
ARXIV   
[![Paper](http://img.shields.io/badge/arxiv-math.co:1480.1111-B31B1B.svg)](https://www.nature.com/articles/nature14539)
-->
![CI testing](https://github.com/PyTorchLightning/deep-learning-project-template/workflows/CI%20testing/badge.svg?branch=master&event=push)


<!--  
Conference   
-->   
</div>
 
## Description   
Surfers, kitesurfers, windsurfers, divers, sailors will be able to contribute to the acquisition of
marine data. This new network will make it possible to better map marine biodiversity and to
Strengthen the collection of large-scale environmental data on the coastal ecosystems of the
French coastline. The data collected by this network of participatory sciences will enable the
researchers to answer key scientific questions about the impact of change
on marine ecosystems, while involving civil society in this innovative approach.
Open Citizen Science (open data, open source, open hardware and open model). In return, this network
strengthen the information and services expected by users of the marine domain (more data, more information, more information, more services).
available on marine weather, information on sea trips or data enhancement
available for sea rescue).

For more informations about the project see https://drive.google.com/file/d/1UoRMP1YMiqU4Ru9geqHE0cvURKAQnlJx/view
## How to run   
First, install dependencies   
```bash
# clone project   
git clone https://github.com/YourGithubName/deep-learning-project-template

# install project   
cd deep-learning-project-template 
pip install -e .   
pip install -r requirements.txt
 ```   
 Next, navigate to any file and run it.   
 ```bash
# module folder
cd project

# run module (example: mnist as your main contribution)   
python lit_classifier_main.py    
```

## Imports
This project is setup as a package which means you can now easily import any file into any other file like so:
```python
from project.datasets.mnist import mnist
from project.lit_classifier_main import LitClassifier
from pytorch_lightning import Trainer

# model
model = LitClassifier()

# data
train, val, test = mnist()

# train
trainer = Trainer()
trainer.fit(model, train, val)

# test using the best model!
trainer.test(test_dataloaders=test)
```

### Code and folders structure
* ***proj_seatizen*** contains:
  * ***main.jpynb*** calls the main functions:
    * **fine_tuning_config_file** : configuration file;
  * ***input_dataset*** folder contains the original dataframe;
  * ***output_dataset*** folder contains the train and the validation dataframes;
    * ***train*** folder contains the train dataframe;
    * ***val*** folder contains the train dataframe;
  * ***references*** folder contains main bibliography exploited in our work;
