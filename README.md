# Robust Data-centric Graph Structure Learning for Text Classification (DCGSL)

### Author: Jun Zhuang.

### Paper:
> Companion Proceedings of the ACM Web Conference 2024 (WWW '24 Companion)

### Abstract:
> <p align="justify">
Over the past decades, text classification underwent remarkable evolution across diverse domains. Despite these advancements, most existing model-centric methods in text classification cannot generalize well on class-imbalanced datasets that contain high-similarity textual information. Instead of developing new model architectures, data-centric approaches enhance the performance by manipulating the data structure. In this study, we aim to investigate robust data-centric approaches that can help text classification in our collected dataset, the metadata of survey papers about Large Language Models (LLMs). In the experiments, we explore four paradigms and observe that leveraging arXiv's co-category information on graphs can help robustly classify the text data over the other three paradigms, conventional machine-learning algorithms, pre-trained language models' fine-tuning, and zero-shot / few-shot classifications using LLMs.
</p>

### Dataset:
> We first collected the metadata of 112 literature reviews about Large Language Models (LLMs).

### Getting Started:
#### Prerequisites
> Linux or macOS \
> CPU or NVIDIA GPU + CUDA CuDNN \
> Python 3.11 \
> pytorch, dgl, transformers, numpy, scipy, sklearn, yaml

#### Clone this repo
> ```git clone https://github.com/junzhuang-code/DCGSL.git``` \
> ```cd DCGSL```

#### Install dependencies
> For pip users, please type the command: ```pip install -r requirements.txt``` \
> For Conda users, you may create a new Conda environment using: ```conda env create -f environment.yml```

#### Directories
> **data**: contain graph data, survey data, and text corpus; \
> **data_collection**: contain scripts for scraping data and processing text corpus; \
> **baselines**: source code of GNNs and LMs; \
> **config**: the config files.

#### Processing Steps
> **Data Collection**: Collect raw data from arXiv. \
> **Data Construction**: Generate co-graphs and text graphs. \
> **Data Evaluation**: Validate the dataset via GNNs and LMs.
