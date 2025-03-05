# 测鱼宝（CeFish）使用指南

## 项目简介
测鱼宝是基于HRNet深度学习模型开发的鱼类形态表型高通量分析工具，可自动化获取体长、体高、胸鳍、尾鳍等10个关键形态特征[1](@ref)。该软件支持实时拍摄与批量导入模式，适用于大黄鱼、鲈鱼、鲤鱼等多种养殖鱼类，助力遗传育种研究与生产优化。

[![GitHub Repository](https://img.shields.io/badge/GitHub-miaomiaoge/CeFish-blue)](https://github.com/miaomiaoge/CeFish)

## 安装指南

### 1. CP2102 USB-UART驱动安装
#### 设备管理器检查
- 连接设备后，右键「此电脑」→「管理」→「设备管理器」
- 检查端口（COM和LPT）是否存在黄色警示标志  
  ![驱动状态检查](https://github.com/user-attachments/assets/bdf34115-5977-4393-b110-05db46d79531)

#### 官方驱动安装
1. 下载Silicon Labs官方驱动：[CP210x_VCP_Windows.zip](https://github.com/user-attachments/assets/2350fd66-5f4f-4288-bb49-649bdf96120d)
2. 解压后运行`CP210xVCPInstaller_x64.exe`
3. 按向导完成安装，重启计算机

#### 验证安装
设备管理器应显示正常通信端口：  
![验证成功示例](https://github.com/user-attachments/assets/b0c8e3ad-ace1-41ce-b8b8-9bf465b42fa6)

### 2. 系统授权
1. 启动软件后进入授权申请界面：  
   ![授权申请](https://github.com/user-attachments/assets/34076251-4dc0-4a8d-a166-f6cc88576)
2. 输入激活码后进入验证状态：  
   ![激活界面](https://github.com/user-attachments/assets/c03ece07-c2bd-40ac-ad87-6c0e07dd4cff)

## 操作流程

### 图像采集模块
#### 实时拍摄模式
1. 调整摄像头至鱼体正上方
2. 点击「实时拍摄」按钮  
   ![实时拍摄界面](https://github.com/user-attachments/assets/6dbd2f7b-16d7-405f-9981-4b644f5f64d9)
3. 自动生成形态特征热图与数据报表

#### 批量导入模式
1. 准备标准化拍摄的JPG/PNG图像
2. 拖拽文件夹至导入区域：  
   ![批量导入界面](https://github.com/user-attachments/assets/c103f0d0-ea6b-4e79-8364-9e976ab3baa4)
3. 支持同时处理≤500张图像（建议分辨率1920×1080）

## 技术文档
- 形态特征检测原理说明
- API接口开发指南
- 数据标准化采集规范  
  [查看完整文档](https://github.com/miaomiaoge/CeFish/wiki)

## 引用文献
[1](@ref): Zeng J, Feng M, et al. Deep learning to obtain high-throughput morphological phenotypes and its genetic correlation with swimming performance in juvenile large yellow croaker. Aquaculture. 2023. https://doi.org/10.1016/j.aquaculture.2023.740051
