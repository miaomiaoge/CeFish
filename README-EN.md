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
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="90%">
      <br>必备元素：实验鱼+电子秤+5mm黑色实线
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="90%">
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
<style>
.driver-container {
    max-width: 1200px;
    margin: 2rem auto;
    padding: 0 1.5rem;
    font-family: 'Segoe UI', system-ui;
}

.section-card {
    background: #f8f9fa;
    border-radius: 12px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.05);
    padding: 2rem;
    margin-bottom: 2rem;
}

.section-title {
    color: #2c3e50;
    border-left: 4px solid #3498db;
    padding-left: 1rem;
    margin: 1.5rem 0;
}

.img-grid {
    display: grid;
    gap: 1.5rem;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}

.driver-img {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    transition: transform 0.2s;
    width: 100%;
    height: auto;
}

.driver-img:hover {
    transform: translateY(-3px);
}

.download-card {
    background: linear-gradient(135deg, #3498db, #2980b9);
    color: white;
    padding: 2rem;
    border-radius: 12px;
    text-align: center;
}

.download-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.8rem;
    padding: 1rem 2rem;
    background: rgba(255,255,255,0.15);
    border: 2px solid rgba(255,255,255,0.3);
    border-radius: 50px;
    transition: all 0.3s;
}

.download-btn:hover {
    background: rgba(255,255,255,0.25);
    transform: scale(1.05);
}

@media (max-width: 768px) {
    .img-grid {
        grid-template-columns: 1fr;
    }
}
</style>

<div class="driver-container">
    <!-- 驱动检查 -->
    <div class="section-card">
        <h2 class="section-title">驱动状态检测</h2>
        <div class="img-grid">
            <img src="https://github.com/user-attachments/assets/bdf34115-5977-4393-b110-05db46d79531" 
                 alt="设备管理器驱动异常示意图"
                 class="driver-img">
        </div>
        <p style="color: #e74c3c; margin-top: 1rem;">⚠️ 黄色感叹号标识表示驱动异常（参考网页1）</p>
    </div>

    <!-- 驱动安装 -->
    <div class="section-card">
        <h2 class="section-title">驱动安装指南</h2>
        <div class="download-card">
            <a href="https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads" 
               class="download-btn"
               target="_blank">
                <svg width="24" height="24" fill="currentColor" style="margin-right:8px;">...</svg>
                访问 Silicon Labs 官方下载
            </a>
            <p style="margin-top:1.5rem;">最新版本：v6.7（2025-02-20更新）</p>
        </div>
        
        <div class="img-grid" style="margin-top:2rem;">
            <img src="https://github.com/user-attachments/assets/b0c8e3ad-ace1-41ce-b8b8-9bf465b42fa6" 
                 alt="驱动安装成功示意图"
                 class="driver-img">
        </div>
    </div>

    <!-- 设备授权 -->
    <div class="section-card">
        <h2 class="section-title">设备权限配置</h2>
        <div class="img-grid">
            <img src="https://github.com/user-attachments/assets/34076251-4dc0-4a8d-a166-f26f6cc88576" 
                 alt="Windows设备授权界面"
                 class="driver-img">
            <img src="https://github.com/user-attachments/assets/c03ece07-c2bd-40ac-ad87-6c0e07dd4cff" 
                 alt="Linux设备授权界面"
                 class="driver-img">
        </div>
        <p style="margin-top:1rem;">➡️ Ubuntu系统需要执行 <code>sudo chmod 666 /dev/ttyUSB0</code>（参考网页3）</p>
    </div>

    <!-- 功能演示 -->
    <div class="section-card">
        <h2 class="section-title">串口功能验证</h2>
        <div class="img-grid">
            <img src="https://github.com/user-attachments/assets/6dbd2f7b-16d7-405f-9981-4b644f5f64d9" 
                 alt="串口调试工具界面"
                 class="driver-img">
            <img src="https://github.com/user-attachments/assets/c103f0d0-ea6b-4e79-8364-9e976ab3baa4" 
                 alt="数据收发验证界面"
                 class="driver-img">
        </div>
    </div>
</div>
