# **NER 命名实体识别  LSTM CNN CRF**
NER 命名实体识别，Pytorch，LSTM、BiLSTM、CNN，可添加条件随机场CRF  

[** Blog 详细内容 **](https://ppphhhleo.github.io/2021/11/01/nlp1/)

## **Quick Start**

### 0 实验环境  
> python3 + jieba + pytorch1.0.0 + numpy  
  pip install -r requirement.txt  

python-crfsuite==0.9.6
six==1.12.0
sklearn-crfsuite==0.3.6
tabulate==0.8.3

### 1 配置模型相关超参数及预训练词向量路径：

    /models/config.py

**ckpts 文件夹** ，存放训练好的模型


### 2 模型训练及测试：


```gas
python main.py --model [模型] --crf --use_w2v
```  

其中，可根据实际需求调整

**--model [模型]：cnn / lstm / bilstm**

**--crf ：增加crf层**

**--use_w2v ：使用预训练词向量**

### 3 数据记录

    **Loss图，测试结果，均保存在：**

    **record.ipynb** 可视化结果


---- 
## **相关论文**

1.  [**Bidirectional LSTM-CRF models for sequence tagging**](https://arxiv.org/pdf/1508.01991.pdf)

2.  [**A survey on deep learning for named entity recognition**](https://ieeexplore.ieee.org/abstract/document/9039685/)


