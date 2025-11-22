# Submission Requirements | 提交要求

## 📤 How to Submit Your Mechanical Assignment | 如何提交机械作业

After completing your laser cutting design and 3D printing model, you need to submit your work properly organized.

完成激光切割设计和 3D 打印模型后，你需要正确组织并提交作品。

---

## 📁 Required Folder Structure | 必需的文件夹结构

Your submission **MUST** follow this exact structure:

你的提交**必须**遵循以下确切结构：

```
YourName_MakerAssignment/
│
├── submission.json                    ← Your submission info | 提交信息
│
├── A_LaserCut/                       ← Task A files | 任务 A 文件
│   ├── design_source.ai OR .svg      ← Source design | 源设计
│   ├── final_export.dxf              ← DXF for cutting | 切割用 DXF
│   ├── README_LaserCut.md            ← Documentation | 文档
│   └── photos/                       ← Process photos | 过程照片
│       ├── design_screenshot.png
│       └── detail_view.jpg
│
└── B_3DModel/                        ← Task B files | 任务 B 文件
    ├── model.stl                     ← 3D model | 3D 模型
    ├── README_3DPrint.md             ← Documentation | 文档
    ├── tinkercad_link.txt (optional) ← Tinkercad link | Tinkercad 链接
    └── photos/                       ← Screenshots | 截图
        ├── front_view.png
        └── side_view.png
```

**⚠️ IMPORTANT | 重要:**
- Folder names are case-sensitive! (文件夹名称区分大小写！)
- Use exact names: `A_LaserCut` and `B_3DModel` (使用确切名称)
- Each task must have its own folder (每个任务必须有自己的文件夹)

---

## 📝 Task A: Laser Cutting Submission | 任务 A：激光切割提交

### Required Files | 必需文件

#### 1. Design Source File | 设计源文件
**File name | 文件名:** `design_source.ai` OR `design_source.svg`

**Requirements | 要求:**
- Format: Adobe Illustrator (.ai) OR Inkscape (.svg) (格式)
- Must be editable source file (必须是可编辑源文件)
- NOT a screenshot or PDF (不是截图或 PDF)
- Contains original design with layers (包含原始设计及图层)

**Why needed | 为什么需要:**
Source files allow instructors to verify your design process and provide feedback.

源文件允许讲师验证你的设计过程并提供反馈。

#### 2. DXF Export File | DXF 导出文件
**File name | 文件名:** `final_export.dxf`

**Requirements | 要求:**
- Format: DXF (AutoCAD Drawing Exchange Format)
- All text converted to paths (所有文本已转换为路径)
- Stroke width: 0.01–0.05 mm (描边宽度：0.01–0.05 毫米)
- All paths are closed (所有路径都已闭合)
- No raster images (无光栅图像)

**Technical specifications | 技术规格:**
```
✅ Vector paths only (仅矢量路径)
✅ Closed shapes (闭合形状)
✅ Line width 0.01–0.05 mm (线宽)
✅ Size: 4–15 cm (尺寸)
✅ Minimum feature: ≥ 1 mm (最小特征)
```

#### 3. README_LaserCut.md | 激光切割文档
**File name | 文件名:** `README_LaserCut.md` (exact name!) (确切名称！)

**Required sections | 必需部分:**

```markdown
# Laser Cutting Assignment (DXF)

## 1. My Design | 我的设计

- **Project Type | 项目类型**: [Keychain/Sign/Snap-fit]
- **Design Theme | 设计主题**: [Describe your concept]
- **Dimensions | 尺寸**: [Length × Width in cm/mm]

## 2. Design Process | 制作步骤

Describe how you created your design (3-5 steps):

描述你如何创建设计（3-5 步）：

1. [Step 1]
2. [Step 2]
3. [Step 3]

## 3. Design Concept | 设计概念

Explain your design inspiration and choices:

解释你的设计灵感和选择：

[Write 2-3 sentences about your design thinking]

## 4. Technical Checklist | 技术检查清单

- [ ] All lines are vector paths (所有线条都是矢量路径)
- [ ] Line width is 0.01–0.05 mm (线宽为 0.01–0.05 毫米)
- [ ] All shapes are closed (所有形状都已闭合)
- [ ] Minimum details > 1 mm (最小细节 > 1 毫米)
- [ ] Text converted to paths (文本已转换为路径)
- [ ] File exported as DXF (文件导出为 DXF)

## 5. Files Included | 文件说明

- **Source file**: `design_source.[ai/svg]` - Original design
- **Export file**: `final_export.dxf` - Ready for laser cutting
- **Photos**: [List photo files]
```

**Content requirements | 内容要求:**
- Write in complete sentences (用完整句子写)
- Be specific about your design decisions (具体说明设计决策)
- Minimum 100 words total (总共至少 100 字)
- Include both English and Chinese (or at least one) (包含中英文（或至少一种）)

#### 4. Photos | 照片
**Folder | 文件夹:** `A_LaserCut/photos/` (or directly in A_LaserCut/) (或直接在 A_LaserCut/ 中)

**Minimum required | 最少要求:** 2 photos (2 张照片)

**Photo requirements | 照片要求:**

**Photo 1: Design Screenshot | 设计截图**
- Screenshot of your design in Inkscape/Illustrator (Inkscape/Illustrator 中的设计截图)
- Show the full workspace (显示完整工作区)
- Must be clearly visible (必须清晰可见)

**Photo 2: Detail View | 细节视图**
- Close-up showing design details (显示设计细节的特写)
- OR planning sketch (或规划草图)
- OR different angle/view (或不同角度/视图)

**Technical specs | 技术规格:**
- Format: `.jpg`, `.jpeg`, `.png`, `.heic`, `.webp`
- Resolution: Minimum 800×600 pixels (分辨率：最小 800×600 像素)
- File size: < 5 MB per photo (文件大小：每张 < 5 MB)
- Clear and in focus (清晰且对焦)

**Optional photos | 可选照片:**
- Sketch/planning drawings (草图/规划图)
- Design iterations (设计迭代)
- Measurement verification (测量验证)

---

## 🖨️ Task B: 3D Printing Submission | 任务 B：3D 打印提交

### Required Files | 必需文件

#### 1. STL Model File | STL 模型文件
**File name | 文件名:** `model.stl`

**Requirements | 要求:**
- Format: STL (Standard Tessellation Language)
- Exported from Tinkercad (从 Tinkercad 导出)
- Model is a closed solid (manifold) (模型是封闭实体（流形）)
- Proper orientation (sits flat) (正确方向（平放）)

**Technical specifications | 技术规格:**
```
✅ Closed/watertight mesh (封闭/水密网格)
✅ Wall thickness ≥ 1.2 mm (壁厚)
✅ No overhangs > 45° (无悬垂 > 45°)
✅ Maximum size ≤ 50 mm (最大尺寸)
✅ File size: 100 KB – 10 MB (文件大小)
```

**File size guidance | 文件大小指导:**
- Too small (< 10 KB): Likely too simple or corrupted (可能太简单或损坏)
- Normal (100 KB – 5 MB): Good range (良好范围)
- Too large (> 10 MB): Model might be too complex (模型可能太复杂)

#### 2. README_3DPrint.md | 3D 打印文档
**File name | 文件名:** `README_3DPrint.md` (exact name!) (确切名称！)

**Required sections | 必需部分:**

```markdown
# 3D Printing Assignment (STL)

## 1. My Model | 我的模型

- **Model Type | 模型类型**: [Badge/Accessory/Phone Stand]
- **Model Dimensions | 模型尺寸**: [X × Y × Z in mm]
- **Minimum Wall Thickness | 最小壁厚**: [X mm]

## 2. Design Concept | 设计概念

Explain your design idea and purpose:

解释你的设计想法和目的：

[Write 2-3 sentences about what you created and why]

## 3. Modeling Steps | 建模步骤

Describe how you built your model in Tinkercad (3-5 steps):

描述你如何在 Tinkercad 中构建模型（3-5 步）：

1. [Step 1: e.g., "Started with a cylinder 20mm diameter"]
2. [Step 2]
3. [Step 3]

## 4. Printability Checklist | 可打印性检查清单

- [ ] Model is a closed solid (模型是封闭实体)
- [ ] Wall thickness ≥ 1.2 mm (壁厚 ≥ 1.2 毫米)
- [ ] No overhangs > 45° (无悬垂 > 45°)
- [ ] Model sits flat on workplane (模型平放在工作平面上)
- [ ] Size ≤ 50 mm (尺寸 ≤ 50 毫米)
- [ ] All shapes grouped (所有形状已组合)
- [ ] Exported as STL (导出为 STL)

## 5. Files Included | 文件说明

- **Model file**: `model.stl` - 3D printable model
- **Tinkercad link**: [Your share link] (optional)
- **Photos**: [List photo files]
```

**Content requirements | 内容要求:**
- Write in complete sentences (用完整句子写)
- Explain your modeling choices (解释建模选择)
- Minimum 100 words total (总共至少 100 字)
- Include both English and Chinese (or at least one) (包含中英文（或至少一种）)

#### 3. Tinkercad Link (Optional) | Tinkercad 链接（可选）
**File name | 文件名:** `tinkercad_link.txt`

**Content | 内容:**
```
https://www.tinkercad.com/things/YOUR-DESIGN-ID
```

**How to get your link | 如何获取链接:**
1. In Tinkercad, click "Share" button (在 Tinkercad 中，点击"分享"按钮)
2. Set to "Anyone with the link" (设置为"任何有链接的人")
3. Copy the link (复制链接)
4. Paste into `tinkercad_link.txt` (粘贴到 `tinkercad_link.txt`)

**Why optional | 为什么可选:**
- STL file is sufficient for grading (STL 文件足以评分)
- Link allows instructor to see your design process (链接允许讲师查看设计过程)
- **+1 bonus point** for including link (**+1 加分**如果包含链接)

#### 4. Photos/Screenshots | 照片/截图
**Folder | 文件夹:** `B_3DModel/photos/` (or directly in B_3DModel/) (或直接在 B_3DModel/ 中)

**Minimum required | 最少要求:** 2 screenshots (2 张截图)

**Photo requirements | 照片要求:**

**Photo 1: Front/Main View | 正面/主视图**
- Screenshot from Tinkercad showing your model (Tinkercad 中显示模型的截图)
- Clear view of the design (设计的清晰视图)
- Include workplane for reference (包含工作平面以供参考)

**Photo 2: Angle/Side View | 角度/侧视图**
- Different angle showing depth/thickness (显示深度/厚度的不同角度)
- OR top/bottom view (或顶部/底部视图)
- Helps show 3D structure (帮助显示 3D 结构)

**Technical specs | 技术规格:**
- Format: `.jpg`, `.jpeg`, `.png`, `.heic`, `.webp`
- Resolution: Minimum 800×600 pixels (分辨率：最小 800×600 像素)
- File size: < 5 MB per photo (文件大小：每张 < 5 MB)
- Clear and in focus (清晰且对焦)

**Optional screenshots | 可选截图:**
- Dimension annotations (尺寸标注)
- Design iterations (设计迭代)
- Multiple angles (多角度)

---

## 📋 submission.json | 提交信息

**File location | 文件位置:** Root directory (根目录)

**Required format | 必需格式:**

```json
{
  "student_name": "Your Full Name",
  "laser_cut_project_type": "keychain",
  "3d_model_project_type": "badge",
  "completion_date": "2024-11-22",
  "notes": "Optional notes about your work"
}
```

**Field descriptions | 字段说明:**

| Field | Description | Example |
|-------|-------------|---------|
| `student_name` | Your full name (你的全名) | "张三 (Zhang San)" |
| `laser_cut_project_type` | Type of laser project (激光项目类型) | "keychain", "sign", or "snap-fit" |
| `3d_model_project_type` | Type of 3D model (3D 模型类型) | "badge", "accessory", or "phone-stand" |
| `completion_date` | Submission date (提交日期) | "2024-11-22" |
| `notes` | Optional comments (可选评论) | Any additional information |

**Common mistakes | 常见错误:**
- ❌ Leaving "Your Name" as placeholder (将"Your Name"留作占位符)
- ❌ Invalid JSON syntax (JSON 语法无效)
- ❌ Missing required fields (缺少必需字段)

---

## ✅ Pre-Submission Checklist | 提交前检查清单

Before submitting, verify ALL of these:

提交前，验证所有这些：

### Folder Structure | 文件夹结构
- [ ] `submission.json` in root directory (根目录中的 `submission.json`)
- [ ] `A_LaserCut/` folder exists (文件夹存在)
- [ ] `B_3DModel/` folder exists (文件夹存在)
- [ ] Folder names are exactly correct (文件夹名称完全正确)

### Task A Files | 任务 A 文件
- [ ] Source file (.ai OR .svg) included (包含源文件)
- [ ] DXF export file included (包含 DXF 导出文件)
- [ ] README_LaserCut.md is complete (README_LaserCut.md 已完成)
- [ ] At least 2 photos included (至少包含 2 张照片)
- [ ] All design rules followed (遵循所有设计规则)

### Task B Files | 任务 B 文件
- [ ] model.stl file included (包含 model.stl 文件)
- [ ] README_3DPrint.md is complete (README_3DPrint.md 已完成)
- [ ] At least 2 screenshots included (至少包含 2 张截图)
- [ ] All printability rules followed (遵循所有可打印性规则)
- [ ] (Optional) tinkercad_link.txt included (（可选）包含 tinkercad_link.txt)

### Content Quality | 内容质量
- [ ] READMEs have meaningful content (README 有有意义的内容)
- [ ] Photos are clear and relevant (照片清晰相关)
- [ ] Technical specifications met (满足技术规格)
- [ ] All checklists completed (所有检查清单已完成)

### Git Submission | Git 提交
- [ ] All files added to Git (`git add .`) (所有文件已添加到 Git)
- [ ] Changes committed (`git commit`) (更改已提交)
- [ ] Pushed to GitHub (`git push`) (已推送到 GitHub)
- [ ] GitHub Actions validation passed (GitHub Actions 验证通过)

---

## 🚫 Common Submission Mistakes | 常见提交错误

### ❌ Wrong Folder Names | 错误的文件夹名称

**Wrong | 错误:**
```
LaserCut/          (missing "A_")
laser-cut/         (wrong capitalization)
A-LaserCut/        (hyphen instead of underscore)
3DModel/           (missing "B_")
```

**Correct | 正确:**
```
A_LaserCut/
B_3DModel/
```

### ❌ Wrong File Extensions | 错误的文件扩展名

**Wrong | 错误:**
- `design.pdf` (not editable source) (非可编辑源文件)
- `export.svg` (should be .dxf for laser) (激光应为 .dxf)
- `model.obj` (should be .stl for printing) (打印应为 .stl)

**Correct | 正确:**
- `design_source.ai` or `.svg`
- `final_export.dxf`
- `model.stl`

### ❌ Missing README Files | 缺少 README 文件

**Wrong | 错误:**
- `readme.md` (wrong capitalization) (大小写错误)
- `README.md` (missing specific name) (缺少特定名称)
- `LaserCut_README.md` (wrong format) (格式错误)

**Correct | 正确:**
- `README_LaserCut.md` (exact name!) (确切名称！)
- `README_3DPrint.md` (exact name!) (确切名称！)

### ❌ Incomplete Documentation | 文档不完整

**Wrong | 错误:**
- Single sentence descriptions (单句描述)
- Missing technical checklist (缺少技术检查清单)
- No design process explanation (无设计过程说明)
- Template text not filled in (模板文本未填写)

**Correct | 正确:**
- Complete paragraphs (完整段落)
- All checklists filled out (所有检查清单已填写)
- Detailed process steps (详细过程步骤)
- Original content (原创内容)

### ❌ Poor Photo Quality | 照片质量差

**Wrong | 错误:**
- Blurry screenshots (模糊截图)
- Photos of screen (instead of screenshots) (屏幕照片（而非截图）)
- Files over 5 MB (文件超过 5 MB)
- No photos at all (完全没有照片)

**Correct | 正确:**
- Clear screenshots (清晰截图)
- Multiple angles (多角度)
- Reasonable file sizes (合理文件大小)
- Minimum 2 photos per task (每个任务至少 2 张照片)

---

## 🔧 File Size Guidelines | 文件大小指南

### Expected File Sizes | 预期文件大小

| File Type | Typical Size | Warning If | 文件类型 |
|-----------|--------------|------------|---------|
| .ai source | 100 KB – 5 MB | < 50 KB or > 20 MB | AI 源文件 |
| .svg source | 10 KB – 500 KB | < 5 KB or > 2 MB | SVG 源文件 |
| .dxf export | 10 KB – 500 KB | < 5 KB (might be empty) | DXF 导出 |
| .stl model | 100 KB – 5 MB | < 10 KB or > 10 MB | STL 模型 |
| Photos | 100 KB – 2 MB | > 5 MB (too large) | 照片 |

**If files are too small | 如果文件太小:**
- File might be corrupted (文件可能已损坏)
- Design might be too simple (设计可能太简单)
- Export might have failed (导出可能失败)

**If files are too large | 如果文件太大:**
- Compress photos (压缩照片)
- Simplify complex designs (简化复杂设计)
- Check for embedded images (检查嵌入图像)

---

## 📚 Additional Resources | 其他资源

**For detailed help, see | 详细帮助见:**
- [HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md) - Step-by-step submission guide (分步提交指南)
- [DESIGN-GUIDE.md](./DESIGN-GUIDE.md) - Design rules and tutorials (设计规则和教程)
- [README.md](./README.md) - Full assignment instructions (完整作业说明)
- [rubric.md](./rubric.md) - Grading criteria (评分标准)

---

## ❓ FAQ | 常见问题

<details>
<summary><strong>Q: Can I submit both tasks in one folder? | 可以在一个文件夹中提交两个任务吗？</strong></summary>

**A**: **NO!** You must use separate folders: `A_LaserCut/` and `B_3DModel/`

**答**: **不可以！**你必须使用单独的文件夹：`A_LaserCut/` 和 `B_3DModel/`
</details>

<details>
<summary><strong>Q: What if I made multiple versions? | 如果我做了多个版本怎么办？</strong></summary>

**A**: Submit your final/best version. You can mention iterations in your README.

**答**: 提交最终/最佳版本。你可以在 README 中提及迭代。
</details>

<details>
<summary><strong>Q: Can I use different file names? | 可以使用不同的文件名吗？</strong></summary>

**A**: The README files must be exactly `README_LaserCut.md` and `README_3DPrint.md`. Other files can have descriptive names.

**答**: README 文件必须完全是 `README_LaserCut.md` 和 `README_3DPrint.md`。其他文件可以有描述性名称。
</details>

<details>
<summary><strong>Q: How many photos do I need? | 我需要多少张照片？</strong></summary>

**A**: Minimum 2 per task (total 4). More is better! Include design process, different angles, details.

**答**: 每个任务至少 2 张（总共 4 张）。越多越好！包括设计过程、不同角度、细节。
</details>

<details>
<summary><strong>Q: My DXF file won't open | 我的 DXF 文件无法打开</strong></summary>

**A**: Make sure you:
1. Converted all text to paths first (先将所有文本转换为路径)
2. Used correct DXF export settings (使用正确的 DXF 导出设置)
3. File is not corrupted (check file size > 0) (文件未损坏（检查文件大小 > 0）)

**答**: 确保你：
1. 先将所有文本转换为路径
2. 使用正确的 DXF 导出设置
3. 文件未损坏（检查文件大小 > 0）
</details>

---

**Ready to submit? Follow [HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md) for step-by-step instructions!**

**准备提交？按照 [HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md) 获取分步说明！**


