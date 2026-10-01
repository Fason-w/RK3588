# RK3588_Project

## 初步了解

### PC配置

- 不能用WINDOWS系统，采用虚拟机**VMware**+**Ubuntu**
- 下载**Anaconda**（python环境需要，比如PyTorch）
- 去github官网上下载**RKNN-Toolkit2**

### 基本逻辑

1. 定昌SDK写好需要的AI代码并转换成**.nnx形式**（例：yolov5s_relu.onnx）

2. 接下来在**Anaconda的rknn环境**里，用**RKNN-Toolkit**把现成的**.nnx**模型转换成**.rknn**格式（板子只认rknn格式的内容）
3. 把**.rknn**格式的推理代码传到板子上，RK3588调用NPU运行