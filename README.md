# TSGen ⚛️

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.10%2B-brightgreen)](https://www.python.org/)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey)]()

TSGen (**Training Set Generator**) 是一个用于 **ReaxFF 力场训练集准备** 与 **Gaussian 任务批量生成/解析** 的桌面软件。  
它集成了图形界面（tkinter）和高质量 3D 可视化，帮助科研人员快速构建训练集并进行自动化计算。

## ✨ 功能特性

- 📄 **Gaussian 输出解析**  
  批量读取 `.log` 文件，提取能量、几何、频率等关键信息。  

- 🔬 **3D 结构可视化**  
  内置渲染器，高质量球棍模型，支持原子选择与几何测量。  

- ⚙️ **GEO 文件输出**  
  自动或手动生成 ReaxFF 约束（BOND / ANGLE），支持扫描任务。  

- 📊 **训练集管理**  
  一键生成 `trainset.in`，可批量管理 Gaussian/DFT 计算任务。  

- 🚀 **一键运行**  
  已打包为 Windows 可执行文件，无需 Python 环境，下载即用。  

## 📥 下载与安装

你可以在 https://github.com/child112/TSGen/releases 下载最新的安装包。

1. 下载压缩包 `TsGen_x.x.zip`  
2. 解压到任意目录（建议避免路径中包含中文或空格）  
3. 双击 `TsGen.exe` 启动程序  

无需安装 Python 或额外依赖。

## 📂 目录结构

解压后的目录大致如下：

TsGen/
│
├─ TsGen.exe <-- 主程序
├─ TsGen_icon_v6.ico <-- 程序图标
├─ tsgen/ <-- 软件核心代码
│ ├─ io/
│ ├─ gui/
│ ├─ web/assets/ <-- 内置网页资源
│ └─ ...
├─ 示例文件/ <-- 附带的样例 .gjf / .log
└─ README.md

## 🖥️ 使用说明

1. 打开软件后，在主界面选择对应功能：  
   - **Gaussian log 解析**：导入 log 文件，提取优化结果、能量等信息。  
   - **结构可视化**：以 3D 球棍模型显示分子，支持测量距离、角度、二面角。  
   - **GEO 输出**：生成带约束的 GEO 文件，可选手动设置或自动生成。  
   - **训练集批量生成**：自动构建 `trainset.in` 文件，并可管理计算任务。  

2. 所有生成的文件会保存到用户指定的目录。  

3. 如需批量任务，只需在界面中导入文件夹即可。  

## ⚡ 常见问题 FAQ

- **双击没反应 / 闪退**  
  请确认 `tsgen/web/assets/` 文件夹未丢失。  

- **提示缺少 DLL**  
  安装 [Microsoft Visual C++ Redistributable 2015–2022](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist)。  


