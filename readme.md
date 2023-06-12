## 项目结构
Updating: 2023-06-12<br>

url:[点击此处（click here）](https://github.com/sellenzh/pedCMT)<br>
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
├── PIE                         <- 数据集（此处下载:[PIE](https://github.com/aras62/PIE.git))
│   ├── ...                     <- note: 需要解压文件`annotations.zip`,`annotations_vehicle.zip`,
│   │   ├── ...                 <- `annotations_attributes.zip`
│   │   └── ....                <- 此处下载:[PIE](https://github.com/aras62/PIE.git)
│   └── ...  
│       ├── ...                 <- 另一个数据集[JAAD](https://github.com/ykotseruba/JAAD.git)
│       └── ...                 <- ...
│
├── utils                       <- 保存工具文件。
│   ├── pie_data.py             <- 数据集加载器。
│   └── pie_preprocessing.py    <- 训练过程处理文件。
│
├── model                       <- 保存模型文件。
│   ├── BottleNeck.py           <- 瓶颈结构。
│   ├── FFN.py                  <- 前馈神经网络。
│   ├── model_blocks.py         <- 一些使用或未使用的模型块。
│   └── main_model.py           <- 主模型。
│
├── pie.py                      <- 训练文件。 
│                                 └ 
└── README.md
```
此处下载:[PIE](https://github.com/aras62/PIE.git)<br>
另一个数据集[JAAD](https://github.com/ykotseruba/JAAD.git)