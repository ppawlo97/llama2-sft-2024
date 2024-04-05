# LLaMa2 Weather Conditions Generation

## Table of Contents

* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)



## Getting Started

Follow these steps to get a local copy up and running.



### Prerequisites

1. Optionally, if you want to rerun `notebooks/01_Dataset_Generation.ipynb`, obtaining Anthropic API token is necessary. The token is not free and can be generated [here](https://www.anthropic.com/api).
2. If you don't want to use Google Colab environment, make sure that you have access to a GPU with at least 16GB of RAM, since without it the code will execute very long.
3. If you don't want to use Google Colab environment, make sure that you have [Anaconda](https://www.anaconda.com/) installed.



### Installation

#### Google Colab (recommended)

1. Copy all contents of the repository to the Google Colab workspace.
2. Open either of the notebooks, e.g. `notebooks/02_LLaMa_SFT.ipynb` and follow the instructions there. You should find a `pip install` cell at the beginning of each notebook.


#### Local Environment

1. Create separate virtual environment for the project.
```sh
conda create --name=llama-sft python=3.10 -y
```
2. Switch to the created environment.
```sh
conda activate llama-sft
```
3. Install the dependencies.
```sh
pip install -r requirements.txt
```
4. Install Jupyter Notebook.
```sh
pip install notebook
```



## Usage

#### Local Environment
Not recommended, since I've run on Google Colab.

1. Remember to always switch to the right virtual environment.
```sh
conda activate llama-sft
```
2. Optionally, if you plan to run Dataset Generation, export Anthropic token as an environmental variable
```sh
export ANTHROPIC_API_KEY=<token>
```
3. Start Jupyter Notebook server or preview notebooks in IDE plugins (e.g. VSCode)
```sh
jupyter notebook
```
