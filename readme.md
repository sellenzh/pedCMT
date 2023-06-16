## 项目结构
Updating: 2023-06-16<br>

项目地址:[点击此处（click here）](https://github.com/sellenzh/pedCMT)<br>
项目结构如下所示：

```
├── checkpoints                 <- 保存训练模型文件。
│   ├── JAAD_all.pt             <- 这里依据的数据集名称命名。
│   ├── JAAD_beh.pt
│   └── PIE.pt
│
├── logs                        <- 保存训练日志文件。
│   └── PIE                     <- 这里依据的数据集名称命名。
│       └── ...                 <- ...
│
├── PIE                         <- 数据集（下载:[PIE]）
│   ├── ...                     <- note: 需要解压文件`annotations.zip`,`annotations_vehicle.zip`,
│   │   ├── ...                 <- `annotations_attributes.zip`
│   │   └── ....                <- 
│   └── ...  
│       ├── ...                 <- 另一个数据集[JAAD]
│       └── ...                 <- ...
│
├── utils                       <- 保存工具文件。
│   ├── pie_data.py             <- 数据集加载器。
│   └── pie_preprocessing.py    <- 训练过程处理文件。
│
├── model                       <- 保存模型文件。
│   ├── BottleNeck.py           <- 瓶颈结构。
│   ├── FFN.py                  <- 前馈神经网络。
│   ├── model_blocks.py         <- 一些使用的小型模型块。
│   └── main_model.py           <- 主模型。
│
├── pie.py                      <- 训练文件。 
│                                 └ 
├── jaad.py                     <- 训练文件。 （未标记注释。）
│                                 └ 在JAAD数据集上的训练文件。
└── README.md
```
此处下载:[PIE](https://github.com/aras62/PIE.git)<br>
另一个数据集[JAAD](https://github.com/ykotseruba/JAAD.git)
