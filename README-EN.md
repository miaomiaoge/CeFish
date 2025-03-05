<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/29e05213-f44f-4e2d-9e51-7cca4024a54a" alt="CeFish Logo">
</p>

<h1 align="center">CeFish 测鱼宝 - 智能鱼类表型分析系统</h1>

<div align="center">
  <img src="https://img.shields.io/badge/Version-2.1.0-brightgreen" alt="版本">
  <img src="https://img.shields.io/github/downloads/miaomiaoge/CeFish/total" alt="下载量">
  <img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue" alt="许可协议">
</div>

## 🚀 核心优势
| 功能维度 | 技术突破 |
|---------|----------|
| ​**智能检测**​ | 基于HRNet深度学习模型[1](@ref)，单张图片即可获取14+表型特征 |
| ​**多物种支持**​ | 覆盖大黄鱼、加州鲈、鲤鱼等9大养殖鱼种 |
| ​**测量精度**​ | 关键点检测准确率≥96%[1](@ref)，支持动态比例校准 |
| ​**操作便捷性**​ | 全流程自动化处理，兼容复杂背景图像 |

## 🔍 检测标准体系
### 大黄鱼关键检测点示意图
<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/e65d7965-0400-4525-8b31-435e6606b8fa" alt="检测标准" width="70%">
  <br><em>涵盖体长、体高、胸鳍等10个形态学关键点[1](@ref)</em>
</p>

## 📸 拍摄规范
<div align="center">
  <div style="display: flex; justify-content: space-around;">
    <div>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="90%">
      <p><strong>模式A（三要素）</strong><br>鱼体+电子秤+5cm黑色标尺</p>
    </div>
    <div>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="90%">
      <p><strong>模式B（双要素）</strong><br>鱼体+5cm黑色标尺</p>
    </div>
  </div>
</div>

## ⚙️ 安装与配置
### 1. 源码获取
```bash
git clone https://github.com/miaomiaoge/CeFish.git
