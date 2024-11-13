## 概述
这是 MASTER 基准测试的一个替代版本。

论文: [MASTER: Market-Guided Stock Transformer for Stock Price Forecasting](https://arxiv.org/abs/2312.15235)

代码: [https://github.com/SJTU-Quant/MASTER](https://github.com/SJTU-Quant/MASTER)

## 配置
我们建议您使用 conda 来配置环境并运行代码：
> 请注意，您需要自行安装 `torch`。
```
bash config.sh
```

## 运行
您可以直接使用 bash 脚本来运行代码（您可以在 `run.sh` 中设置 `universe` 和 `only_backtest` 标志），这个 `main.py` 将使用 3 个随机种子来测试模型：
```
conda activate MASTER
bash run.sh
```
<!-- 或者您也可以直接使用 `qrun` 来运行代码（请注意，您需要修改您的 `qlib`，因为我们在 `qlib/contrib/data/dataset.py`、`qlib/data/dataset/__init__.py`、`qlib/data/dataset/processor.py` 和 `qlib/contrib/model/pytorch_master.py` 中添加或修改了一些文件）：
```
qrun workflow_config_master_Alpha158.yaml
``` -->