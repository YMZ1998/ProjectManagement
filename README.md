# ProjectManagement

> 个人项目统一管理仓库 —— 汇总各子项目的仓库链接、技术栈与克隆方式，作为本地代码集合的索引与入口。

## 📑 目录

- [项目总览](#项目总览)
- [子项目详情](#子项目详情)
- [快速克隆](#快速克隆)
- [本地目录约定](#本地目录约定)

---

## 项目总览

| 序号 | 项目名称 | 技术栈 / 类型 | 简介 |
| ---: | :--- | :--- | :--- |
| 1 | [2D-Image-Segmentation](#1-2d-image-segmentation) | Python · 深度学习 | RGB / RGB-D 图像分割实现 |
| 2 | [3rdparty](#2-3rdparty) | C++ · 第三方依赖 | Windows C++ 项目第三方依赖统一集合 |
| 3 | [codex-skills](#3-codex-skills) | 文档 · 安装指南 | Codex 技能与工具在 Windows 下的安装指南 |
| 4 | [labelme](#4-labelme) | Python · 标注工具 | 基于 Python 的图像标注工具 |
| 5 | [AI-Infer](#5-ai-infer) | C++ · 推理动态库 | 图像分割推理动态库（OpenCV + ONNX Runtime） |

---

## 子项目详情

### 1. 2D-Image-Segmentation
- **仓库：** https://github.com/YMZ1998/2D-Image-Segmentation
- **技术栈：** Python、Conda、深度学习（图像分割）
- **说明：** RGB 与 RGB-D 图像的分割实现，提供训练 / 预测 / 后处理 / MIoU 评估等脚本，环境由 `myenv.yml` 定义。
- **克隆：**
  ```bash
  git clone https://github.com/YMZ1998/2D-Image-Segmentation.git
  ```

### 2. 3rdparty
- **仓库：** https://github.com/YMZ1998/3rdparty
- **技术栈：** C++、CMake（第三方依赖）
- **说明：** 集中存放 Windows C++ 项目使用的第三方依赖，覆盖图像处理、推理、界面开发与包管理，通过 `3rdparty.cmake` 为使用方提供统一依赖路径。包含 OpenCV、ONNX Runtime、TensorRT、cuDNN、vcpkg、Dear ImGui、spdlog 等。
- **克隆：**
  ```bash
  git clone https://github.com/YMZ1998/3rdparty.git
  ```

### 3. codex-skills
- **仓库：** https://github.com/YMZ1998/codex-skills
- **技术栈：** 文档、PowerShell 安装指南
- **说明：** 整理 Codex 技能与工具在 Windows PowerShell 下的安装方法，涵盖 frontend-skill、Agent Skills for Context Engineering、Superpowers、Product Design、CodeGraph CLI 与 Codex MCP 集成。
- **克隆：**
  ```bash
  git clone https://github.com/YMZ1998/codex-skills.git
  ```

### 4. labelme
- **仓库：** https://github.com/YMZ1998/labelme
- **技术栈：** Python、PyQt / 图像标注
- **说明：** 基于 Python 的图像标注工具，用于生成分割 / 检测等任务的标注数据。
- **克隆：**
  ```bash
  git clone https://github.com/YMZ1998/labelme.git
  ```

### 5. AI-Infer
- **仓库：** https://github.com/YMZ1998/AI-Infer
- **技术栈：** C++、OpenCV 4.14.0、ONNX Runtime 1.29.0
- **说明：** 图像分割推理动态库，基于 OpenCV 与 ONNX Runtime，推理实现封装于 `ai_infer.dll`；示例程序通过公共 C++ API 调用动态库。
- **克隆：**
  ```bash
  git clone https://github.com/YMZ1998/AI-Infer.git
  ```

---

## 快速克隆

一键克隆全部子项目（PowerShell）：

```powershell
cd D:\Code
$repos = @("2D-Image-Segmentation", "3rdparty", "codex-skills", "labelme", "AI-Infer")
foreach ($r in $repos) { git clone "https://github.com/YMZ1998/$r.git" }
```

---

## 本地目录约定

- 所有子项目统一克隆至 `D:\Code\` 目录下，目录名与仓库名保持一致。
- 仓库地址统一前缀：`https://github.com/YMZ1998/`
- 本仓库（ProjectManagement）仅作为索引与说明，不包含子项目源码。

---

> 维护说明：新增子项目时，请同步更新「项目总览」表格与「子项目详情」章节，并保持克隆指令可一键复制。
