# Assignment: Day 2 Afternoon - Laser Cutting + 3D Printing
# 作业：第2天下午 - 激光切割 + 3D 打印

> **📚 This is a GitHub Classroom Assignment**  
> **这是一个 GitHub Classroom 作业**  
>   
> **Students**: Follow this handbook step-by-step to design and fabricate your first maker projects.  
> **学生**：按照本手册逐步操作，设计并制作你的第一个创客项目。

---

## 📋 Assignment Overview | 作业概览

🎯 **Maker Assignment | 激光切割 + 3D 打印**

Welcome to your first digital fabrication challenge! Today you'll learn to design for two essential maker tools: the laser cutter and the 3D printer.

欢迎来到你的第一个数字制造挑战！今天你将学习为两个重要的创客工具设计：激光切割机和 3D 打印机。

**What You'll Create | 你将创建什么：**
- ✅ A laser-cuttable 2D design (DXF file) (可激光切割的 2D 设计（DXF 文件）)
- ✅ A 3D-printable model (STL file) (可 3D 打印的模型（STL 文件）)
- ✅ Complete design documentation (完整的设计文档)
- ✅ Photos of your design process (设计过程的照片)

**Timeline | 时间线：**
- ⏰ **Total Duration** | **总时长**: 3–4 hours (3–4 小时)
- ⏰ **Task A (90 min)** | **任务 A（90分钟）**: Laser Cutting Design (激光切割设计)
- ⏰ **Task B (90 min)** | **任务 B（90分钟）**: 3D Printing Model (3D 打印模型)
- ⏰ **Documentation (30 min)** | **文档（30分钟）**: Photos & README files (照片和 README 文件)

---

## 🎯 Learning Objectives | 学习目标

By completing this assignment, you will:

完成此作业后，你将：

- ✅ Understand design constraints for laser cutting (理解激光切割的设计约束)
- ✅ Learn to create manufacturable 3D models (学习创建可制造的 3D 模型)
- ✅ Master vector design tools (掌握矢量设计工具)
- ✅ Use parametric 3D modeling software (使用参数化 3D 建模软件)
- ✅ Document your design process professionally (专业地记录设计过程)
- ✅ Prepare files for digital fabrication (准备数字制造文件)

---

## 📦 What to Submit | 提交内容

You need to submit your work organized in this folder structure:

你需要按以下文件夹结构组织并提交作品：

```
StudentName_MakerAssignment/
│
├── submission.json                    (Your submission info | 提交信息)
│
├── A_LaserCut/                       (Task A: Laser Cutting | 任务 A：激光切割)
│   ├── design_source.ai OR .svg      (Source file | 源文件)
│   ├── final_export.dxf              (Export for cutting | 切割导出文件)
│   ├── README_LaserCut.md            (Design documentation | 设计文档)
│   └── photos/                       (Design process photos | 设计过程照片)
│       ├── photo1.jpg/png
│       └── photo2.jpg/png
│
└── B_3DModel/                        (Task B: 3D Printing | 任务 B：3D 打印)
    ├── model.stl                     (3D model file | 3D 模型文件)
    ├── README_3DPrint.md             (Model documentation | 模型文档)
    ├── tinkercad_link.txt (optional) (Tinkercad link | Tinkercad 链接)
    └── photos/                       (Design screenshots | 设计截图)
        ├── photo1.jpg/png
        └── photo2.jpg/png
```

**See [SUBMISSION.md](./SUBMISSION.md) for detailed submission instructions.**

**详细提交说明见 [SUBMISSION.md](./SUBMISSION.md)。**

---

## ✅ Prerequisites | 前置要求

Before starting, make sure you have:

开始之前，确保你有：

- [ ] A computer with internet access (有互联网访问的计算机)
- [ ] Vector design software installed (已安装矢量设计软件)
  - **Inkscape** (Free, recommended for beginners) (免费，推荐初学者)
  - **Adobe Illustrator** (If you have access) (如果你有访问权限)
- [ ] Access to **Tinkercad** (https://www.tinkercad.com) (访问 Tinkercad)
  - Create a free account if needed (如需要创建免费账号)
- [ ] Basic understanding of design concepts (基本的设计概念理解)
- [ ] A GitHub account for submission (用于提交的 GitHub 账号)

**🆘 Need help installing software? Ask your instructor!**

**🆘 需要安装软件的帮助？询问你的讲师！**

---

## 🎨 Task A: Laser Cutting Design (90 minutes)
## 🎨 任务 A：激光切割设计（90分钟）

### 📌 Choose Your Project Type | 选择项目类型

Select **ONE** of the following project types:

选择以下项目类型之**一**：

#### Option 1: Personalized Keychain | 个性化钥匙扣
- Design a keychain with your name or initials (设计带有你名字或首字母的钥匙扣)
- Size: 4–8 cm (尺寸：4–8 厘米)
- Must include a hole for keyring (必须包含钥匙圈孔)
- **Best for**: Beginners (最适合：初学者)

#### Option 2: Standing Sign/Logo | 立式标牌/Logo
- Create a freestanding sign or logo (创建独立站立的标牌或 Logo)
- Size: 5–10 cm (尺寸：5–10 厘米)
- Must be self-supporting (必须能自我支撑)
- **Best for**: Intermediate (最适合：中级)

#### Option 3: Snap-Fit Assembly | 拼插结构
- Design 2+ pieces that fit together (设计 2+ 个可以拼插在一起的部件)
- Size: Total assembled size 8–12 cm (尺寸：组装后总尺寸 8–12 厘米)
- Must demonstrate interlocking joints (必须展示联锁接头)
- **Best for**: Advanced (最适合：高级)

### 🔧 Technical Requirements | 技术要求

Your design **MUST** meet these specifications:

你的设计**必须**满足这些规格：

✅ **File Format | 文件格式:**
- Source file: `.ai` (Illustrator) OR `.svg` (Inkscape)
- Export file: `.dxf` (for laser cutter)

✅ **Design Rules | 设计规则:**
- All lines must be **vector paths** (所有线条必须是**矢量路径**)
- Line width: **0.01–0.05 mm** (cutting lines) (线宽：**0.01–0.05 毫米**（切割线）)
- All shapes must be **closed paths** (所有形状必须是**闭合路径**)
- Minimum feature size: **≥ 1 mm** (最小特征尺寸：**≥ 1 毫米**)
- No overlapping lines (无重叠线条)

✅ **Size Constraints | 尺寸约束:**
- Minimum size: 4 cm (最小尺寸：4 厘米)
- Maximum size: 15 cm (最大尺寸：15 厘米)
- Recommended: 5–10 cm for best results (推荐：5–10 厘米以获得最佳效果)

### 📚 Step-by-Step Guide | 分步指南

**See [DESIGN-GUIDE.md](./DESIGN-GUIDE.md) for detailed design tutorials!**

**详细设计教程见 [DESIGN-GUIDE.md](./DESIGN-GUIDE.md)！**

#### Quick Steps | 快速步骤:

1. **Sketch your idea** on paper first (先在纸上画草图)
2. **Open Inkscape/Illustrator** and create a new document (打开 Inkscape/Illustrator 并创建新文档)
3. **Design your shape** using vector tools (使用矢量工具设计形状)
4. **Convert text to paths** (if using text) (将文本转换为路径（如果使用文本）)
5. **Set stroke width** to 0.01–0.05 mm (将描边宽度设置为 0.01–0.05 毫米)
6. **Check all paths are closed** (检查所有路径都已闭合)
7. **Export as DXF** (导出为 DXF)
8. **Save source file** (.ai or .svg) (保存源文件（.ai 或 .svg）)

⏱️ **Expected time**: 60–90 minutes (预计时间：60–90 分钟)

---

## 🖨️ Task B: 3D Printing Model (90 minutes)
## 🖨️ 任务 B：3D 打印模型（90分钟）

### 📌 Choose Your Project Type | 选择项目类型

Select **ONE** of the following project types:

选择以下项目类型之**一**：

#### Option 1: Badge/Pin | 徽章/胸针
- Design a wearable badge or pin (设计可穿戴的徽章或胸针)
- Size: 3–5 cm diameter (尺寸：直径 3–5 厘米)
- Thickness: 2–4 mm (厚度：2–4 毫米)
- **Best for**: Beginners (最适合：初学者)

#### Option 2: Accessory/Charm | 配件/挂件
- Create a small accessory or charm (创建小配件或挂件)
- Size: 2–5 cm (尺寸：2–5 厘米)
- Must include attachment point (必须包含附着点)
- **Best for**: Intermediate (最适合：中级)

#### Option 3: Mini Phone Stand | 迷你手机支架
- Design a functional phone stand (设计功能性手机支架)
- Must support a phone at an angle (必须以一定角度支撑手机)
- Size: 5–8 cm (尺寸：5–8 厘米)
- **Best for**: Advanced (最适合：高级)

### 🔧 Technical Requirements | 技术要求

Your model **MUST** meet these specifications:

你的模型**必须**满足这些规格：

✅ **File Format | 文件格式:**
- Export file: `.stl` (standard for 3D printing)

✅ **Design Rules | 设计规则:**
- Model must be a **closed solid** (manifold) (模型必须是**封闭实体**（流形）)
- Minimum wall thickness: **≥ 1.2 mm** (最小壁厚：**≥ 1.2 毫米**)
- Maximum overhang angle: **≤ 45°** (最大悬垂角度：**≤ 45°**)
- Avoid thin/fragile features (避免薄/脆弱的特征)

✅ **Size Constraints | 尺寸约束:**
- Maximum size: 50 mm (any dimension) (最大尺寸：50 毫米（任何维度）)
- Recommended: 20–40 mm (推荐：20–40 毫米)
- Print time should be < 2 hours (打印时间应 < 2 小时)

### 📚 Step-by-Step Guide | 分步指南

**See [DESIGN-GUIDE.md](./DESIGN-GUIDE.md) for detailed Tinkercad tutorials!**

**详细 Tinkercad 教程见 [DESIGN-GUIDE.md](./DESIGN-GUIDE.md)！**

#### Quick Steps | 快速步骤:

1. **Sign in to Tinkercad** (https://www.tinkercad.com) (登录 Tinkercad)
2. **Create a new 3D design** (创建新的 3D 设计)
3. **Build your model** using basic shapes (使用基本形状构建模型)
4. **Use Group/Hole** to combine/subtract shapes (使用组合/孔来组合/减去形状)
5. **Check minimum thickness** (≥1.2 mm) (检查最小厚度（≥1.2 毫米）)
6. **Align and scale** your design (对齐和缩放设计)
7. **Export as STL** (导出为 STL)
8. **Share Tinkercad link** (optional but recommended) (分享 Tinkercad 链接（可选但推荐）)

⏱️ **Expected time**: 60–90 minutes (预计时间：60–90 分钟)

---

## 📸 Documentation Requirements | 文档要求

For **BOTH** tasks, you must create documentation:

对于**两个**任务，你必须创建文档：

### README Files | README 文件

#### README_LaserCut.md (Task A)
Must include:
- Project type (钥匙扣/立牌/拼插结构)
- Design concept and inspiration (设计概念和灵感)
- Design dimensions (L × W) (设计尺寸（长 × 宽）)
- Design process description (设计过程描述)
- Technical checklist (技术检查清单)
- File list (文件列表)

#### README_3DPrint.md (Task B)
Must include:
- Model type (徽章/配件/支架)
- Design concept and inspiration (设计概念和灵感)
- Model dimensions (X × Y × Z) (模型尺寸（X × Y × Z）)
- Modeling steps description (建模步骤描述)
- Printability checklist (可打印性检查清单)
- File list (文件列表)

**Templates are provided in [SUBMISSION.md](./SUBMISSION.md)**

**模板在 [SUBMISSION.md](./SUBMISSION.md) 中提供**

### Photos | 照片

#### Required Photos | 必需照片:

**For Laser Cut Design | 激光切割设计:**
- Screenshot of design in Inkscape/Illustrator (Inkscape/Illustrator 中的设计截图)
- Close-up showing design details (显示设计细节的特写)
- (Optional) Sketch or planning drawings (（可选）草图或规划图)

**For 3D Model | 3D 模型:**
- Screenshot of model in Tinkercad (multiple angles) (Tinkercad 中的模型截图（多角度）)
- Front, side, and top views (正面、侧面和顶部视图)
- (Optional) Design iterations (（可选）设计迭代)

#### Photo Requirements | 照片要求:
- Format: `.jpg`, `.jpeg`, `.png`, `.heic`, `.webp`
- Minimum: 2 photos per task (每个任务至少 2 张照片)
- Clear and well-lit (清晰且光线充足)
- File size: < 5 MB each (文件大小：每张 < 5 MB)

---

## 🎁 Bonus Points (up to +10) | 加分项（最多 +10 分）

Go beyond the basics to earn bonus points:

超越基础以获得加分：

### Laser Cutting Bonus | 激光切割加分
- **+3 pts**: Use boolean operations for creative designs (使用布尔运算进行创意设计)
- **+2 pts**: Include "negative space" in design (在设计中包含"负空间")
- **+2 pts**: Multi-layer or assembly design (多层或组装设计)
- **+2 pts**: Add fillets/chamfers for smooth edges (添加圆角/倒角以平滑边缘)

### 3D Printing Bonus | 3D 打印加分
- **+3 pts**: Functional moving parts (功能性可动部件)
- **+2 pts**: Organic/curved surfaces (有机/曲面)
- **+2 pts**: Text or embossed details (文本或浮雕细节)
- **+2 pts**: Support-free design (optimized orientation) (无支撑设计（优化方向）)

### Documentation Bonus | 文档加分
- **+2 pts**: Detailed design process with iterations (详细的设计过程及迭代)
- **+2 pts**: Professional photo documentation (专业照片文档)
- **+1 pt**: Design inspiration sources cited (引用设计灵感来源)

---

## 📤 Submission Instructions | 提交说明

### Step 1: Organize Your Files | 组织文件

Follow the folder structure shown at the top of this README.

遵循本 README 顶部显示的文件夹结构。

### Step 2: Fill submission.json | 填写 submission.json

```json
{
  "student_name": "Your Name",
  "laser_cut_project_type": "keychain/sign/snap-fit",
  "3d_model_project_type": "badge/accessory/phone-stand",
  "completion_date": "2024-11-22",
  "notes": "Optional notes about your submission"
}
```

### Step 3: Commit and Push | 提交并推送

```bash
git add .
git commit -m "Submit Day 2 Afternoon mechanical assignment"
git push origin main
```

### Step 4: Verify Automated Checks | 验证自动检查

1. Go to the **Actions** tab in your repository (访问仓库的 **Actions** 标签)
2. Check that the file validation passes (检查文件验证通过)
3. Review feedback in **Issues** tab (在 **Issues** 标签查看反馈)

**Detailed submission instructions: [HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md)**

**详细提交说明：[HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md)**

---

## 🆘 Troubleshooting | 故障排除

### Common Issues | 常见问题

<details>
<summary><strong>Q: Inkscape won't export to DXF | Inkscape 无法导出为 DXF</strong></summary>

**A**: Make sure all objects are converted to paths first:
1. Select all (Ctrl+A)
2. Path → Object to Path
3. Then try exporting again

**答**: 确保所有对象首先转换为路径：
1. 全选（Ctrl+A）
2. Path → Object to Path
3. 然后再次尝试导出
</details>

<details>
<summary><strong>Q: My STL file is too large | 我的 STL 文件太大</strong></summary>

**A**: Your model might be too detailed. In Tinkercad:
- Reduce the number of shapes
- Simplify complex curves
- Check your model dimensions (should be in mm, not cm)

**答**: 你的模型可能过于详细。在 Tinkercad 中：
- 减少形状数量
- 简化复杂曲线
- 检查模型尺寸（应为毫米，而非厘米）
</details>

<details>
<summary><strong>Q: Lines are too thick in my laser cut design | 激光切割设计中的线条太粗</strong></summary>

**A**: Set stroke width to 0.01–0.05 mm:
- **Inkscape**: Object → Fill and Stroke → Stroke Style
- **Illustrator**: Window → Stroke → Set width

**答**: 将描边宽度设置为 0.01–0.05 毫米：
- **Inkscape**: Object → Fill and Stroke → Stroke Style
- **Illustrator**: Window → Stroke → Set width
</details>

<details>
<summary><strong>Q: Tinkercad says "No internet connection" | Tinkercad 显示"无网络连接"</strong></summary>

**A**: Tinkercad is cloud-based and requires internet:
- Check your internet connection
- Try a different browser
- Clear browser cache
- Make sure you're logged in

**答**: Tinkercad 是基于云的，需要互联网：
- 检查互联网连接
- 尝试不同的浏览器
- 清除浏览器缓存
- 确保已登录
</details>

**More help: [DESIGN-GUIDE.md](./DESIGN-GUIDE.md) has detailed tutorials**

**更多帮助：[DESIGN-GUIDE.md](./DESIGN-GUIDE.md) 有详细教程**

---

## ✅ Completion Checklist | 完成检查清单

Before submitting, verify:

提交前，验证：

### Task A: Laser Cutting | 任务 A：激光切割
- [ ] Design source file (.ai or .svg) is saved (设计源文件（.ai 或 .svg）已保存)
- [ ] DXF export file is created (DXF 导出文件已创建)
- [ ] All lines are vector paths (所有线条都是矢量路径)
- [ ] Line width is 0.01–0.05 mm (线宽为 0.01–0.05 毫米)
- [ ] All shapes are closed (所有形状都已闭合)
- [ ] Size is within 4–15 cm range (尺寸在 4–15 厘米范围内)
- [ ] README_LaserCut.md is complete (README_LaserCut.md 已完成)
- [ ] At least 2 photos included (至少包含 2 张照片)

### Task B: 3D Printing | 任务 B：3D 打印
- [ ] STL file is exported (STL 文件已导出)
- [ ] Model is a closed solid (模型是封闭实体)
- [ ] Wall thickness ≥ 1.2 mm (壁厚 ≥ 1.2 毫米)
- [ ] No overhangs > 45° (无 > 45° 的悬垂)
- [ ] Size is ≤ 50 mm (尺寸 ≤ 50 毫米)
- [ ] README_3DPrint.md is complete (README_3DPrint.md 已完成)
- [ ] At least 2 photos/screenshots included (至少包含 2 张照片/截图)
- [ ] (Optional) Tinkercad link saved (（可选）已保存 Tinkercad 链接)

### Submission | 提交
- [ ] Folders organized correctly (文件夹组织正确)
- [ ] submission.json filled out (submission.json 已填写)
- [ ] All files committed to Git (所有文件已提交到 Git)
- [ ] Pushed to GitHub (已推送到 GitHub)
- [ ] GitHub Actions validation passed (GitHub Actions 验证通过)

---

## 📚 Resources | 资源

### Software Downloads | 软件下载
- 🎨 [Inkscape](https://inkscape.org/release/) - Free vector graphics editor (免费矢量图形编辑器)
- 🖨️ [Tinkercad](https://www.tinkercad.com/) - Free online 3D design tool (免费在线 3D 设计工具)
- 📐 [Fusion 360](https://www.autodesk.com/products/fusion-360/) - Advanced CAD (optional) (高级 CAD（可选）)

### Learning Resources | 学习资源
- 📖 [DESIGN-GUIDE.md](./DESIGN-GUIDE.md) - Complete design tutorials (完整设计教程)
- 📋 [SUBMISSION.md](./SUBMISSION.md) - Submission requirements (提交要求)
- 📊 [rubric.md](./rubric.md) - Grading criteria (评分标准)
- 💡 [Inkscape Tutorials](https://inkscape.org/learn/) - Official tutorials (官方教程)
- 🎓 [Tinkercad Learn](https://www.tinkercad.com/learn) - Guided lessons (指导课程)

### Design Inspiration | 设计灵感
- 🔍 [Thingiverse](https://www.thingiverse.com/) - 3D model repository (3D 模型库)
- 🎨 [Instructables](https://www.instructables.com/craft/) - DIY projects (DIY 项目)
- 📐 [Obrary](https://obrary.com/) - Laser cut designs (激光切割设计)

---

## 🌟 Tips for Success | 成功提示

### Design Tips | 设计提示

1. **Start Simple** (从简单开始)
   - Don't overcomplicate your first design (不要让第一个设计过于复杂)
   - Master the basics before adding details (在添加细节之前掌握基础)

2. **Test Your Dimensions** (测试尺寸)
   - Use a ruler to check your design is the right size (使用尺子检查设计是否为正确尺寸)
   - Remember: 1 cm = 10 mm (记住：1 厘米 = 10 毫米)

3. **Think About Manufacturing** (考虑制造)
   - Can this actually be cut/printed? (这真的可以切割/打印吗？)
   - Are all parts thick enough? (所有部件都足够厚吗？)

4. **Save Often** (经常保存)
   - Save your work every 10-15 minutes (每 10-15 分钟保存一次)
   - Keep backup copies (保留备份副本)

5. **Document As You Go** (边做边记录)
   - Take screenshots during the process (在过程中截图)
   - Write notes about decisions you make (记录你做出的决定)

### Time Management | 时间管理

- ⏰ **Hour 1**: Complete Task A design (完成任务 A 设计)
- ⏰ **Hour 2**: Complete Task B model (完成任务 B 模型)
- ⏰ **Hour 3**: Documentation and photos (文档和照片)
- ⏰ **Final 30 min**: Review, organize files, submit (审查、组织文件、提交)

### Getting Help | 获取帮助

- 💬 Ask your instructor or TAs during class (课堂上询问讲师或助教)
- 🤝 Work with classmates - collaboration is encouraged! (与同学合作 - 鼓励协作！)
- 📖 Check DESIGN-GUIDE.md for detailed tutorials (查看 DESIGN-GUIDE.md 获取详细教程)

---

## 📄 Grading | 评分

**Total Points | 总分**: 100 points (100分)

See **[rubric.md](./rubric.md)** for detailed grading criteria.

详细评分标准见 **[rubric.md](./rubric.md)**。

**Quick Breakdown | 快速分解:**
- Laser Cutting Design (40 pts) | 激光切割设计（40 分）
- 3D Printing Model (40 pts) | 3D 打印模型（40 分）
- Documentation (15 pts) | 文档（15 分）
- Photos (5 pts) | 照片（5 分）
- Bonus (up to +10 pts) | 加分（最多 +10 分）

---

## 🎉 What's Next? | 接下来做什么？

After completing this assignment:

完成此作业后：

- **Keep designing!** Your files are yours forever (继续设计！文件永远是你的)
- **Share your work** with friends and on social media (与朋友和社交媒体分享作品)
- **Iterate and improve** your designs based on feedback (根据反馈迭代和改进设计)
- **Prepare for fabrication** in the next session (为下一次会议的制造做准备)

---

**Happy Making! 🎨🔧💡**

**祝你创作愉快！🎨🔧💡**

---

*If you have any questions, don't hesitate to ask. We're here to help you succeed!*

*如果你有任何问题，请随时提问。我们在这里帮助你成功！*


