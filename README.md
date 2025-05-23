# LoRA-Qwen-MedQA
Fine-tuning the QWen model for Chinese question answering.
本项目基于LoRA方法微调开源大语言模型QWen-1.8B,使其更适用于中文问答场景。

## 项目简介
- 使用 HuggingFace Transformers + PEFT(LoRA)进行低资源微调
- 数据集为CMRC2018
- 模型部署支持Gradio网页问答接口

## 使用方法
### 1.安装依赖
```bash
pip install -r requirements.txt
### 2.启动训练（LoRA微调）
bash
python train.py
### 3.启动问答系统（Gradio页面）
bash
python app.py

## 项目结构
LoRA-Qwen-MedQA/
├── README.md             # 项目说明文档
├── train.py              # LoRA 训练脚本
├── evaluate.py           # 模型评估
├── app.py                # 网页问答界面
├── requirements.txt      # 依赖包列表
├── data/
│   └── train.json        # 中文问答数据
├── checkpoints/          # 模型保存路径
└── results/
    └── loss_curve.png    # 训练过程图

## 实验结果


## 联系方式
作者：闫晓莹
邮箱：2765532139@qq.com
  
