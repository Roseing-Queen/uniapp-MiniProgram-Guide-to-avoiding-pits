# 微信小程序 & uni-app 开发禁忌  
**WeChat Mini Programs & uni-app Development Taboos**

> ⚠️ 不是官方文档，而是一本“血泪避坑手册”。  
> ⚠️ Not official docs, but a **survival guide full of painful lessons**.

---

## 🤔 这是什么 / What is this?

写小程序和 uni-app 的体验，大概就是：  
- 以为写的是 **Web**，结果发现是 **伪 Web**；  
- 模拟器告诉你“没问题”，真机说“呵呵”；  
- 文档写“支持”，实际就是“部分支持”；  
- 审核规则？玄学。  

This repo is a collection of:  
- ❌ Things you **should NOT do** in WeChat Mini Programs & uni-app  
- 💡 Tips & tricks to **avoid unnecessary pain**  
- 😂吐槽 & WTFs that every developer will eventually meet  

---

## 🎯 目标 / Goals

- 记录开发中各种“**禁忌**”和坑点  
- 让后来者少踩雷，少掉头发  
- 让大家在吐槽的同时，至少还能笑着掉坑里  

---

## 💀 经典吐槽 / Highlights

- `<div>`? 不存在的，用 `<view>` 吧。  
- `rpx` = **Random PX (随缘像素)**。  
- 审核：今天能过，明天就可能挂。  
- iOS / Android 表现完全不同？正常现象。  
- 模拟器：**我骗你，但我不说**。  

---

## 📂 仓库结构 / Repository Structure

```bash
.
├── docs/           # 避坑文档（Markdown）
├── examples/       # 小程序 & uni-app 示例（可选）
├── screenshots/    # 踩坑截图
└── README.md
```
## 🛠 如何贡献 / How to Contribute

欢迎 PR！如果你也踩过坑，别自己默默流泪，来一起写进来吧。
PRs are welcome! If you’ve stepped on a landmine, don’t cry alone — share it here.

## 📜 License
MIT License.
毕竟吐槽也要自由 😏。
