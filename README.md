# 自动驾驶目标检测模型（YOLOv11）


基于YOLOv11的自动驾驶场景目标检测模型，针对交通参与者（行人、车辆等）进行优化，支持在公开/自定义数据集上的训练与推理。


## 1. 运行环境配置


### 1.1 Conda 环境配置（推荐）
```
#创建虚拟环境
conda create -n yolov11 python=3.10 -y
conda activate yolov11


#安装依赖（包含PyTorch、CUDA支持）
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu130
pip install ultralytics  # YOLOv11核心库
pip install opencv-python pandas tqdm  # 辅助工具库


```
## 2. 代码训练以及模型测试示例命令


### 2.1 代码训练示例命令
```
#跳转到工作目录
cd path/to/hw2/code
#运行训练程序
python train.py
```
### 2.2 模型测试命令
```
#跳转到工作目录
cd path/to/hw2/code
```

打开evaluate.py 修改第32行model_path的值为所训模型所在位置

```
#运行训练程序
python evaluate.py
```


## 3. 自动驾驶数据集验证集上的准确率
在 SODA10M 数据集测试集 上的评估结果（目标类别：行人、骑行者、小汽车、卡车、电车、三轮车）：  
Precision(精确率):0.7556  
模型文件：
