# Logical_MRC_ReClor

个人学习仓库，整理逻辑推理机器阅读理解的代码库。

使用RoBerta预训练模型， 使用ReClor数据集， 使用inductive learning 图神经网络

代码参考https://github.com/yuweihao/reclor， https://github.com/Eleanor-H/DAGN

在目录下需要创建保存数据集以及保存模型的文件夹

目录结构如下：

  --reclor_data
    --train.json
    --val.json
      
    --test.json
      
  --roberta-large
  
    --config.json
      
    --vocab.json
      
    --pytorch_model.bin
      
