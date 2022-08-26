# Sentence Tranformers with Tensorflow

[Sentence Transformers](https://www.sbert.net/) is the state-of-the-art library for sentence, text, and image embeddings to build semantic textual similarity, semantic search, or paraphrase mining applications using BERT and Transformers 🔎 1️⃣ ⭐️

The library is built on top of PyTorch and Hugging Face Transforemrs so it is compatible with PyTorch models and not with TensorFlow. But since Hugging Face Transformers is compatible with PyTorch and TensorFlow it is possible to load the raw Sentence Transformer models in Tensorflow. 

This repository contains code, examples and introductions on how to use Sentence Transformers in Tensorflow.

* [training _coming soon_](./training)
* [inference](./inference)


## Getting started 

All included examples expect a setup Python environment, e.g. with conda. 

```bash
# Get Miniconda and make it the main Python interpreter
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p ~/miniconda 
rm ~/miniconda.sh
export PATH=~/miniconda/bin:$PATH
```

### GPU: CUDA112 setup 

create GPU env

```bash
conda create --channel=conda-forge --name tf \
  python=3.9 \
  nvidia::cudatoolkit=11.2 \
  tensorflow=2.9.1=*cuda112*py39* 
```

### CPU setup 

create CPU env

```bash
conda create --channel=conda-forge --name tf \
  python=3.9 \
  tensorflow=2.9.1=*cpu*py39*
```


  - transformers[sklearn,sentencepiece,audio,vision]==4.21.1
  - tensorflow-text