```markdown
<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/29e05213-f44f-4e2d-9e51-7cca4024a54a">
</p>

---

## 📥 软件获取
**最新版本**  
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
    <td>深度学习图像识别（HRNet模型）</td>
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
```bash
git clone https://github.com/miaomiaoge/CeFish.git
```
或直接下载[ZIP压缩包](https://github.com/miaomiaoge/CeFish/archive/refs/heads/main.zip)

### 2. 驱动配置
<details>
  <summary>点击查看详细驱动安装说明</summary>
  
  **故障诊断**：  
  <img src="https://github.com/user-attachments/assets/bdf34115-5977-4393-b110-05db46d79531" width="30%" alt="驱动异常示意图">

  **解决方案**：  
  1. 访问[Silicon Labs驱动下载页](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
  2. 选择对应系统版本安装
  3. 验证安装结果：  
     <img src="https://github.com/user-attachments/assets/b0c8e3ad-ace1-41ce-b8b8-9bf465b42fa6" width="40%" alt="驱动成功示意图">
</details>

---

## 📱 操作界面
<div align="center">
  <img src="https://github.com/user-attachments/assets/6dbd2f7b-16d7-405f-9981-4b644f5f64d9" width="45%" alt="设备授权界面">
  <img src="https://github.com/user-attachments/assets/c103f0d0-ea6b-4e79-8364-9e976ab3baa4" width="45%" alt="图像采集界面">
</div>

---

## 📚 扩展资源
- 操作手册：[在线文档](https://xmufgl-wyh.notion.site/b5eaa498d4b04dfb81802616cce8e0a1)
- 模型原理：基于HRNet的高分辨率特征融合技术
- 研究支持：已应用于1300+尾大黄鱼表型-基因关联分析
</details>
```
