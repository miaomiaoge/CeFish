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

## 软件获取
### 最新版本下载
- ​**正式版地址**：  
  https://doi.org/10.6084/m9.figshare.24278065.v2  
  （注：如遇403访问限制，建议通过VPN访问或发送邮件至2992861134@qq.com索取安装包）

## 核心优势
基于HRNet深度学习框架[1](@ref)，测鱼宝具备以下技术优势：
1. ​**智能检测**​  
   单张图片即可获取14+形态表型数据（体长/体宽/鳍长等），检测精度>96%[1](@ref)
2. ​**多物种适配**​  
   支持大黄鱼、加州鲈、鲤鱼等9大类养殖鱼种，通过迁移学习实现跨物种检测[1](@ref)
3. ​**环境鲁棒性**​  
   自适应处理复杂背景，仅需包含鱼体及5cm黑色参照线即可完成标定[1](@ref)
4. ​**数据完整性**​  
   集成PIT ID识别系统，实现形态数据与个体身份的精准关联

## 检测规范
### 标准检测项（以大黄鱼为例）
<img src="https://github.com/miaomiaoge/CeFish/assets/43084054/e65d7965-0400-4525-8b31-435e6606b8fa" alt="大黄鱼形态检测关键点示意图" width="60%" style="display:block;margin:20px auto">

包含10个形态关键点检测：
1. 吻端 2. 眼球前缘 3. 鳃盖后缘 4. 背鳍起点 5. 臀鳍起点  
6. 尾鳍上叶 7. 尾鳍下叶 8. 胸鳍末端 9. 腹鳍末端 10. 尾柄末端

### 拍摄规范
<table>
  <tr>
    <td width="50%">
      <strong>模式A（含体重检测）</strong><br>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="90%">
      <br>要素：鱼体+电子秤+5cm黑色标定线
    </td>
    <td width="50%">
      <strong>模式B（纯形态检测）</strong><br>
      <img src="https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1" width="90%">
      <br>要素：鱼体+5cm黑色标定线
    </td>
  </tr>
</table>

## 安装与配置
### 1. 环境部署

# 克隆代码仓库
git clone https://github.com/miaomiaoge/CeFish.git

# 或直接下载压缩包
wget https://github.com/miaomiaoge/CeFish/archive/refs/heads/main.zip

<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/29e05213-f44f-4e2d-9e51-7cca4024a54a" alt="测鱼宝系统架构">
</p>

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
