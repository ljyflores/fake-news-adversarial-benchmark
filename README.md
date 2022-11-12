# fake-news-explainability
<b>TLDR:</b> We demonstrate that fake news classification models are brittle: they can achieve great performance on fake news classification benchmarks, while also failing on adversarial examples. 

We create adversarial examples by negating the original sentences and swapping names of politicians in the statements. In theory, an accurate model would flip its predictions (see paper for explanation), but we find that "SOTA" models don't. We find that these models don't necessarily learn facts or how to distinguish <i>real</i> vs <i>fake</i>, but rather learn to associate certain keywords with certain probabilities, which are biased based by how many pieces of real or fake news are in the dataset that pertain to that keyword.

This repository only contains the notebooks used to train the models and evaluate them.
Check out the <a href="https://drive.google.com/drive/folders/10zdrFakmNSOeOmQufYwQvTiESwP8pNyz?usp=sharing">data</a> and <a href="https://drive.google.com/drive/folders/1XFoYNmYP-DD3Bj7zg9AXzDT7VmGtf0aG?usp=sharing">models</a>!

Feel free to check out our paper <a href=https://arxiv.org/abs/2201.00912>here</a>, which we presented at <a href=https://advml-workshop.github.io/aaai2022/> Workshop on Adversarial Machine Learning and Beyond at AAAI 2022 </a>! 

If you find our work useful, please consider citing our paper!
```
@inproceedings{
flores2022an,
title={An Adversarial Benchmark for Fake News Detection Models},
author={Lorenzo Jaime Yu Flores and Yiding Hao},
booktitle={The AAAI-22 Workshop on Adversarial Machine Learning and Beyond},
year={2022},
url={https://openreview.net/forum?id=n3PMOhS42s6}
}
```
