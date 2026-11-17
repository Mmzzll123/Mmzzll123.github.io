# 心晴手册 · 班级心理委员个人主页

马振霖（Mǎ Zhènlín）的**心理委员主题个人主页**：单文件 HTML + CSS + 原生 JS，零依赖、零构建、零后端。所有记录类功能只写本机浏览器 `localStorage`，不收集、不上传任何数据。

> 一个可以慢慢看的地方：情绪工具、心理科普与求助资源。

## 模块一览

| 编号 | 模块 | 内容 |
| --- | --- | --- |
| — | 首屏 | 姓名三行（中文 / 拼音 / 英文）、呼吸圆环动效、快捷入口 |
| 01 | 关于我 | 心理委员自述 + 三条工作信念 |
| 02 | 我在做什么 | 六张职责卡：倾听、科普、活动、转介、边界、自我照顾 |
| 03 | 心晴工具 | 情绪天气记录（含统计条与时间线）、4-7-8 呼吸练习（带节律动画与倒计时）、两周情绪小自查（5 题计分，非诊断） |
| 04 | 心理科普 | 四组「误解 vs 事实」对照 + 六个实用心理效应卡片 |
| 05 | 求助资源 | 危机提示框 + 渠道表格（12356 等全国热线 + 校内渠道占位） |
| 06 | 树洞 | 本机留言板：写入、删除、清空、字数统计 |
| — | 全站 | 深浅色切换、锚点导航滚动高亮、滚动入场动画、响应式（桌面 / 平板 / 手机）、打印样式、`prefers-reduced-motion` 降级 |

## 本地预览

直接双击 `index.html`；或：

```bash
python3 -m http.server 8000
# 访问 http://localhost:8000
```

## 部署到 GitHub Pages

以 `<username>` 代表你的 GitHub 用户名：

1. 在 GitHub 新建仓库 `<username>.github.io`（Public，不勾任何初始化文件）。
2. 推送本目录：

   ```bash
   git init
   git add .
   git commit -m "feat: mental-health commissioner homepage"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```

3. Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)` → Save。
4. 访问 `https://<username>.github.io`。

## 发布前必须修改的占位内容

| 位置 | 现状 | 改成 |
| --- | --- | --- |
| 「求助资源」表格第一行  | 本校心理健康教育中心的真实预约方式 |
| 页脚 GitHub 链接 | `href="https://github.com/"` | 你的主页地址 |
| 页脚邮箱 | `mailto:your@email.com` | 你的邮箱 |

另外两处建议核对：

- 姓名拼音、学校名（首屏与页脚）按实际情况调整；
- 页面中所有热线号码发布前再核对一次官方公告。

## 隐私与边界声明

- 情绪记录与树洞留言仅存于本机浏览器 `localStorage`，清除浏览器数据即消失。
- 页面反复强调：**心理委员不是心理咨询师**；自查工具不构成诊断，不替代专业评估。
- 危机信息（12356、危机干预热线）置于显著位置，符合心理委员工作伦理。

## 许可

MIT，见 [LICENSE](LICENSE)。
