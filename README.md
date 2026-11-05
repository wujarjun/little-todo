# Little Todo · 轻待办

一件一件，慢慢完成。一个轻巧的中文待办清单，用一个 HTML 文件记录日常小事。

**无需安装、无需登录、没有第三方依赖。** 下载后双击 `index.html` 即可使用，也可以部署到 GitHub Pages。

## 功能

- 添加任务，支持回车快捷提交。
- 勾选完成，实时查看完成进度。
- 按全部、未完成、已完成筛选。
- 删除单个任务或清除已完成事项，支持撤销最近一次删除。继续添加任务或切换完成状态后，撤销记录会清空。
- 自动保存在当前浏览器，重新打开后恢复。
- 浅色 / 深色主题，首次打开跟随系统设置。
- 适配手机和电脑，支持键盘操作。

## 开始使用

1. 点击仓库页面的 **Code → Download ZIP**，解压。
2. 用 Chrome、Edge、Firefox 或 Safari 打开 `index.html`。
3. 写下一件小事，然后点击「添加」或按回车。

也可以使用本地静态服务器，例如已安装 Python 3 时，在项目目录执行：

```sh
python -m http.server 8000
```

然后访问 `http://localhost:8000`。

## 部署到 GitHub Pages

1. 将项目文件上传至公开仓库。
2. 打开仓库 **Settings → Pages**。
3. 在 **Build and deployment** 里选择 **Deploy from a branch**。
4. 选择 `main` 分支和 `/(root)` 目录，点击 **Save**。
5. 等待 GitHub 完成部署，页面会提供可访问的网址。

## 数据与隐私

- 任务保存在浏览器的 `localStorage`，不需要服务器，也不会主动上传任务。
- 不同浏览器、设备和网址之间的数据不会同步。直接打开本地文件时，保存行为由浏览器决定；需要稳定的存储来源时，可使用本地服务器或 GitHub Pages。
- 清除浏览器数据或使用隐私模式可能导致任务丢失，请勿把这里作为重要信息的唯一备份。
- 如果浏览器禁止存储或存储空间不足，页面会提示，仍可在本次打开期间使用。
- 同时打开多个标签页时不会实时同步，后保存的标签页可能覆盖之前的更改。

## 技术实现

原生 HTML、CSS 和 JavaScript，全部包含在 `index.html` 中。无需 Node.js、打包工具或外部字体。

任务文本通过 `textContent` 渲染，不作为 HTML 执行。

## 贡献

欢迎在 [Issues](https://github.com/wujarjun/little-todo/issues) 提出问题和改进建议，也欢迎提交 Pull Request。

## 许可证

[MIT](LICENSE) © 2026 wujarjun
