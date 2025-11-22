# Design Guide | 设计指南

> **📚 Student Handbook for Laser Cutting & 3D Printing**  
> **📚 激光切割和 3D 打印学生手册**

This guide will help you understand the design rules, common pitfalls, and best practices for digital fabrication.

本指南将帮助你了解数字制造的设计规则、常见陷阱和最佳实践。

---

## 📑 Table of Contents | 目录

1. [Laser Cutting Design Rules](#laser-cutting-design-rules--激光切割设计规则)
2. [3D Printing Design Rules](#3d-printing-design-rules--3d-打印设计规则)
3. [Inkscape Tutorial](#inkscape-tutorial--inkscape-教程)
4. [Adobe Illustrator Tutorial](#adobe-illustrator-tutorial--adobe-illustrator-教程)
5. [Tinkercad Tutorial](#tinkercad-tutorial--tinkercad-教程)
6. [Common Mistakes to Avoid](#common-mistakes-to-avoid--常见错误避免)
7. [Design Best Practices](#design-best-practices--设计最佳实践)

---

## 🔷 Laser Cutting Design Rules | 激光切割设计规则

### What is Laser Cutting? | 什么是激光切割？

Laser cutting uses a high-powered laser beam to cut through materials like wood, acrylic, and cardboard. The laser follows vector paths in your design file.

激光切割使用高功率激光束切割木材、亚克力和纸板等材料。激光沿着设计文件中的矢量路径移动。

### ✅ Critical Design Requirements | 关键设计要求

#### 1. Vector Paths Only | 仅矢量路径

**✅ CORRECT | 正确:**
- All lines must be vector paths (not raster images) (所有线条必须是矢量路径（非光栅图像）)
- Shapes made with Bezier curves or straight lines (使用贝塞尔曲线或直线制作的形状)
- Scalable without losing quality (可缩放而不失真)

**❌ WRONG | 错误:**
- PNG/JPG images (PNG/JPG 图像)
- Imported photos (导入的照片)
- Text that hasn't been converted to paths (未转换为路径的文本)

#### 2. Line Width (Stroke) | 线宽（描边）

**✅ CORRECT | 正确:**
- **0.01 mm to 0.05 mm** (cutting line) (**0.01 毫米到 0.05 毫米**（切割线）)
- Hair line stroke (发丝描边)
- Pure RGB color (usually Red: 255,0,0 for cutting) (纯 RGB 颜色（通常切割用红色：255,0,0）)

**❌ WRONG | 错误:**
- Thick lines (> 1 mm) (粗线（> 1 毫米）)
- Filled shapes without stroke (无描边的填充形状)
- Multiple overlapping lines (多条重叠线条)

**Why it matters | 为什么重要:**
Thick lines waste material and time. The laser only needs a thin path to follow.

粗线浪费材料和时间。激光只需要一条细路径即可跟随。

#### 3. Closed Paths | 闭合路径

**✅ CORRECT | 正确:**
- All shapes must be completely closed (所有形状必须完全闭合)
- No gaps in the path (路径中没有间隙)
- Start point = End point (起点 = 终点)

**❌ WRONG | 错误:**
- Open paths with gaps (有间隙的开放路径)
- Disconnected line segments (断开的线段)
- Almost-closed shapes (几乎闭合的形状)

**How to check | 如何检查:**
- Zoom in to 800% and look for gaps (放大到 800% 并查找间隙)
- Select all → check for "Open path" warnings (全选 → 检查"开放路径"警告)

#### 4. Minimum Feature Size | 最小特征尺寸

**✅ CORRECT | 正确:**
- Minimum width of any feature: **≥ 1 mm** (任何特征的最小宽度：**≥ 1 毫米**)
- Gaps between elements: **≥ 1 mm** (元素之间的间隙：**≥ 1 毫米**)
- Text height: **≥ 5 mm** (文本高度：**≥ 5 毫米**)

**❌ WRONG | 错误:**
- Tiny details < 1 mm (小于 1 毫米的细小细节)
- Very thin connecting bridges (非常细的连接桥)
- Small text < 3 mm (小于 3 毫米的小文本)

**Why it matters | 为什么重要:**
Features that are too small will:
- Break easily (容易断裂)
- Burn during cutting (切割时燃烧)
- Not cut cleanly (切割不干净)

#### 5. Material Considerations | 材料考虑

**Typical materials | 典型材料:**
- **3mm Plywood** (3毫米胶合板): Good for beginners (适合初学者)
- **3mm Acrylic** (3毫米亚克力): Clean edges, more expensive (边缘干净，更贵)
- **Cardboard** (纸板): Practice material (练习材料)

**Design adjustments | 设计调整:**
- **Kerf**: Laser removes ~0.2 mm of material (激光移除约 0.2 毫米材料)
- For tight fits, make holes 0.2 mm larger (对于紧密配合，将孔加大 0.2 毫米)
- For tabs, make them 0.2 mm smaller (对于榫头，将其缩小 0.2 毫米)

---

## 🔶 3D Printing Design Rules | 3D 打印设计规则

### What is 3D Printing? | 什么是 3D 打印？

3D printing (FDM) builds objects layer by layer from melted plastic. Your design must be printable from bottom to top.

3D 打印（FDM）从熔化的塑料逐层构建物体。你的设计必须能够从底部到顶部打印。

### ✅ Critical Design Requirements | 关键设计要求

#### 1. Manifold (Watertight) Model | 流形（水密）模型

**✅ CORRECT | 正确:**
- Model is a single closed solid (模型是单个封闭实体)
- No holes in the mesh (网格中没有孔)
- All faces are properly connected (所有面都正确连接)
- "Watertight" geometry (水密几何体)

**❌ WRONG | 错误:**
- Open surfaces (开放表面)
- Intersecting geometry (相交几何体)
- Floating vertices (浮动顶点)
- Non-manifold edges (非流形边)

**How to check | 如何检查:**
- In Tinkercad: All shapes should be "Grouped" (在 Tinkercad 中：所有形状应该"分组")
- Model should have "volume" when exported (导出时模型应该有"体积")

#### 2. Minimum Wall Thickness | 最小壁厚

**✅ CORRECT | 正确:**
- **Minimum thickness: 1.2 mm** (**最小厚度：1.2 毫米**)
- Recommended: 2–3 mm for strength (推荐：2–3 毫米以获得强度)
- Consistent thickness throughout (整体厚度一致)

**❌ WRONG | 错误:**
- Thin walls < 1 mm (薄壁 < 1 毫米)
- Paper-thin features (纸薄特征)
- Sharp knife-like edges (锋利的刀状边缘)

**Why it matters | 为什么重要:**
Thin features will:
- Fail to print (无法打印)
- Break easily (容易断裂)
- Warp during printing (打印时翘曲)

#### 3. Overhang Angle | 悬垂角度

**✅ CORRECT | 正确:**
- Maximum overhang: **≤ 45°** from vertical (最大悬垂：从垂直**≤ 45°**)
- Use gradual angles (使用渐进角度)
- Self-supporting geometry (自支撑几何体)

**❌ WRONG | 错误:**
- Horizontal overhangs (> 45°) (水平悬垂（> 45°）)
- Floating features (浮动特征)
- Upside-down designs (倒置设计)

**The 45° Rule | 45° 规则:**
```
    ✅ OK         ❌ NOT OK
    /\            ____
   /  \              \
  /    \              \
 /______\          ____\
```

**Why it matters | 为什么重要:**
Features over 45° will:
- Sag during printing (打印时下垂)
- Need support material (需要支撑材料)
- Have rough surfaces (表面粗糙)

#### 4. First Layer Adhesion | 第一层附着

**✅ CORRECT | 正确:**
- Large flat bottom surface (大平底面)
- Good contact with build plate (与打印床良好接触)
- No small contact points (没有小接触点)

**❌ WRONG | 错误:**
- Tiny bottom surface (极小的底面)
- Sphere/curved bottom (球形/弯曲底部)
- Tall thin tower (高细塔)

**Design tip | 设计提示:**
- Add a base/platform if needed (如需要添加底座/平台)
- Chamfer bottom edges (倒角底边)

#### 5. Size Limitations | 尺寸限制

**✅ CORRECT | 正确:**
- Maximum size: **50 mm** (any dimension) (最大尺寸：**50 毫米**（任何维度）)
- Realistic print time: < 2 hours (实际打印时间：< 2 小时)
- Efficient use of volume (高效使用体积)

**❌ WRONG | 错误:**
- Massive solid blocks (大块实体)
- Oversized models (超大模型)
- Wasteful internal volume (浪费的内部体积)

**Size optimization | 尺寸优化:**
- Hollow out large volumes (挖空大体积)
- Use shells instead of solids (使用壳体而非实体)
- Scale down if too large (如太大则缩小)

---

## 🎨 Inkscape Tutorial | Inkscape 教程

### Getting Started | 入门

#### Installation | 安装
1. Download from https://inkscape.org/release/
2. Install for your operating system (为你的操作系统安装)
3. Launch Inkscape (启动 Inkscape)

#### Interface Overview | 界面概览
- **Toolbox** (Left): Drawing tools (左侧：绘图工具)
- **Canvas** (Center): Work area (中央：工作区)
- **Properties** (Right): Object properties (右侧：对象属性)
- **Top Bar**: File, Edit, View menus (顶部栏：文件、编辑、视图菜单)

### Essential Tools | 基本工具

#### 1. Selection Tool (Arrow) | 选择工具（箭头）
**Shortcut | 快捷键:** `S` or `F1`

**Use for | 用于:**
- Moving objects (移动对象)
- Resizing shapes (调整形状大小)
- Rotating elements (旋转元素)

#### 2. Rectangle Tool | 矩形工具
**Shortcut | 快捷键:** `R` or `F4`

**How to use | 如何使用:**
1. Click and drag to create rectangle (点击并拖动创建矩形)
2. Hold `Ctrl` for square (按住 `Ctrl` 创建正方形)
3. Adjust corners with circle handles (使用圆形手柄调整角)

#### 3. Circle Tool | 圆形工具
**Shortcut | 快捷键:** `C` or `F5`

**How to use | 如何使用:**
1. Click and drag to create circle/ellipse (点击并拖动创建圆形/椭圆)
2. Hold `Ctrl` for perfect circle (按住 `Ctrl` 创建完美圆形)
3. Adjust with handles (使用手柄调整)

#### 4. Bezier Tool (Pen) | 贝塞尔工具（钢笔）
**Shortcut | 快捷键:** `B` or `F6`

**How to use | 如何使用:**
1. Click to place points (点击放置点)
2. Click and drag for curves (点击并拖动创建曲线)
3. Press `Enter` to finish path (按 `Enter` 完成路径)

#### 5. Text Tool | 文本工具
**Shortcut | 快捷键:** `T` or `F8`

**How to use | 如何使用:**
1. Click to place text cursor (点击放置文本光标)
2. Type your text (输入文本)
3. **IMPORTANT**: Convert to path before exporting! (**重要**：导出前转换为路径！)
   - Select text → Path → Object to Path (选择文本 → Path → Object to Path)

### Critical Operations | 关键操作

#### Converting Objects to Paths | 将对象转换为路径
**Why | 为什么:** Laser cutters need vector paths, not shape objects (激光切割机需要矢量路径，而非形状对象)

**How | 如何:**
1. Select all objects (`Ctrl + A`) (全选对象)
2. Path → Object to Path (Path → Object to Path)
3. Check: objects should no longer have circle/square handles (检查：对象不应再有圆形/方形手柄)

#### Boolean Operations | 布尔运算
**Use for | 用于:** Combining or subtracting shapes (组合或减去形状)

**Union (Combine) | 联合（组合):**
- Select 2+ shapes (选择 2+ 个形状)
- Path → Union (`Ctrl + +`) (Path → Union)
- Creates single merged shape (创建单个合并形状)

**Difference (Subtract) | 差集（减去）:**
- Select shapes (top one will be subtracted) (选择形状（顶部的将被减去）)
- Path → Difference (`Ctrl + -`)
- Creates cutout (创建镂空)

**Intersection (共同部分):**
- Path → Intersection (`Ctrl + *`)
- Keeps only overlapping area (仅保留重叠区域)

#### Setting Stroke Width | 设置描边宽度
**Critical for laser cutting! | 对激光切割至关重要！**

**Method 1: Fill and Stroke Panel | 方法1：填充和描边面板**
1. Select object (选择对象)
2. Object → Fill and Stroke (`Ctrl + Shift + F`)
3. Stroke Style tab (描边样式标签)
4. Set Width to **0.01 mm** (将宽度设置为 **0.01 毫米**)

**Method 2: Stroke Width in Toolbar | 方法2：工具栏中的描边宽度**
1. Select object (选择对象)
2. Top toolbar → "Stroke width" field (顶部工具栏 → "描边宽度"字段)
3. Type `0.01 mm` (输入 `0.01 mm`)

### Exporting to DXF | 导出为 DXF

**Step-by-step | 分步指南:**

1. **Prepare your design | 准备设计:**
   - Select all (`Ctrl + A`) (全选)
   - Path → Object to Path (Path → Object to Path)
   - Check all paths are closed (检查所有路径都已闭合)

2. **Set document size | 设置文档大小:**
   - File → Document Properties (File → Document Properties)
   - Set units to **mm** (将单位设置为 **毫米**)
   - Set page size to match your design (设置页面大小以匹配设计)

3. **Export | 导出:**
   - File → Save As (File → Save As)
   - Format: Desktop Cutting Plotter (DXF) (格式：Desktop Cutting Plotter (DXF))
   - Choose location and filename (选择位置和文件名)
   - Click Save (点击保存)

4. **Verify | 验证:**
   - File size should be small (< 1 MB) (文件大小应该很小（< 1 MB）)
   - Open in text editor to check it's not empty (在文本编辑器中打开以检查不为空)

---

## 🎨 Adobe Illustrator Tutorial | Adobe Illustrator 教程

### Getting Started | 入门

#### Interface Overview | 界面概览
- **Toolbox** (Left): Tools (左侧：工具)
- **Canvas** (Center): Artboard (中央：画板)
- **Panels** (Right): Properties, Layers, etc. (右侧：属性、图层等)

### Essential Tools | 基本工具

#### 1. Selection Tool (V) | 选择工具
**Shortcut | 快捷键:** `V`
- Basic selection and movement (基本选择和移动)

#### 2. Direct Selection Tool (A) | 直接选择工具
**Shortcut | 快捷键:** `A`
- Edit individual anchor points (编辑单个锚点)

#### 3. Pen Tool (P) | 钢笔工具
**Shortcut | 快捷键:** `P`
- Create custom paths (创建自定义路径)

#### 4. Shape Tools | 形状工具
- Rectangle (`M`), Ellipse (`L`)
- Polygon, Star tools (多边形、星形工具)

### Critical Operations | 关键操作

#### Setting Stroke Width | 设置描边宽度

**Method 1: Stroke Panel | 方法1：描边面板**
1. Window → Stroke (Window → Stroke)
2. Set Weight to **0.01 pt** (将粗细设置为 **0.01 点**)
3. Make sure Cap and Corner are set (确保设置了端点和角)

**Method 2: Properties Panel | 方法2：属性面板**
1. Select object (选择对象)
2. Properties panel → Stroke weight (属性面板 → 描边粗细)
3. Enter `0.01 pt` (输入 `0.01 点`)

#### Expanding Text and Strokes | 扩展文本和描边

**Convert text to outlines | 将文本转换为轮廓:**
1. Select text (选择文本)
2. Type → Create Outlines (`Ctrl + Shift + O`)

**Expand strokes | 扩展描边:**
1. Select object (选择对象)
2. Object → Expand (Object → Expand)
3. Check "Stroke" box (勾选"描边"框)

#### Pathfinder Operations | 路径查找器操作

**Open Pathfinder | 打开路径查找器:**
- Window → Pathfinder (Window → Pathfinder)

**Unite | 联合:** Combine shapes (组合形状)
**Minus Front | 前减:** Subtract top shape (减去顶部形状)
**Intersect | 相交:** Keep overlap only (仅保留重叠)
**Exclude | 排除:** Remove overlap (移除重叠)

### Exporting to DXF | 导出为 DXF

**Step-by-step | 分步指南:**

1. **Prepare design | 准备设计:**
   - Select all (`Ctrl + A`)
   - Type → Create Outlines (for any text)
   - Object → Expand (for strokes if needed)

2. **Export | 导出:**
   - File → Export → Export As
   - Format: AutoCAD Drawing (*.DXF)
   - Choose location (选择位置)
   - Click Export (点击导出)

3. **DXF Options | DXF 选项:**
   - Version: AutoCAD 2010 (版本：AutoCAD 2010)
   - Units: Millimeters (单位：毫米)
   - Click OK (点击确定)

---

## 🖨️ Tinkercad Tutorial | Tinkercad 教程

### Getting Started | 入门

#### Creating an Account | 创建账号
1. Go to https://www.tinkercad.com
2. Click "Sign Up" (点击"注册")
3. Use email or Google/Microsoft account (使用电子邮件或 Google/Microsoft 账号)
4. Verify your email (验证电子邮件)

#### Starting a New Design | 开始新设计
1. Click "Create new design" (点击"创建新设计")
2. Name your project (命名项目)
3. You'll see the workplane (you'll see工作平面)

### Interface Overview | 界面概览

- **Workplane** (Grid): Where you build (网格：构建位置)
- **Shapes Panel** (Right): Basic shapes (右侧：基本形状)
- **View Cube** (Top right): Rotate view (右上角：旋转视图)
- **Zoom controls** (Bottom right): Zoom in/out (右下角：放大/缩小)

### Essential Operations | 基本操作

#### 1. Adding Shapes | 添加形状

**How to add | 如何添加:**
1. Click a shape from Shapes panel (从形状面板点击形状)
2. Drag onto workplane (拖到工作平面)
3. Release to place (释放以放置)

**Common shapes | 常见形状:**
- **Box** (盒子): Rectangular solid (矩形实体)
- **Cylinder** (圆柱体): Circular solid (圆形实体)
- **Sphere** (球体): Round solid (圆形实体)
- **Cone** (圆锥体): Tapered solid (锥形实体)

#### 2. Moving Objects | 移动对象

**Method 1: Drag | 方法1：拖动**
- Click and drag shape (点击并拖动形状)
- Stays on workplane (保持在工作平面上)

**Method 2: Arrow Keys | 方法2：箭头键**
- Select shape (选择形状)
- Use arrow keys for precise movement (使用箭头键精确移动)

**Method 3: Height Adjustment | 方法3：高度调整**
- Select shape (选择形状)
- Drag the up-arrow cone (拖动向上箭头锥体)
- Or click and enter height value (或点击并输入高度值)

#### 3. Resizing Shapes | 调整形状大小

**Using handles | 使用手柄:**
1. Select shape (选择形状)
2. Drag white corner handles to resize (拖动白色角手柄调整大小)
3. Hold `Shift` to maintain proportions (按住 `Shift` 保持比例)

**Using dimension boxes | 使用尺寸框:**
1. Select shape (选择形状)
2. Click dimension value (点击尺寸值)
3. Type new value (输入新值)
4. Press `Enter` (按 `Enter`)

#### 4. Rotating Objects | 旋转对象

**Method 1: Rotation arrows | 方法1：旋转箭头**
1. Select shape (选择形状)
2. Drag curved arrows to rotate (拖动弯曲箭头旋转)

**Method 2: Rotation tool | 方法2：旋转工具**
1. Select shape (选择形状)
2. Click rotation values above shape (点击形状上方的旋转值)
3. Enter precise angle (输入精确角度)

#### 5. Group (Combine) | 组合

**Critical for creating solid models! | 对创建实体模型至关重要！**

**How to group | 如何组合:**
1. Select multiple shapes (选择多个形状)
   - Click first shape (点击第一个形状)
   - Hold `Shift` and click others (按住 `Shift` 并点击其他)
2. Click **Group** button (点击**组合**按钮)
   - Or press `Ctrl + G` (或按 `Ctrl + G`)
3. Shapes merge into one solid (形状合并为一个实体)

**Why group? | 为什么组合？**
- Creates manifold (watertight) model (创建流形（水密）模型)
- Required for STL export (STL 导出所需)
- Makes object movable as one unit (使对象作为一个单元移动)

#### 6. Hole (Subtract) | 孔（减去）

**Use for | 用于:** Cutting out shapes from solids (从实体中切出形状)

**How to create holes | 如何创建孔:**
1. Add a shape where you want hole (在需要孔的位置添加形状)
2. Select the shape (选择形状)
3. Click **Hole** button (点击**孔**按钮)
   - Shape turns transparent (形状变透明)
4. Position hole shape inside/through solid (将孔形状定位在实体内部/穿过实体)
5. Select both shapes (选择两个形状)
6. Click **Group** (点击**组合**)
   - Hole is cut out! (孔被切出！)

**Examples | 示例:**
- Cylinder hole through badge (徽章上的圆柱孔)
- Box hole in bracket (支架上的方孔)

#### 7. Align Tool | 对齐工具

**Critical for precise positioning! | 对精确定位至关重要！**

**How to align | 如何对齐:**
1. Select shapes to align (选择要对齐的形状)
2. Click **Align** button (点击**对齐**按钮)
3. Alignment dots appear (出现对齐点)
4. Click dots to align:
   - **Center**: Middle dots (中心：中间点)
   - **Edge**: Side dots (边缘：侧面点)
   - **Top/Bottom**: Vertical dots (顶部/底部：垂直点)

**Common use | 常见用途:**
- Center hole on badge (在徽章上居中孔)
- Align multiple parts (对齐多个部件)
- Stack layers precisely (精确堆叠层)

### Design Workflows | 设计工作流程

#### Example 1: Simple Badge | 示例1：简单徽章

1. Add **Cylinder** (20mm diameter, 3mm height) (添加**圆柱体**（直径 20 毫米，高度 3 毫米）)
2. Add **Text** with your initials (添加带有首字母的**文本**)
3. Resize text to fit (调整文本大小以适应)
4. Raise text height to 4mm (above badge) (将文本高度提高到 4 毫米（徽章上方）)
5. Select text + cylinder (选择文本 + 圆柱体)
6. Click **Group** (点击**组合**)
7. Add small **Cylinder** (2mm) at top for hole (在顶部添加小**圆柱体**（2 毫米）作为孔)
8. Make it a **Hole** (将其设为**孔**)
9. Group all together (全部组合在一起)
10. Export as STL (导出为 STL)

#### Example 2: Phone Stand | 示例2：手机支架

1. Add **Box** (50mm × 30mm × 5mm) - base (添加**盒子**（50 毫米 × 30 毫米 × 5 毫米）- 底座)
2. Add **Wedge** (30mm × 30mm × 40mm) - back support (添加**楔形**（30 毫米 × 30 毫米 × 40 毫米）- 后支撑)
3. Rotate wedge to desired angle (将楔形旋转到所需角度)
4. Position wedge on base (将楔形定位在底座上)
5. Group base + wedge (组合底座 + 楔形)
6. Add **Box** for phone slot (10mm × 30mm × 2mm) (为手机槽添加**盒子**（10 毫米 × 30 毫米 × 2 毫米）)
7. Make it a **Hole** (将其设为**孔**)
8. Position in support (定位在支撑中)
9. Group all (全部组合)
10. Export as STL (导出为 STL)

### Exporting to STL | 导出为 STL

**Step-by-step | 分步指南:**

1. **Verify model | 验证模型:**
   - All shapes are grouped (所有形状都已组合)
   - No floating parts (没有浮动部件)
   - Model sits on workplane (模型位于工作平面上)

2. **Export | 导出:**
   - Click **Export** button (top right) (点击**导出**按钮（右上角）)
   - Select **.STL** format (选择 **.STL** 格式)
   - Click **Export** (点击**导出**)
   - File downloads to your computer (文件下载到计算机)

3. **Get share link (optional) | 获取分享链接（可选）:**
   - Click **Share** button (点击**分享**按钮)
   - Set to "Anyone with the link" (设置为"任何有链接的人")
   - Copy link (复制链接)
   - Save to `tinkercad_link.txt` (保存到 `tinkercad_link.txt`)

4. **Verify STL | 验证 STL:**
   - File size: typically 100 KB - 5 MB (文件大小：通常 100 KB - 5 MB)
   - Can be opened in slicer software (可在切片软件中打开)

---

## ⚠️ Common Mistakes to Avoid | 常见错误避免

### Laser Cutting Mistakes | 激光切割错误

#### ❌ Mistake 1: Text Not Converted to Paths | 文本未转换为路径
**Problem | 问题:** Laser cutter can't read text as fonts (激光切割机无法将文本读取为字体)

**Solution | 解决方案:**
- Always: Text → Path → Object to Path (始终：Text → Path → Object to Path)
- Do this BEFORE exporting DXF (导出 DXF 之前执行此操作)

#### ❌ Mistake 2: Overlapping Lines | 重叠线条
**Problem | 问题:** Laser cuts same path twice, burns material (激光切割相同路径两次，烧材料)

**Solution | 解决方案:**
- Use Path → Union to merge shapes (使用 Path → Union 合并形状)
- Check for duplicate paths (检查重复路径)
- Delete hidden layers (删除隐藏图层)

#### ❌ Mistake 3: Using Raster Images | 使用光栅图像
**Problem | 问题:** Photos/PNG can't be laser cut (照片/PNG 无法激光切割)

**Solution | 解决方案:**
- Use Path → Trace Bitmap (if you must) (使用 Path → Trace Bitmap（如果必须）)
- Or redraw using vector tools (或使用矢量工具重绘)
- Keep it simple! (保持简单！)

#### ❌ Mistake 4: Details Too Small | 细节太小
**Problem | 问题:** Features < 1mm break or burn (< 1 毫米的特征会断裂或燃烧)

**Solution | 解决方案:**
- Simplify design (简化设计)
- Make text larger (5mm+ height) (使文本更大（高度 5 毫米+）)
- Increase gap between elements (增加元素之间的间隙)

### 3D Printing Mistakes | 3D 打印错误

#### ❌ Mistake 1: Walls Too Thin | 壁太薄
**Problem | 问题:** Walls < 1.2mm fail to print or are fragile (< 1.2 毫米的壁无法打印或很脆)

**Solution | 解决方案:**
- Check all dimensions (检查所有尺寸)
- Make walls 2–3mm for strength (将壁做成 2–3 毫米以获得强度)
- Test by measuring in Tinkercad (在 Tinkercad 中测量测试)

#### ❌ Mistake 2: Overhangs Too Steep | 悬垂太陡
**Problem | 问题:** Angles > 45° sag or need supports (> 45° 的角度下垂或需要支撑)

**Solution | 解决方案:**
- Keep overhangs ≤ 45° (保持悬垂 ≤ 45°)
- Add chamfers/fillets (添加倒角/圆角)
- Rotate model for better orientation (旋转模型以获得更好的方向)

#### ❌ Mistake 3: Not Grouped | 未组合
**Problem | 问题:** Ungrouped shapes export as multiple objects (未组合的形状导出为多个对象)

**Solution | 解决方案:**
- Select all shapes (选择所有形状)
- Click **Group** (点击**组合**)
- Should become single orange object (应该成为单个橙色对象)

#### ❌ Mistake 4: Floating in Air | 浮在空中
**Problem | 问题:** Parts not on workplane won't print properly (不在工作平面上的部件无法正确打印)

**Solution | 解决方案:**
- Drag vertical axis to lower shape (拖动垂直轴降低形状)
- Use **Align** → Bottom to workplane (使用**对齐** → 底部到工作平面)
- Check from side view (从侧视图检查)

---

## ✨ Design Best Practices | 设计最佳实践

### General Tips | 一般提示

#### 1. Start Simple | 从简单开始
- First design should be basic (第一个设计应该基础)
- Master fundamentals before details (在细节之前掌握基础)
- Complex designs come with practice (复杂设计来自练习)

#### 2. Measure Everything | 测量一切
- Use rulers in software (在软件中使用尺子)
- Check dimensions often (经常检查尺寸)
- Remember: 10mm = 1cm (记住：10 毫米 = 1 厘米)

#### 3. Test Before Fabricating | 制造前测试
- Check all design rules (检查所有设计规则)
- Verify file exports correctly (验证文件正确导出)
- Ask for peer review (要求同行审查)

#### 4. Document Your Process | 记录过程
- Take screenshots at each step (每步截图)
- Write down decisions (写下决定)
- Note problems and solutions (记录问题和解决方案)

### Laser Cutting Best Practices | 激光切割最佳实践

#### Design for Assembly | 为组装设计
- **Kerf compensation**: Add 0.2mm to holes (间隙补偿：在孔中添加 0.2 毫米)
- **Snap-fit tabs**: Make 0.2mm smaller (卡扣榫：缩小 0.2 毫米)
- **Test fit**: Do a cardboard prototype first (试装：先做纸板原型)

#### Optimize Material Use | 优化材料使用
- Nest parts efficiently (高效嵌套部件)
- Minimize waste (最小化浪费)
- Consider material grain direction (考虑材料纹理方向)

#### Add Registration Marks | 添加定位标记
- Small circles/crosses for alignment (用于对齐的小圆圈/十字)
- Help with multi-layer designs (帮助多层设计)

### 3D Printing Best Practices | 3D 打印最佳实践

#### Design for Orientation | 为方向设计
- Think about which side prints first (考虑哪一侧先打印)
- Flat side down = better adhesion (平面朝下 = 更好的附着)
- Minimize overhangs (最小化悬垂)

#### Add Chamfers | 添加倒角
- Bottom edges: 45° chamfer (底边：45° 倒角)
- Improves first layer (改善第一层)
- Reduces warping (减少翘曲)

#### Hollow Large Volumes | 挖空大体积
- Save material and time (节省材料和时间)
- Faster printing (更快打印)
- Use shell thickness 2–3mm (使用壳厚 2–3 毫米)

#### Add Drainage Holes | 添加排水孔
- For hollow objects (对于空心对象)
- Prevents air pressure issues (防止气压问题)
- Small 2mm hole is enough (2 毫米小孔就够了)

---

## 📏 Measurement Reference | 测量参考

### Size Guidelines | 尺寸指南

| Feature | Minimum | Recommended | 说明 |
|---------|---------|-------------|-----|
| Laser line width | 0.01 mm | 0.05 mm | 切割线宽 |
| Laser feature size | 1 mm | 2 mm | 最小特征 |
| Laser gap spacing | 1 mm | 2 mm | 间隙间距 |
| Laser text height | 3 mm | 5 mm | 文字高度 |
| 3D wall thickness | 1.2 mm | 2–3 mm | 壁厚 |
| 3D overhang angle | 45° | < 45° | 悬垂角度 |
| 3D hole diameter | 2 mm | 3 mm | 孔直径 |
| 3D feature height | 0.4 mm | 1 mm | 特征高度 |

### Unit Conversions | 单位转换

- **1 cm = 10 mm** (1 厘米 = 10 毫米)
- **1 inch = 25.4 mm** (1 英寸 = 25.4 毫米)
- **1 mm = 0.1 cm** (1 毫米 = 0.1 厘米)

---

## 🎯 Quick Reference Checklist | 快速参考检查清单

### Before Exporting Laser Cut Design | 导出激光切割设计前
- [ ] All text converted to paths (所有文本已转换为路径)
- [ ] Stroke width is 0.01–0.05 mm (描边宽度为 0.01–0.05 毫米)
- [ ] All paths are closed (所有路径都已闭合)
- [ ] No overlapping lines (无重叠线条)
- [ ] Minimum feature size ≥ 1 mm (最小特征尺寸 ≥ 1 毫米)
- [ ] Design size is 4–15 cm (设计尺寸为 4–15 厘米)

### Before Exporting 3D Model | 导出 3D 模型前
- [ ] All shapes are grouped (所有形状都已组合)
- [ ] Wall thickness ≥ 1.2 mm (壁厚 ≥ 1.2 毫米)
- [ ] No overhangs > 45° (无 > 45° 的悬垂)
- [ ] Model sits flat on workplane (模型平放在工作平面上)
- [ ] Size ≤ 50 mm (尺寸 ≤ 50 毫米)
- [ ] No floating parts (无浮动部件)

---

## 💬 Need More Help? | 需要更多帮助？

### In-Class Resources | 课堂资源
- 🙋 Ask your instructor or TAs (询问讲师或助教)
- 👥 Collaborate with classmates (与同学合作)
- 📖 Refer back to this guide (参考本指南)

### Online Resources | 在线资源
- 🎓 [Inkscape Tutorials](https://inkscape.org/learn/) (Inkscape 教程)
- 🎓 [Tinkercad Lessons](https://www.tinkercad.com/learn) (Tinkercad 课程)
- 📺 YouTube: Search "laser cutting design" or "Tinkercad tutorial" (YouTube：搜索"laser cutting design"或"Tinkercad tutorial")

---

**Good luck with your designs! Remember: simple, clean, and manufacturable! 🎨🔧**

**祝设计顺利！记住：简单、干净、可制造！🎨🔧**


