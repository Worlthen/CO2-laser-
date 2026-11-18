# CO2 激光光路与 Collimation 仿真系统 (CO2 Laser Simulation)

基于物理光学与工业级激光加工参数建模的交互式 CO2 激光光路仿真平台，直观展示激光器光源、准直透镜位置移动、Mask 光阑截取、聚焦及工作台加工面能量密度（Fluence）之间的动态映射关系。

---

## 🌐 在线预览 / Live Demo

👉 **[点击直接访问在线交互网页 (GitHub Pages)](https://worlthen.github.io/CO2-laser-/)**

> 提示：如果在线页面尚未开启，可在本仓库 **Settings** -> **Pages** -> **Branch** 选择 `main` / `/(root)` 即可启用。

---

## 📸 功能特性 (Key Features)

1. **光路俯视物理仿真 (Optical Path Simulation)**
   - 包含激光发射源 (Source)、可移动准直透镜 (Collimation Lens)、孔径光阑 (Mask)、f-Theta 聚焦透镜与工作台传感器 (Processing Point @ Table Level)。
   - 动态光线追踪渲染，清晰反映光束发散角与扩束聚焦全流程。

2. **核心加工参数控制 (Parameter Controls)**
   - **Collimation Mag. (准直值)**：120 ~ 1200 连续无级微调（单位 0.1 unit），真实模拟准直透镜的物理位移与扩束比率（Expansion Factor）。
   - **Mask Select (光圈选择)**：
     - `Mask 1`: Small (20)
     - `Mask 2`: Std (40)
     - `Mask 3`: Large (60)

3. **加工点能量与光束质量实时监测 (Energy & Beam Diagnostics)**
   - **Beam Profile (实时光束截面分布图)**：高斯光束截断与平顶度状态指示（Good Flatness / Edge Truncation）。
   - **Lens Position**：透镜实际物理移动距离 (mm)。
   - **Beam Dia. (Mask)**：光阑处的激光束光斑直径。
   - **Efficiency (%)**：Mask 透光率与系统能量利用效率。
   - **Fluence (加工面能量密度)** 与 **Ref. Target (参考标定线)** 动态对齐游标。

---

## 🛠️ 本地运行 (Local Run)

该项目为轻量级零依赖纯前端架构，无需任何 Node.js/Python 构建环境：

1. 克隆本仓库：
   ```bash
   git clone https://github.com/Worlthen/CO2-laser-.git
   ```
2. 双击打开 `index.html` 或 `CO2 laser.html` 即可在任意现代浏览器（Chrome、Edge、Safari、Firefox 等）中运行。

---

## ⚙️ GitHub Pages 网页版配置说明

本仓库已预先配置好根目录部署结构（`index.html` 与 `.nojekyll`）：
1. 进入 GitHub 仓库页面顶部的 **Settings** 选项卡。
2. 在左侧菜单点击 **Pages**。
3. 在 **Build and deployment** 下方的 **Source** 选择 `Deploy from a branch`。
4. **Branch** 选择 `main`，目录保持 `/(root)`，点击 **Save**。
5. 等待 1~2 分钟，即可通过 `https://worlthen.github.io/CO2-laser-/` 预览网页版。
