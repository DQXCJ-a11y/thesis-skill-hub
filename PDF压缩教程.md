# 📦 论文PDF压缩教程

**问题：** 论文PDF超过31MB，无法上传到Claude进行审查

**解决：** 用免费开源工具Ghostscript压缩，通常31MB可压到3-8MB，不影响文字清晰度

**适用系统：** Windows 10 / 11

**所需时间：** 首次安装约5分钟，之后每次压缩10秒

---

## 第一步：下载Ghostscript

1. 打开浏览器，进入官方下载页面：

```
https://github.com/ArtifexSoftware/ghostpdl-downloads/releases
```

2. 找到最新版本（如 `gs10060w64.exe`），点击下载
3. 如果打不开GitHub，备用地址：`https://ghostscript.com/releases/gsdnld.html`

> ⚠ 只下载 **64位版本**（文件名含 `w64`），不要下32位的

---

## 第二步：安装

1. 双击下载好的 `.exe` 文件
2. **记住安装路径**（默认是 `C:\Program Files\gs\gs版本号\`）
3. 一路点 Next → Install → Finish

**安装完成后确认一下路径：** 打开文件管理器，进入安装目录，找到这个文件：

```
C:\Program Files\gs\gs10.06.0\bin\gswin64c.exe
```

> ⚠ 版本号可能不同（如 `gs10.04.0`、`gs10.06.0`），以你实际安装的为准
>
> ⚠ 如果你安装到了D盘，路径就是 `D:\gs10.06.0\bin\gswin64c.exe`

---

## 第三步：压缩PDF

### 3.1 准备工作

把你的论文PDF复制到**桌面**，记住文件名（比如 `论文.pdf`）

### 3.2 打开命令行

按键盘 `Win + R`，输入 `cmd`，回车

### 3.3 输入压缩命令

把下面这行命令复制到cmd窗口（右键粘贴），**修改两个地方后**按回车：

```
"C:\Program Files\gs\gs10.06.0\bin\gswin64c.exe" -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -dNOPAUSE -dQUIET -dBATCH -sOutputFile="%USERPROFILE%\Desktop\压缩版.pdf" "%USERPROFILE%\Desktop\论文.pdf"
```

**你需要修改的两个地方：**

| 修改项 | 改成什么 | 举例 |
|--------|---------|------|
| `gs10.06.0` | 你实际安装的版本号 | 如果是10.04.0就改成 `gs10.04.0` |
| `论文.pdf` | 你的实际文件名 | 如果叫 `毕业论文终稿.pdf` 就改成它 |

> ⚠ 其他参数不要动！
>
> ⚠ 如果你装在D盘，把开头的 `C:\Program Files\gs\` 改成 `D:\`

### 3.4 等待完成

回车后等几秒钟，桌面会自动出现 **`压缩版.pdf`**，这就是压缩后的文件。

---

## 压缩质量选择

命令里的 `/ebook` 控制压缩程度，可以换成其他选项：

| 参数 | 图片质量 | 压缩效果 | 适合场景 |
|------|---------|---------|---------|
| `/screen` | 72 dpi | 最小 | 只需看文字，不在意图片 |
| **`/ebook`** | **150 dpi** | **中等** | **上传Claude/发邮件（推荐）** |
| `/printer` | 300 dpi | 较大 | 需要打印 |
| `/prepress` | 最高 | 最大 | 出版印刷 |

**建议：** 先用 `/ebook` 试一次。如果压缩后图片太模糊，换 `/printer`；如果还是太大，换 `/screen`。

---

## 常见问题

**Q：提示"找不到文件"**
- 检查文件名是否打对了（包括中英文、空格、后缀名）
- 确认PDF确实在桌面上
- 文件名有空格的话，确保命令里的双引号没有丢

**Q：提示"gswin64c不是内部命令"**
- 路径里的版本号和你实际安装的不一致，去文件管理器确认真实版本号
- 确认安装盘符对不对（C盘还是D盘）

**Q：压缩后反而变大了**
- 原PDF可能已经被压缩过了，再压没效果
- 试试换 `/screen` 参数

**Q：Mac系统怎么办**
- 安装Homebrew后执行 `brew install ghostscript`
- 压缩命令改为：
```
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -dNOPAUSE -dQUIET -dBATCH -sOutputFile=~/Desktop/压缩版.pdf ~/Desktop/论文.pdf
```

---

## 不想装软件？在线替代方案

| 工具 | 地址 | 说明 |
|------|------|------|
| iLovePDF | `ilovepdf.com/compress_pdf` | 免费，有文件大小限制 |
| Smallpdf | `smallpdf.com/compress-pdf` | 免费版每天2次 |

> ⚠ 在线工具会把你的论文上传到别人的服务器，如果论文涉及保密内容，建议用Ghostscript本地处理
