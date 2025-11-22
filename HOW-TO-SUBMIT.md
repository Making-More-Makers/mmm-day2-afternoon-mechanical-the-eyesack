# How to Submit Your Mechanical Assignment
# 如何提交你的机械作业

## Quick Start | 快速开始

Follow these steps to submit your laser cutting and 3D printing work:

按照以下步骤提交你的激光切割和 3D 打印作品：

---

## 🗂️ Step 1: Organize Your Files | 组织文件

### Create the Folder Structure | 创建文件夹结构

Your submission must be organized like this:

你的提交必须按以下方式组织：

```
YourName_Assignment/
│
├── submission.json
├── A_LaserCut/
│   ├── design_source.ai (or .svg)
│   ├── final_export.dxf
│   ├── README_LaserCut.md
│   └── photos/
│       ├── photo1.png
│       └── photo2.jpg
│
└── B_3DModel/
    ├── model.stl
    ├── README_3DPrint.md
    ├── tinkercad_link.txt (optional)
    └── photos/
        ├── screenshot1.png
        └── screenshot2.png
```

### Using Terminal/Command Line | 使用终端/命令行

```bash
# Create folders | 创建文件夹
mkdir A_LaserCut
mkdir A_LaserCut/photos
mkdir B_3DModel
mkdir B_3DModel/photos

# Move your files into the correct folders
# 将文件移动到正确的文件夹
# (Use your file manager or mv commands)
```

### Using File Manager (Easier for Beginners) | 使用文件管理器（更适合初学者）

**Windows/Mac/Linux:**
1. Right-click → New Folder (右键 → 新建文件夹)
2. Name it exactly: `A_LaserCut` (名称准确：`A_LaserCut`)
3. Create subfolder: `A_LaserCut/photos` (创建子文件夹)
4. Repeat for `B_3DModel` (重复 `B_3DModel`)
5. Drag your files into correct folders (将文件拖到正确文件夹)

---

## 📝 Step 2: Fill Out submission.json | 填写 submission.json

### Create the File | 创建文件

Create a file named `submission.json` in your main folder:

在主文件夹中创建名为 `submission.json` 的文件：

```json
{
  "student_name": "Zhang San (张三)",
  "laser_cut_project_type": "keychain",
  "3d_model_project_type": "badge",
  "completion_date": "2024-11-22",
  "notes": "I designed a keychain with my initials and a badge with a star shape."
}
```

### Fill in Your Information | 填写你的信息

**Required fields | 必需字段:**

| Field | What to Enter | Example |
|-------|---------------|---------|
| `student_name` | Your full name | "李明 (Li Ming)" |
| `laser_cut_project_type` | Choose one: `keychain`, `sign`, or `snap-fit` | "keychain" |
| `3d_model_project_type` | Choose one: `badge`, `accessory`, or `phone-stand` | "badge" |
| `completion_date` | Today's date (YYYY-MM-DD) | "2024-11-22" |
| `notes` | Optional: Any comments | "My first 3D design!" |

**⚠️ Important | 重要:**
- Use exact project type names (使用确切的项目类型名称)
- Keep the JSON format (quotes, commas, braces) (保持 JSON 格式（引号、逗号、大括号）)
- Replace ALL placeholder text (替换所有占位符文本)

---

## ✍️ Step 3: Write Your README Files | 编写 README 文件

### README_LaserCut.md Template | 模板

Create `A_LaserCut/README_LaserCut.md`:

创建 `A_LaserCut/README_LaserCut.md`：

```markdown
# Laser Cutting Assignment (DXF)

## 1. My Design | 我的设计

- **Project Type | 项目类型**: Keychain
- **Design Theme | 设计主题**: My initials "ZS" in a hexagonal frame
- **Dimensions | 尺寸**: 6 cm × 4 cm

## 2. Design Process | 制作步骤

1. Sketched my initials on paper to plan the layout
2. Created hexagon base in Inkscape using polygon tool
3. Added text with my initials and converted to paths
4. Added keyring hole (5mm diameter) at top
5. Set all strokes to 0.01mm and exported as DXF

## 3. Design Concept | 设计概念

I wanted a simple but personal keychain with my initials. The hexagonal shape 
makes it modern and easy to identify. I chose a bold font that will cut cleanly 
and be readable at small size.

## 4. Technical Checklist | 技术检查清单

- [x] All lines are vector paths
- [x] Line width is 0.01 mm
- [x] All shapes are closed
- [x] Minimum details > 1 mm
- [x] Text converted to paths
- [x] File exported as DXF

## 5. Files Included | 文件说明

- **Source file**: `design_source.svg` - Original Inkscape design
- **Export file**: `final_export.dxf` - Ready for laser cutting
- **Photos**: 
  - `inkscape_screenshot.png` - Design in Inkscape
  - `detail_view.png` - Close-up of initials
```

### README_3DPrint.md Template | 模板

Create `B_3DModel/README_3DPrint.md`:

创建 `B_3DModel/README_3DPrint.md`：

```markdown
# 3D Printing Assignment (STL)

## 1. My Model | 我的模型

- **Model Type | 模型类型**: Badge
- **Model Dimensions | 模型尺寸**: 30mm × 30mm × 3mm
- **Minimum Wall Thickness | 最小壁厚**: 2 mm

## 2. Design Concept | 设计概念

I created a star-shaped badge with my name embossed on top. The design is 
simple but has 3D relief that makes it interesting. I added a small hole at 
the top so it can be attached to clothing or a bag.

## 3. Modeling Steps | 建模步骤

1. Started with a cylinder (30mm diameter, 3mm height) as base
2. Added a star shape from basic shapes and scaled to fit
3. Grouped star with cylinder using Union
4. Added text with my name, raised it to 4mm height
5. Added small cylinder (2mm) for attachment hole, made it a Hole
6. Grouped everything and exported as STL

## 4. Printability Checklist | 可打印性检查清单

- [x] Model is a closed solid
- [x] Wall thickness ≥ 1.2 mm
- [x] No overhangs > 45°
- [x] Model sits flat on workplane
- [x] Size ≤ 50 mm
- [x] All shapes grouped
- [x] Exported as STL

## 5. Files Included | 文件说明

- **Model file**: `model.stl` - 3D printable badge
- **Tinkercad link**: https://www.tinkercad.com/things/abc123xyz
- **Photos**: 
  - `front_view.png` - Main view of badge
  - `angle_view.png` - 3D perspective showing thickness
```

**Tips for writing READMEs | 编写 README 的提示:**
- Be specific about steps (具体说明步骤)
- Explain WHY you made design choices (解释为什么做出设计选择)
- Write in complete sentences (用完整句子写)
- Minimum 100 words per README (每个 README 至少 100 字)

---

## 📸 Step 4: Add Photos/Screenshots | 添加照片/截图

### For Laser Cutting (A_LaserCut/photos/) | 激光切割

**Required | 必需:** Minimum 2 photos (至少 2 张照片)

**Photo 1: Design Screenshot | 设计截图**
- Open your design in Inkscape/Illustrator (在 Inkscape/Illustrator 中打开设计)
- Zoom to fit the whole design (缩放以适应整个设计)
- Take screenshot: 
  - **Windows**: `Windows + Shift + S`
  - **Mac**: `Command + Shift + 4`
  - **Linux**: `PrtScn`
- Save as `design_screenshot.png` (保存为 `design_screenshot.png`)

**Photo 2: Detail View | 细节视图**
- Zoom in on interesting details (放大有趣的细节)
- OR show your planning sketch (或显示规划草图)
- Take screenshot (截图)
- Save as `detail_view.png` (保存为 `detail_view.png`)

### For 3D Printing (B_3DModel/photos/) | 3D 打印

**Required | 必需:** Minimum 2 screenshots (至少 2 张截图)

**Screenshot 1: Front View | 正面视图**
- In Tinkercad, rotate to show front of model (在 Tinkercad 中，旋转以显示模型正面)
- Make sure model is centered (确保模型居中)
- Take screenshot (截图)
- Save as `front_view.png` (保存为 `front_view.png`)

**Screenshot 2: Angle View | 角度视图**
- Rotate view cube to show 3D perspective (旋转视图立方体以显示 3D 透视)
- Show thickness and depth (显示厚度和深度)
- Take screenshot (截图)
- Save as `angle_view.png` (保存为 `angle_view.png`)

**Screenshot tips | 截图提示:**
- Use Tinkercad's screenshot feature (使用 Tinkercad 的截图功能)
- Or use OS screenshot tool (或使用操作系统截图工具)
- Make sure image is clear and in focus (确保图像清晰且对焦)
- File size should be < 5 MB (文件大小应 < 5 MB)

---

## 🔗 Step 5: Get Tinkercad Link (Optional) | 获取 Tinkercad 链接（可选）

**Bonus +1 point | 加 1 分**

### How to Share Your Tinkercad Design | 如何分享 Tinkercad 设计

1. **In Tinkercad, click the "Share" button** (在 Tinkercad 中，点击"分享"按钮)
   - Top right corner of your design (设计的右上角)

2. **Change privacy settings | 更改隐私设置:**
   - Select "Anyone with the link" (选择"任何有链接的人")
   - Make sure "Allow others to edit" is OFF (确保"允许他人编辑"关闭)

3. **Copy the link | 复制链接:**
   - Click "Copy Link" (点击"复制链接")
   - Link looks like: `https://www.tinkercad.com/things/abc123xyz`

4. **Save to file | 保存到文件:**
   - Create `B_3DModel/tinkercad_link.txt` (创建文件)
   - Paste your link (粘贴链接)
   - Save (保存)

**Example tinkercad_link.txt | 示例:**
```
https://www.tinkercad.com/things/1A2B3C4D5E
```

---

## 💻 Step 6: Clone Your GitHub Classroom Repository | 克隆你的 GitHub Classroom 仓库

### Get Your Repository URL | 获取仓库 URL

After accepting the GitHub Classroom assignment, you'll receive a repository URL.

接受 GitHub Classroom 作业后，你会收到一个仓库 URL。

**Finding your repository URL | 查找仓库 URL:**
1. Accept the GitHub Classroom assignment link (接受 GitHub Classroom 作业链接)
2. GitHub creates a repository for you (GitHub 为你创建仓库)
3. Copy the repository URL shown (复制显示的仓库 URL)
   - Format: `https://github.com/YOUR-ORG/assignment-name-YOUR-USERNAME`

**Clone the repository | 克隆仓库:**

Open Terminal/Command Prompt and run:

打开终端/命令提示符并运行：

```bash
# Clone your repository | 克隆仓库
git clone https://github.com/YOUR-ORG/assignment-name-YOUR-USERNAME.git

# Example | 例如:
# git clone https://github.com/maker-course/day2-afternoon-alice.git
```

**What happens | 会发生什么:**
- Git downloads the repository to your computer (Git 将仓库下载到电脑)
- Creates a folder with the repository name (创建一个以仓库名命名的文件夹)
- All files and Git history are copied (所有文件和 Git 历史都被复制)

---

## 📂 Step 7: Navigate to Repository Folder | 进入仓库文件夹

```bash
# Change directory to your repository | 进入仓库目录
cd assignment-name-YOUR-USERNAME

# Example | 例如:
# cd day2-afternoon-alice
```

**Verify you're in the right folder | 验证你在正确的文件夹:**

```bash
# Check current directory | 检查当前目录
pwd   # Mac/Linux
cd    # Windows

# List files | 列出文件
ls    # Mac/Linux  
dir   # Windows
```

You should see the repository files (README.md, etc.)

你应该看到仓库文件（README.md 等）

---

## ✏️ Step 8: Add Your Work | 添加你的作品

Now create your folders and add your files:

现在创建文件夹并添加文件：

```bash
# Create folders | 创建文件夹
mkdir A_LaserCut
mkdir A_LaserCut/photos
mkdir B_3DModel
mkdir B_3DModel/photos
```

Then:
1. Copy your design files into the folders (将设计文件复制到文件夹)
2. Fill out submission.json (填写 submission.json)
3. Create README files (创建 README 文件)
4. Add your photos/screenshots (添加照片/截图)

---

## 🔍 Step 9: Check Status | 检查状态

Before committing, check what files have changed:

提交前，检查哪些文件已更改：

```bash
# Check repository status | 检查仓库状态
git status
```

**You should see | 你应该看到:**
```
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        A_LaserCut/
        B_3DModel/
        submission.json
        ...
```

Red text = files not yet added to Git (红色文本 = 文件尚未添加到 Git)

---

## ➕ Step 10: Add Files to Git | 添加文件到 Git

```bash
# Add all files | 添加所有文件
git add .

# Alternative: Add specific folders | 或者：添加特定文件夹
# git add A_LaserCut/ B_3DModel/ submission.json
```

**Check status again | 再次检查状态:**

```bash
git status
```

**Now you should see | 现在你应该看到:**
```
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   A_LaserCut/design_source.svg
        new file:   A_LaserCut/final_export.dxf
        new file:   A_LaserCut/README_LaserCut.md
        ...
```

Green text = files ready to commit (绿色文本 = 文件准备提交)

---

## 💾 Step 11: Commit Changes | 提交更改

```bash
# Commit with a descriptive message | 带描述性消息提交
git commit -m "Submit Day 2 Afternoon mechanical assignment"
```

**Good commit messages | 好的提交消息:**
- "Submit Day 2 Afternoon mechanical assignment" (提交第2天下午机械作业)
- "Add laser cutting and 3D printing projects" (添加激光切割和 3D 打印项目)
- "Complete Task A and Task B with documentation" (完成任务 A 和任务 B 及文档)

**What you'll see | 你会看到:**
```
[main a1b2c3d] Submit Day 2 Afternoon mechanical assignment
 15 files changed, 234 insertions(+)
 create mode 100644 A_LaserCut/design_source.svg
 create mode 100644 A_LaserCut/final_export.dxf
 ...
```

---

## 🔍 Step 12: Verify Commit Status | 验证提交状态

```bash
# Check status after commit | 提交后检查状态
git status
```

**You should see | 你应该看到:**
```
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
```

This means:
- ✅ All files are committed (所有文件已提交)
- ✅ Ready to push to GitHub (准备推送到 GitHub)
- ✅ Local changes saved (本地更改已保存)

---

## 🚀 Step 13: Push to GitHub | 推送到 GitHub

```bash
# Push your changes to GitHub | 推送更改到 GitHub
git push
```

**If this is your first push | 如果这是第一次推送:**
```bash
# You might need to use | 你可能需要使用:
git push -u origin main
```

**What happens | 会发生什么:**
- Your local commits upload to GitHub (本地提交上传到 GitHub)
- Changes become visible on GitHub website (更改在 GitHub 网站上可见)
- GitHub Actions will automatically run (GitHub Actions 将自动运行)

**Successful output | 成功的输出:**
```
Enumerating objects: 25, done.
Counting objects: 100% (25/25), done.
Delta compression using up to 8 threads
Compressing objects: 100% (20/20), done.
Writing objects: 100% (24/24), 5.67 MiB | 2.34 MiB/s, done.
Total 24 (delta 3), reused 0 (delta 0)
To https://github.com/YOUR-ORG/assignment-name-YOUR-USERNAME.git
   a1b2c3d..e4f5g6h  main -> main
```

**If Git asks for authentication | 如果 Git 要求身份验证:**

**Option 1: Personal Access Token (Recommended) | 选项1：个人访问令牌（推荐）**
1. Go to GitHub → Settings → Developer settings → Personal access tokens (访问 GitHub)
2. Generate new token (classic) (生成新令牌)
3. Select scope: `repo` (full control) (选择范围：`repo`（完全控制）)
4. Copy the token (复制令牌)
5. When prompted:
   - Username: your GitHub username (你的 GitHub 用户名)
   - Password: paste your token (粘贴令牌)

**Option 2: SSH Key | 选项2：SSH 密钥**
- See: https://docs.github.com/en/authentication/connecting-to-github-with-ssh

---

## ✅ Step 14: Verify Submission | 验证提交

### Check GitHub Repository | 检查 GitHub 仓库

1. **Open your repository on GitHub | 在 GitHub 上打开仓库**
   - Go to your repository URL in a browser (在浏览器中访问仓库 URL)
   - Or click the link from GitHub Classroom (或点击 GitHub Classroom 的链接)

2. **Verify all files are there | 验证所有文件都在:**
   - ✅ `submission.json`
   - ✅ `A_LaserCut/` folder with all files (文件夹及所有文件)
   - ✅ `B_3DModel/` folder with all files (文件夹及所有文件)
   - ✅ README files (README 文件)
   - ✅ Photos/screenshots (照片/截图)

3. **Check GitHub Actions | 检查 GitHub Actions:**
   - Click "Actions" tab (点击"Actions"标签)
   - You should see a workflow run in progress or completed (应该看到正在进行或已完成的工作流运行)
   - Green checkmark ✅ = validation passed (绿色复选标记 = 验证通过)
   - Red X ❌ = validation failed (check errors) (红色 X = 验证失败（检查错误）)

4. **Read feedback in Issues | 在 Issues 中阅读反馈:**
   - Click "Issues" tab (点击"Issues"标签)
   - Look for "File Validation Feedback" issue (查找"文件验证反馈"问题)
   - Read the automated feedback (阅读自动反馈)

---

## 🔧 Troubleshooting | 故障排除

### ❌ Git Clone Failed | Git 克隆失败

**Error: "fatal: could not read Username" | 错误："无法读取用户名"**

**Solution | 解决方案:**
- Make sure you accepted the GitHub Classroom assignment first (确保先接受了 GitHub Classroom 作业)
- Copy the correct repository URL (复制正确的仓库 URL)
- Check your internet connection (检查互联网连接)

**Error: "repository not found" | 错误："仓库未找到"**

**Solution | 解决方案:**
- Verify the URL is correct (验证 URL 正确)
- Make sure you're logged into GitHub (确保已登录 GitHub)
- Check if you have access to the repository (检查是否有仓库访问权限)

### ❌ Git Push Failed | Git 推送失败

**Error: "failed to push some refs" | 错误："推送某些引用失败"**

**Reason | 原因:** Remote repository has changes you don't have locally (远程仓库有你本地没有的更改)

**Solution | 解决方案:**
```bash
# Pull remote changes first | 先拉取远程更改
git pull origin main

# Then push | 然后推送
git push
```

**Error: "Authentication failed" | 错误："身份验证失败"**

**Solution | 解决方案:**
1. Use Personal Access Token instead of password (使用个人访问令牌而非密码)
2. Generate new token at: GitHub → Settings → Developer settings (在以下位置生成新令牌)
3. Use token as password when prompted (提示时使用令牌作为密码)

### ❌ File Validation Failed | 文件验证失败

**Check the Issues tab for specific errors:**

**检查 Issues 标签了解具体错误：**

1. Read error message carefully (仔细阅读错误消息)
2. Fix the issues (修复问题)
3. Commit changes:
   ```bash
   git add .
   git commit -m "Fix validation errors"
   git push origin main
   ```
4. Validation will run again automatically (验证将自动再次运行)

### ❌ Files Not Showing on GitHub | GitHub 上未显示文件

**Possible causes | 可能原因:**

1. **Files not added to Git | 文件未添加到 Git:**
   ```bash
   git status  # Check what's tracked
   git add .   # Add all files
   git commit -m "Add missing files"
   git push origin main
   ```

2. **Large files | 大文件:**
   - GitHub has 100 MB file limit (GitHub 有 100 MB 文件限制)
   - Compress photos if too large (如果照片太大则压缩)

3. **Incorrect .gitignore | 不正确的 .gitignore:**
   - Make sure no important files are ignored (确保没有重要文件被忽略)

### ❌ README Not Displaying | README 未显示

**Check | 检查:**
- File name is exactly: `README_LaserCut.md` (not `readme.md`) (文件名准确)
- File is in correct folder: `A_LaserCut/README_LaserCut.md` (文件在正确文件夹中)
- File has content (not empty) (文件有内容（非空）)

### ❌ Photos Not Loading | 照片未加载

**Check | 检查:**
- File format is supported: `.jpg`, `.jpeg`, `.png`, `.heic`, `.webp`
- File size is < 5 MB per photo (文件大小 < 5 MB)
- Files are in `photos/` subfolder (or main task folder) (文件在子文件夹中)

---

## 📋 Final Checklist | 最终检查清单

Before considering your submission complete, verify:

在认为提交完成之前，验证：

### Files Present | 文件存在
- [ ] `submission.json` filled out correctly (正确填写)
- [ ] `A_LaserCut/` folder exists (文件夹存在)
  - [ ] Source file (.ai or .svg) (源文件)
  - [ ] DXF export file (DXF 导出文件)
  - [ ] README_LaserCut.md (complete) (README_LaserCut.md（完整）)
  - [ ] At least 2 photos (至少 2 张照片)
- [ ] `B_3DModel/` folder exists (文件夹存在)
  - [ ] model.stl file (model.stl 文件)
  - [ ] README_3DPrint.md (complete) (README_3DPrint.md（完整）)
  - [ ] At least 2 screenshots (至少 2 张截图)
  - [ ] tinkercad_link.txt (optional) (tinkercad_link.txt（可选）)

### Git & GitHub | Git 和 GitHub
- [ ] All files committed to Git (所有文件已提交到 Git)
- [ ] Pushed to GitHub successfully (成功推送到 GitHub)
- [ ] All files visible on GitHub (GitHub 上可见所有文件)
- [ ] GitHub Actions ran (workflow executed) (GitHub Actions 已运行)
- [ ] Validation passed or errors reviewed (验证通过或已查看错误)

### Content Quality | 内容质量
- [ ] READMEs have meaningful content (README 有有意义的内容)
- [ ] All checklists completed (所有检查清单已完成)
- [ ] Photos are clear and relevant (照片清晰相关)
- [ ] Design meets technical requirements (设计满足技术要求)

---

## 🎉 Submission Complete! | 提交完成！

**Once everything is pushed and validated:**

**一旦一切都推送并验证后：**

✅ Your submission is complete! (你的提交完成了！)
✅ Wait for instructor review (等待讲师审查)
✅ Check Issues tab for feedback (查看 Issues 标签获取反馈)
✅ If needed, you can push updates (如需要，可以推送更新)

---

## 🔄 Making Changes After Submission | 提交后进行更改

**You can always update your submission:**

**你始终可以更新提交：**

```bash
# Make your changes | 进行更改
# Edit files, add photos, improve READMEs, etc.

# Add and commit | 添加并提交
git add .
git commit -m "Improve documentation and add more photos"

# Push updates | 推送更新
git push origin main
```

Validation will run again automatically!

验证将自动再次运行！

---

## 💬 Need Help? | 需要帮助？

**Resources | 资源:**
- [README.md](./README.md) - Full assignment instructions (完整作业说明)
- [DESIGN-GUIDE.md](./DESIGN-GUIDE.md) - Design rules and tutorials (设计规则和教程)
- [SUBMISSION.md](./SUBMISSION.md) - Detailed requirements (详细要求)
- [rubric.md](./rubric.md) - Grading criteria (评分标准)

**Get help from | 从以下获取帮助:**
- 👨‍🏫 Your instructor or TAs (讲师或助教)
- 👥 Classmates (collaboration encouraged!) (同学（鼓励协作！）)
- 📚 Course discussion forum (课程讨论论坛)

---

**Good luck! You've got this! 🚀**

**祝你好运！你能做到！🚀**

---

## 📌 Quick Reference Commands | 快速参考命令

```bash
# === GitHub Classroom Workflow | GitHub Classroom 工作流程 ===

# 1. Clone repository | 克隆仓库
git clone https://github.com/YOUR-ORG/assignment-name-YOUR-USERNAME.git

# 2. Navigate to folder | 进入文件夹
cd assignment-name-YOUR-USERNAME

# 3. Create folders | 创建文件夹
mkdir A_LaserCut A_LaserCut/photos B_3DModel B_3DModel/photos

# 4. Add your files, then check status | 添加文件后检查状态
git status

# 5. Add all files | 添加所有文件
git add .

# 6. Check status again | 再次检查状态
git status

# 7. Commit changes | 提交更改
git commit -m "Submit Day 2 Afternoon mechanical assignment"

# 8. Check status after commit | 提交后检查状态
git status

# 9. Push to GitHub | 推送到 GitHub
git push

# === Making Changes Later | 后续修改 ===

# After making changes | 做出更改后
git status              # Check what changed
git add .              # Add changes
git commit -m "Update documentation"
git push               # Push updates

# === Useful Commands | 实用命令 ===

# View commit history | 查看提交历史
git log --oneline

# View remote URL | 查看远程 URL
git remote -v

# Pull latest changes | 拉取最新更改
git pull

# Check Git version | 检查 Git 版本
git --version
```

**Save these commands for quick reference!**

**保存这些命令以供快速参考！**

