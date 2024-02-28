1 下载数据到input文件夹

https://www.kaggle.com/datasets/columbia2131/otto-chunk-data-inparquet-format

https://www.kaggle.com/datasets/cdeotte/otto-validation

https://www.kaggle.com/competitions/otto-recommender-system/data

https://www.kaggle.com/datasets/radek1/otto-full-optimized-memory-footprint

2 运行word2vec训练模型word2vec-train.ipynb；建议用kaggle的GPU训练

3 依次运行模型验证代码

运行召回程序 code/recall_valid.ipynb；建议用kaggle的GPU训练

运行特征程序 code/feature_prepare_valid.ipynb

运行排序模型 code/rank_model_valid.ipynb

分三种类型去运行代码，可以修改参数t=clicks/carts/orders

可以修改召回的数量，默认是50，可以修改到250，召回越多分数越好

4 依次运行模型预测代码

运行召回程序 code/recall_test.ipynb；建议用kaggle的GPU训练

运行特征程序 code/feature_prepare_test.ipynb

运行排序模型 code/rank_model_test.ipynb，得到提交文件submission.csv


关键代码包

pandas

numpy

lightgbm

cudf

gensim

建议内存128G，代码需要运行48小时



