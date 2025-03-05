<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/29e05213-f44f-4e2d-9e51-7cca4024a54a" alt="CeFish Logo">
</p>

<h1 align="center"> 测鱼宝 - 智能鱼类表型采集系统</h1>

<div align="center">
  <img src="https://img.shields.io/badge/Version-2.1.0-brightgreen" alt="版本">
  <img src="https://img.shields.io/github/downloads/miaomiaoge/CeFish/total" alt="下载量">
  <img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue" alt="许可协议">
</div>


# 测鱼宝使用指南
---
## 📥 软件获取
**最新版本**​  
`v2.0.1` 发布于2023年11月  
[![DOI](https://img.shields.io/badge/DOI-10.6084/m9.figshare.24278065.v2-blue)](https://doi.org/10.6084/m9.figshare.24278065.v2)  

⚠️ 访问提示：  
- 遇到403错误建议使用校园VPN访问
- 或发送请求至技术支持邮箱：2992861134@qq.com

---
## 🏆 核心优势
<table>
  <tr>
    <th width="25%">功能维度</th>
    <th>传统方法</th>
    <th>测鱼宝方案</th>
  </tr>
  <tr>
    <td>测量方式</td>
    <td>手工测量工具（游标卡尺等）</td>
    <td>深度学习图像识别（HRNet模型[1](@ref)）</td>
  </tr>
  <tr>
    <td>检测指标</td>
    <td>≤5项基础指标</td>
    <td>14项形态特征 + 体重数据</td>
  </tr>
  <tr>
    <td>适用鱼种</td>
    <td>特定品种</td>
    <td>跨物种通用（支持大黄鱼、鲈鱼等9+品种）</td>
  </tr>
  <tr>
    <td>环境要求</td>
    <td>实验室标准环境</td>
    <td>复杂背景自适应（准确率＞96%[1](@ref)）</td>
  </tr>
</table>

---

## 🎯 检测标准示例
### 大黄鱼关键点标注规范
<img src="https://github.com/miaomiaoge/CeFish/assets/43084054/e65d7965-0400-4525-8b31-435e6606b8fa" width="70%" alt="大黄鱼形态关键点示意图">

---

## 📸 拍摄规范
<table>
  <tr>
    <th width="50%">场景A：体尺+体重检测</th>
    <th>场景B：纯体尺检测</th>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="30%">
      <br>必备元素：实验鱼+电子秤+5mm黑色实线
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="30%">
      <br>必备元素：实验鱼+5mm黑色实线
    </td>
  </tr>
</table>

---

## 🛠️ 安装指南

### 1. 源码获取
git clone https://github.com/miaomiaoge/CeFish.git

### 2. 或直接下载压缩包
wget https://github.com/miaomiaoge/CeFish/archive/refs/heads/main.zip

---

## 硬件驱动管理（CP2102 USB-UART）
### 1. 驱动状态验证
**异常状态标识**​  
当设备管理器出现以下状态时，需重新安装驱动：

<img src="https://github.com/user-attachments/assets/bdf34115-5977-4393-b110-05db46d79531" width="300" style="border:2px solid #ff6b6b; border-radius:8px;">

---

### 2. 驱动安装流程
#### 2.1 官方驱动下载
[![Silicon Labs官方下载入口](https://github.com/user-attachments/assets/2350fd66-5f4f-4288-bb49-649bdf96120d)](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads)  
*支持Windows 10/11系统 | 最新版本v6.7.6 (2024-03更新)*

#### 2.2 安装验证
<img src="https://github.com/user-attachments/assets/b0c8e3ad-ace1-41ce-b8b8-9bf465b42fa6" width="400" style="box-shadow: 0 4px 6px rgba(0,0,0,0.1);">

---

## 系统权限配置

<table>
  <tr>
    <th width="50%">申请授权界面</th>
    <th>授权界面</th>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/34076251-4dc0-4a8d-a166-f26f6cc88576" width="90%">
     
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/c03ece07-c2bd-40ac-ad87-6c0e07dd4cff" width="90%">
    </td>
  </tr>
</table>


---

## 功能验证
### 实时图像采集
<div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px">
  <div style="position:relative">
    <img src="https://github.com/user-attachments/assets/6dbd2f7b-16d7-405f-9981-4b644f5f64d9" style="border:2px solid #4ecdc4">
    <div style="position:absolute; bottom:10px; left:10px; background:rgba(78,205,196,0.8); color:white; padding:5px 10px; border-radius:4px">
      STEP 1: 设备连接
    </div>
  </div>
  <div style="position:relative">
    <img src="https://github.com/user-attachments/assets/c103f0d0-ea6b-4e79-8364-9e976ab3baa4" style="border:2px solid #4ecdc4">
    <div style="position:absolute; bottom:10px; left:10px; background:rgba(78,205,196,0.8); color:white; padding:5px 10px; border-radius:4px">
      STEP 2: 参数设置
    </div>
  </div>
</div>

---

## 技术支持
📧 服务邮箱: tech@cefish.com  
📞 技术支持: 0592-2186 0335  
🌐 知识库: [测鱼宝使用手册](https://xmufgl-wyh.notion.site/b5eaa498d4b04dfb81802616cce8e0a1)
