# ProjectManagement

本仓库用于统一管理本地代码集合，记录各子项目仓库链接与克隆指令。

## 仓库列表

### 1. 2D-Image-Segmentation
- 链接：https://github.com/YMZ1998/2D-Image-Segmentation
- 克隆：
```bash
git clone https://github.com/YMZ1998/2D-Image-Segmentation.git
```

### 2. 3rdparty
- 链接：https://github.com/YMZ1998/3rdparty
- 克隆：
```bash
git clone https://github.com/YMZ1998/3rdparty.git
```

### 3. codex-skills
- 链接：https://github.com/YMZ1998/codex-skills
- 克隆：
```bash
git clone https://github.com/YMZ1998/codex-skills.git
```

### 4. labelme
- 链接：https://github.com/YMZ1998/labelme
- 克隆：
```bash
git clone https://github.com/YMZ1998/labelme.git
```

### 5. AI-Infer
- 链接：https://github.com/YMZ1998/AI-Infer
- 克隆：
```bash
git clone https://github.com/YMZ1998/AI-Infer.git
```

---

## 一键克隆全部（PowerShell）
```powershell
cd D:\Code
$repos = @("2D-Image-Segmentation","3rdparty","codex-skills","labelme","AI-Infer")
foreach ($r in $repos) { git clone "https://github.com/YMZ1998/$r.git" }
```

> 路径前缀均为 `https://github.com/YMZ1998/`
