## Chinese Intent Classify 2018-9

#### 1.preprocess

prepare() 将按类文件保存的数据汇总、清洗、去重，augment() 进行数据增强

#### 2.explore

统计词汇、长度、类别的频率，条形图可视化，计算 sent / word_per_sent 指标

#### 3.featurize

ml 特征化，bow() 构建词袋模型，svd() 变换到语义隐空间，降维、平滑

#### 4.vectorize

nn 向量化，embed() 建立词索引到词向量的映射，align() 将序列填充为相同长度

#### 5.build

ml_fit() 通过 svm、xgb，nn_fit() 通过 dnn、cnn、rnn 构建分类模型

#### 6.classify

predict() 实时交互，输入单句、清洗后进行预测，输出所有类别的概率
