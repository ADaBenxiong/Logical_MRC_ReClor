# Logic-Driven Machine Reading Comprehension with Graph Convolutional Networks

Our logical reasoning machine reading comprehension code repository.

We utilize RoBerta as our backbone model, and we use inductive learning graph neural network. We propose a new model **EIGN**, an entity inference graph network.

We verify our result on ReClor dataset and LogiQA dataset.


Our code reference:
[https://github.com/yuweihao/reclor](https://github.com/yuweihao/reclor%EF%BC%8C)  
[https://github.com/Eleanor-H/DAGN](https://github.com/Eleanor-H/DAGN)
##   directory structure
- reclor data
	- train.json
	- val.json
	- test.json
- roberta-large
	- config.json
	- vocab.json
	- pytorch_model.bin

## How to run
	
	1. install dependencies
	pip install -r requirements.txt
	
	2. train model
	bash run_roberta_large.sh

- --use_gcn represents the method of using GCN
- --use_pool represents the method of using Pooling
- --fo_fgm represents the method of using adversarial training


## Results

Our experimental results on the **ReClor** dataset
|       Model         |Dev|Test|
|----------------|-------------------------------|-----------------------------|
|RoBerta|62.80            |55.60           |
|EIGN|65.60            |60.00           |
|EIGN+FGM|67.00|61.00|

The leaderboard of ReClor dataset is : [Leaderboard - EvalAI](https://eval.ai/web/challenges/challenge-page/503/leaderboard)
  

We have experimented many times and the best test has been achieved 61.70%


Our experimental results on the **LoigQA** dataset
|       Model         |Dev|Test|
|----------------|-------------------------------|-----------------------------|
|RoBerta|35.02|35.33|
|EIGN|37.48|38.56|
|EIGN+FGM|38.86|38.86|

We use 1 RTX 2080Ti GPU for all experiments.   

The experimental results will be slightly different in different experimental environments

## Future

We open source our code, anyone interested could have a try.

If our work is helpful to you, hope you can click a star to show encouragement.

Our repository will continue to be updated to get better results on more datasets. And we will continue to  research the task of logical reasoning.
