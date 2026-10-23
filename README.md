# 隐私政策发布说明（GitHub Pages）

> 背景：商店驳回原因是隐私政策链接填了 `https://github.com/strenchen`（个人主页，无政策内容）。
> 解决方案：把本目录的 `privacy.html`（中英双语、自包含单页，logo 已内嵌为 base64，无需其他文件）
> 发布到 GitHub Pages，得到一个正式网页链接，再回填 Partner Center。

## 最终链接（发布成功后）

```
https://strenchen.github.io/netkeeper-site/privacy.html
```

## 发布步骤（约 5 分钟，全部在浏览器中操作）

1. **新建仓库**
   - 打开 https://github.com/new
   - Repository name：`netkeeper-site`
   - 可见性：**Public**（必须公开，Pages 免费版要求）
   - 勾选 "Add a README file"（可选）→ Create repository

2. **上传 privacy.html**
   - 进入刚建的仓库 → Add file → **Upload files**
   - 选择本目录下的 `privacy.html`（完整路径：`doc\privacy\privacy.html`）
   - Commit message 随意（如 `Add privacy policy`）→ Commit changes

3. **开启 GitHub Pages**
   - 仓库 → Settings → 左侧 **Pages**
   - Build and deployment → Source：**Deploy from a branch**
   - Branch：`main` / 目录 `(root)` → **Save**

4. **验证**
   - 等待 1–3 分钟后访问：https://strenchen.github.io/netkeeper-site/privacy.html
   - 确认页面正常显示（绿色页头 + logo + 中文政策 + English policy）
   - 用无痕窗口再验证一次（排除本地缓存/登录态干扰）

5. **回填 Partner Center**
   - 位置：合作伙伴中心 → 该应用 → 提交 → **「隐私策略 / Privacy policy」链接字段**
     （即当初填 `https://github.com/strenchen` 的那个输入框）
   - 替换为：`https://strenchen.github.io/netkeeper-site/privacy.html`
   - **所有提交语言**（当前为中文-中国）都要替换
   - 保存并重新提交

## 注意事项

- 政策正文与源码事实严格一致（零收集、纯本地 `%AppData%\NetKeeper`、仅直连用户选择的目标与测速节点），
  审核员对照应用行为时不会产生矛盾。
- 商店「说明」字段不允许含 URL，政策链接只填在专门的「隐私策略」字段；说明里的【隐私承诺】文案已同步修正
  （见 `doc\storeView\中文\商店一览-中文（中国）.md` 第 2 节）。
- 联系渠道使用仓库 Issues（`https://github.com/strenchen/netkeeper-site/issues`），无需公开个人邮箱；
  如希望改用邮箱联系，编辑 `privacy.html` 第 10 节后重新上传即可。
- 日后政策有改动：直接编辑 `privacy.html` → 仓库页面点击文件 → 铅笔图标 Edit → 粘贴新内容 → Commit，
  Pages 会在 1 分钟左右自动更新。
