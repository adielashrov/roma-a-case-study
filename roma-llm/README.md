
# RoMA - LLM

The following instructions are for installing and executing the roma-llm case study on a linux/ubuntu machine with a GPU properly configured.

### Setting up the environment
1. Start by making sure that you have the following packages installed:

`sudo apt-get install python3.9-dev`

`sudo  apt-get  install libasound2-dev`

2. Create a virtual environment using conda:

`conda create -n roma-llm python=3.10`

3. Activate the environment:

`conda activate roma-llm`

5. Install the requirements file

`pip install -r requirements.txt`

### Executing the experiment

Pre-requisite - you should download the GLUE dataset to a folder named data.

#### Creating the dataset

`python create_full_sentence_dataset.py`

#### Running prediction on the dataset

`python predict_sentence_dataset_full.py`

#### Running RoMA analysis on the predictions

`python analysis_full_prediction.py`

Good Luck!