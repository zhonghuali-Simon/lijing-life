# 立鲸人生成长系统

个人养成系任务/积分/能力库面板 · 单文件 HTML + localStorage 存储

## 在线访问

部署后地址：`https://<你的GitHub用户名>.github.io/lijing-life/`

## 特性

- 🎮 6 维度能力面板（PM/DA/TL/TM/RI/BODY）+ 30 枚徽章
- 📌 今日任务清单，难度自动打分（XS-XXL）+ 关键词识别维度
- 🎁 兑换商店（星币奖励制）
- 📅 历史热力图 + 趋势图
- 🍅 番茄专注计时
- 🏅 能力库（证书/技能档案）
- 💾 一键 JSON 备份/恢复

## 部署到 GitHub Pages

### 步骤

1. 在 GitHub 新建仓库 `lijing-life`（public 或 private 均可）
2. 上传本目录所有文件（`index.html` + `README.md`）
3. 进入仓库 → **Settings → Pages**
4. Source 选 `Deploy from a branch`，Branch 选 `main` / root，点 Save
5. 等 1-2 分钟，页面顶部会显示 `Your site is live at ...` 的链接

### 或用命令行推送

```bash
cd 本目录
git init
git add .
git commit -m "init 立鲸人生成长系统"
git branch -M main
git remote add origin git@github.com:<你的用户名>/lijing-life.git
git push -u origin main
```

## 隐私提示

- 所有数据存在**你自己浏览器的 localStorage**，不会上传服务器
- 如果仓库设为 **public**，代码任何人可看，但你的数据始终只在你自己的浏览器里
- 换设备/清缓存会丢数据 → 用「💾 备份」按钮定期导出 JSON

## 换设备如何迁移

1. 老设备：点「💾 备份」下载 JSON
2. 新设备：打开同一个网址 → 点「📥 导入」选择那个 JSON

## 想要多端同步？

需要加后端。推荐 Supabase 免费方案（约 200 行代码改造）。
