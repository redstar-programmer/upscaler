# 红星缩放器
使用 FFmpeg、Real-ESRGAN 和 Flowframes 的强大视频升频工具，现在支持 ** 多语言用户界面！

🌐 语言：
英语](README.en.md) | [韩语](README.md) | [日本語](README.ja.md) | [中文](README.zh.md) | [法语](README.zh.md)
[Français](README.fr.md) | [Deutsch](README.de.md) | [Español](README.es.md) | [Português](README.pt.md) | [中文](README.zh.md)
[Русский](README.ru.md) | [Italiano](README.it.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [ภาษาไทททย](README.id.md)
[ภาษาไทย](README.th.md) | [العربية](README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>基于 fmpeg、realesrgan 和 flowframes 的视频缩放工具</strong><br
  <em>基于现代图形用户界面，预设设置，支持多文件处理</em
</p>

---.

下载：[发布](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ 请支持 "redstar "升频器

您喜欢这个项目或想支持它的发展吗？
请捐助一小笔钱，帮助我们开发更好的功能和可靠的更新！

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>****PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>****GitHub 赞助商** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 您对服务器成本、开发时间和一杯咖啡的赞助将大有裨益。谢谢！

## 目录

- 引言](#引言)
- 安装和准备](#安装和准备)
- 主要功能](#Main-Features)
- 如何使用（快速入门）](#How-to-use-quick-start)
- [⚙️ 详细功能描述](#detailed-feature-description)
- 致谢](#致谢)
- 历史](#history)

## 👋 简介
**redstar upscaler 是一款基于 Python 的 GUI 工具，用于使用 `ffmpeg`、`Real-ESRGAN` 和 `Flowframes`，将视频自动升频至更高分辨率。

- 提取视频帧 → 升频 → 合并视频，一步完成
- 支持各种真实图像模型
- 可通过 Flowframes 进行插值
- 自动提取和处理音频编解码器
- 在源位置或指定路径上工作

> ⚠️ 在 Windows 环境中开发和测试。

下面是一个简单的使用演示，点击后会跳转到 YouTube：<br> <br
[![观看演示](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "在 YouTube 上观看")

## 💾 安装和准备工作

1. 安装并找到以下外部工具（注意，分发文件包括 ffmpeg、Real-ESRGAN 和 Flowframes 安装文件（请参阅路径中的程序文件夹）
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - Flowframes](https://github.com/n00mkrad/flowframes) *（可选）*。
2. 解压缩并运行 readstar 的 upscaler.exe
3. 对于 Flowframes，加载的模型可能因用户环境而异，因此请务必运行 Flowframes，并确保 Interpolation 选项卡中的 Interpolation AI 和 AI Model 与 redstar upscaler 的 resources/flowframes_models.ini 版本一致。 <br>用 # 标记注释未加载的模型，并确保 redstar upscaler 设置窗口中的模型顺序与 <br>Flowframes 中的模型顺序一致后再继续。

## 🔧 主要功能。

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
- 多个视频选择和顺序操作
- 添加拖放视频
- 主要节目可用性和直接选择
- 光盘保存模式
- 多语言支持（15 种语言）
<br><br
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
- 保存预设并自动应用
- 自动检测音频编解码器并设置比特率
- 自动检测和选择音频模型
- ✅针对 FFMPEG、real-ESRGAN 和 Flowframes 的详细设置
- ✅ 根据 Flowframes 版本更改选项设置<br>（可通过在主页上指定 flowframes 版本路径更改版本）
<br><br
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
- ✅检查 upscale 执行命令（可复制并在 CMD 上单独执行）
<br><br
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
- 监控缩放操作的整体进度
- ✅ 检查升级日志（日志文件按日期创建在实时文件夹中的日志文件夹中）
- 任务完成后自动清理可交付成果（以 [REDSTAR] 为前缀）
- ✅ 设置任务完成后的操作<br>（什么也不做/退出程序/睡眠/休眠模式/关闭窗口）
<br><br
## 🚀 如何使用（快速启动）

1. 添加视频文件（支持 MP4、MKV、AVI、MOV、FLV、WMV、MPG、WEBM、3GP、OGV）
2. 指定工作位置或勾选 "使用原始文件路径 "复选框
3. 点击已添加视频上的 "设置 "按钮
4. 对 ffmpeg、realESRGAN、Flowframes 进行详细设置
5. 单击 "批量应用于所有文件"/"仅应用于选定的文件
6. 单击 "确认 "按钮
7. 选中要执行的命令并单击 "开始任务 "按钮

> 工作结果将是两个文件：所选文件夹中的缩放视频和帧插值视频。
> 完成的文件将以 [REDSTAR] 为前缀保存。
---]

## ⚙️ 详细功能说明

| 项目 | 说明
|------|------|
| 设置工作路径** | 提供默认路径或 "使用原始文件路径 "选项
| 支持大多数视频格式，包括 MP4、MKV、AVI、MOV、FLV、WMV、MPG、WEBM、3GP、OGV 等。
| 自动检测 realesr-animevideov3、realesr-general、4xplus 等。
| 音频处理** | 支持各种格式的编码，如 "aac"、"mp3"、"flac "等。
| 可设置插值（FPS ×2、 ×4、 ×8）。
** 磁盘保存模式** | 自动删除中间图像

## 🙏 鸣谢

- realesrgan by [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes 作者 [n00mkrad](https://github.com/n00mkrad/flowframes)
- 如果您想为本项目做出贡献或提出功能建议，请在 [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues) 上留言。

# 📜 历史

v 1.1.0
 > 1. 菜单配置（打开文件、关闭文件、日志设置、语言设置）
 增加多语言设置（可用语言：韩语、英语、日本语、中文、Français、Deutsch、Español、Português、Русский、Tiếng Việt、印度尼西亚语、ไทย、 Italiano、العربية） > 3.
 更改了信息和部分代码，以适应新增的语言设置 > 4.
 > 一些用户界面配置更改
 显示 ffmpeg、real-ESRGAN 和 Flowframes 版本信息（主屏幕） > 6.
 支持 Flowframes 1.41.0 版本（由于 1.41.0 版本中的 cmd 命令问题，目前只支持 1.40.0 和 1.36.0 版本） > 7.
 > 修正了 AI 模型项目以小写字母显示的问题
 添加了 FFMPEG 选项（像素、视频编解码器）--根据用户电脑显示选项 > 9.
 增强了对每个用户电脑的 CUDA 检查 - 检查可用性和 GPU 类型（主屏幕） > 9.

v 1.0.0
 > 全部代码重写
 > 用户界面更改
 > 增加了可处理的视频/音频范围
 > 增加了光盘保存模式
 > 包括主要节目的发布

v 0.1.92
 > 1.修正了在改变 Flowframes 路径时，由于 AI 模型组合框中的重复输入而导致插值失败的问题。
 > 增加了插值时组合框选择状态的检查代码。

v 0.1.91
 增加了一些与 Flowframes 相关的组合框刷新功能 > 2.
 > 调整了一些分发文件

v 0.1.9
 应用 Flowframes 模型更改 > 2.
 > 新的 Flowframes 1.36.0 模型、1.40.0 模型实现
 不再出现 Flowframes 命令行失败 > 4.
 现在可以通过拖放添加文件 > 5.
 > 修复了 Flowframes 设置未被应用的问题

v 0.1.8
 检查版本时修正了新版本检查错误 > 2.
 > 如果 flowframes 安装在默认路径下（例如 C:\Users\Administrator\AppData\Local\Flowframes），请在启动前将路径设为默认。
 > 添加多个文件选择时，应用程序会因错误而崩溃。
 > 4.修正了添加多个文件后启动任务时出现的错误

v 0.1.7
 方案大小可更改 > 2.
 > 修正了处理无声音文件时的错误
 > 更改了整个用户界面配置（重新配置以适应尺寸变化）

v 0.1.6
 修正了字体大小因屏幕分辨率而异的问题 > 2.
 > 修正了程序标题不显示新版本信息的问题
 > 3. 修复了 config.ini 文件保存路径不同的问题
 > 改变 realesrgan 放大系数时，放大模型组合框也会改变。
 > 已添加更新检查功能
 > 修复了一些逻辑
 > 更改了分辨率和帧速率表的颜色
 > 允许用户编辑分辨率（必须输入 1024x768）

v 0.1.5
 修复了选择 FLOWFRAMES 插值 AI 时 AI 模型不会自动更改的问题 > 2.
 修正了流帧插值未根据所选选项进行插值的问题 > 3.
 > 增加了 "FPS 计算方法 "组合框，以防止某些视频的 FPS 计算错误。
        -> 增加了 "FPS 计算方法 "组合框，以防止某些视频的 FPS 计算错误。
 选择视频文件时显示视频信息获取进度 > 5.
 打开文件后再次选择文件时，默认打开上一次选择的文件夹 > 5.

v 0.1.4
 > 1. 更改了读取 config.ini 文件的方式
 > 更改了从 Python AV 到 ffmpeg 获取视频信息的方式
 > 3. 增加了任务完成后关闭窗口的功能
 > 4. 在任务列表中鼠标移动时以工具提示形式显示完整文件名
 > 5. 显示任务列表中每个文件的分辨率（之前）/分辨率（之后）/FPS（之前）/FPS（之后
 > 删除 FPS 输入框（因为每个文件都有上述标签）
 删除输出 FPS 估计值大小（由于上述针对每个文件的标记而删除） > 8.
 > 8. 以两个进度条的形式显示所有文件/任务的进度

v 0.1.3
 > 修复了加载文件时某些 FPS 信息错误的文件 FPS 计算错误

v 0.1.2
 > 用户界面配置更改
 > 内部逻辑更改
 > 修正了当选择以下两个模型时 realesrgan 模型无法运行的问题
 > 改变了使用 realesrgan 模型的方式
 > -> 将新模型文件（*.param）复制到 realesrgan 安装文件夹下的模型文件夹中即可使用。
 显示目标图像最后一个文件的宽度、高度信息和估计的放大尺寸，以便使用 > 6.
 > 编写代码以迁移 config.ini 文件
 > 更改 FFMPEG 分解图像 AAC -> FLAC
 > 8. 其他错误修复

v 0.1.1
 > 首次使用 FFMEPG、realesrgan 和 flowframes 编写视频升级程序