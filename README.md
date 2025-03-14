<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/29e05213-f44f-4e2d-9e51-7cca4024a54a" alt="CeFish Logo">
</p>

<h1 align="center"> 测鱼宝——智能鱼类表型采集与PIT记录系统</h1>

<div align="center">
  <img src="https://img.shields.io/badge/Version-2.5.0-brightgreen" alt="版本">
  <img src="https://img.shields.io/github/downloads/miaomiaoge/CeFish/total" alt="下载量">
  <img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue" alt="许可协议">
</div>


# 测鱼宝使用指南
---
## 📥 软件获取
**上个版本**​  
`v2.0.1` 发布于2023年11月  
[![DOI](https://img.shields.io/badge/DOI-10.6084/m9.figshare.24278065.v2-blue)](https://doi.org/10.6084/m9.figshare.24278065.v2)  

⚠️ 访问提示：  
- 遇到403错误建议使用VPN访问
- 或发送请求至技术支持邮箱：2992861134@qq.com

---
## 🏆 核心优势
<table>
  <tr>
    <th width="25%">功能维度</th>
    <th>传统方法</th>
    <th>其他深度学习方法</th>
    <th>测鱼宝方案</th>
  </tr>
  <tr>
    <td width="25%">测量方式</td>
    <td width="25%">手工测量工具（游标卡尺等）</td>
    <td width="25%">目标检测，目标分割，关键点检测</td>
    <td width="25%">关键点检测</td>
  </tr>
  <tr>
    <td width="25%">检测指标</td>
    <td width="25%">≤5项基础指标</td>
    <td width="25%">≤7项基础指标</td>
    <td width="25%">15项形态特征 + 体重数据</td>
  </tr>
  <tr>
    <td width="25%">适用鱼种</td>
    <td width="25%">跨物种通用</td>
    <td width="25%">特定品种</td>
    <td width="25%">跨物种通用（支持大黄鱼、鲈鱼、鲤鱼等10+品种）</td>
  </tr>
  <tr>
    <td>环境要求</td>
    <td>标准环境</td>
    <td>标准环境</td>
    <td>复杂背景自适应（准确率＞96%）</td>
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
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="100%">
      <br>必备元素：实验鱼+电子秤+5mm黑色实线
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="100%">
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

#### 2.2 安装验证
<table>
  <tr>
    <th width="50%">下载安装</th>
    <th>安装成功</th>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/a57a0d91-15f9-4e2f-90de-84e503aa818e" style="box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/b0c8e3ad-ace1-41ce-b8b8-9bf465b42fa6" style="box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    </td>
  </tr>
</table>
">

---

## 软件权限配置

<table>
  <tr>
    <th width="50%">申请授权界面</th>
    <th>授权界面</th>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/34076251-4dc0-4a8d-a166-f26f6cc88576" width="%90">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/5c2cf772-6a4a-47b6-9d23-8421d4aaad3c" width="%90">     
    </td>
  </tr>
</table>


---

## 功能验证

<table>
  <tr>
    <th width="50%">图像采集</th>
    <th>表型测量</th>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/6dbd2f7b-16d7-405f-9981-4b644f5f64d9" width="%90">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/c103f0d0-ea6b-4e79-8364-9e976ab3baa4" width="%90">     
    </td>
  </tr>
</table>

---

## 技术支持
📧 服务邮箱: 2992861134@qq.com  
📞 技术支持: 15853246086  
🌐 知识库: [测鱼宝使用手册](https://xmufgl-wyh.notion.site/b5eaa498d4b04dfb81802616cce8e0a1)
