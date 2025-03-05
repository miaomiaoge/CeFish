```markdown
# 测鱼宝简介
<p align="center">
  <img src="https://github.com/miaomiaoge/CeFish/assets/43084054/29e05213-f44f-4e2d-9e51-7cca4024a54a" alt="yu2">
</p>

## 上一版本测鱼宝软件下载地址
[上一版本测鱼宝软件下载](https://doi.org/10.6084/m9.figshare.24278065.v2)

**注意**：若下载时出现 403 错误，你可以使用 VPN 进行下载，或者发送邮件至 [2992861134@qq.com](mailto:2992861134@qq.com) 索取最新版测鱼宝安装包。

## 测鱼宝优点
测鱼宝是一款功能强大的软件，它集成了鱼类拍照、PIT ID 识别功能，能够收集和记录包括体长、体宽、眼宽、鳍长等 14 个体型特征以及体重信息。

与传统的手工测量记录方式相比，测鱼宝具有显著优势。它不仅极大地减少了人工劳动量，还确保了测量结果的准确性和可靠性。与其他同类产品相比，测鱼宝的优势更加突出：
1. **测量过程智能高效**：只需一张图片，即可测得各种表型性状。
2. **表型性状全面覆盖**：涵盖体重、全长、体长、头长、躯干长、尾长、吻长、眼长、眼后头长、尾柄长、体高、尾柄高、胸鳍长、尾鳍长、臀鳍长等。
3. **可测鱼类种类广泛**：目前可检测的鱼类包括但不限于大黄鱼、加州鲈、桂花鲈、鲤鱼、巴浪鱼、黄翅鱼、罗非鱼、黄骨鱼、鲫鱼等。
4. **图片要求低**：可检测各种背景下的鱼类关键点，若事先获知缩放比例，还能直接获得鱼类真实体尺。

## 检测标准
以大黄鱼为例，可检测的关键点及体尺性状如下图所示：
![检测标准](https://github.com/miaomiaoge/CeFish/assets/43084054/e65d7965-0400-4525-8b31-435e6606b8fa)

## 私有照片拍摄标准
- **图 A**：用于检测体重和体尺，包含 3 个元素，即鱼、电子秤和黑色实线。
- **图 B**：仅用于检测体尺，包含 2 个元素，即鱼和黑色实线。

![私有照片拍摄标准](https://github.com/user-attachments/assets/71d7d0f5-53b0-4c8d-ab71-2945c7c284e1)

## 测鱼宝使用流程
### 1. 下载并解压
你可以通过以下两种方式获取测鱼宝：
- 使用 `git` 命令克隆仓库：
```bash
git clone https://github.com/miaomiaoge/CeFish.git
```
- 直接点击 **Download ZIP** 下载压缩包，然后解压。

### 2. UART 驱动检查与重新安装 CP2102 USB to UART Bridge Controller
#### 1) 检查串口驱动
打开“设备管理器”，若出现以下画面，则表示串口驱动安装失败：
![串口驱动安装失败](https://github.com/user-attachments/assets/bdf34115-5977-4393-b110-05db46d79531)

#### 2) 重新安装驱动
你可以通过点击下方图片跳转到官方安装地址进行驱动安装：
<a href="https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads">
  <img src="https://github.com/user-attachments/assets/2350fd66-5f4f-4288-bb49-649bdf96120d" 
       alt="Silicon Labs USB to UART Bridge VCP Drivers Download" 
       width="80%">
</a>

安装成功画面如下：
![安装成功](https://github.com/user-attachments/assets/b0c8e3ad-ace1-41ce-b8b8-9bf465b42fa6)

#### 3) 申请授权
![申请授权 1](https://github.com/user-attachments/assets/34076251-4dc0-4a8d-a166-f26f6cc88576)
![申请授权 2](https://github.com/user-attachments/assets/c03ece07-c2bd-40ac-ad87-6c0e07dd4cff)

#### 4) 拍照功能
![拍照功能 1](https://github.com/user-attachments/assets/6dbd2f7b-16d7-405f-9981-4b644f5f64d9)
![拍照功能 2](https://github.com/user-attachments/assets/c103f0d0-ea6b-4e79-8364-9e976ab3baa4)

## 测鱼宝使用手册
[点击查看测鱼宝使用手册](https://xmufgl-wyh.notion.site/b5eaa498d4b04dfb81802616cce8e0a1?pvs=4)
```

### 润色优化说明：
1. **格式优化**：
    - 对图片添加 `alt` 属性，增强可访问性。
    - 使用列表形式整理文字内容，如使用手册的注意事项、测鱼宝优点等，使逻辑更清晰。
    - 代码块使用 `bash` 语法高亮，让代码更易读。
2. **文字表述优化**：
    - 统一语言风格，使描述更加简洁明了。
    - 补充完整句子结构，增强内容的流畅性。
3. **链接优化**：将纯文本链接转换为 Markdown 链接格式，提高可读性和交互性。 
