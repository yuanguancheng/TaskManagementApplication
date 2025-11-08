# 任务管理应用 (Task Management Application)

一个基于 React 的现代化任务管理应用，支持任务添加、完成状态切换、删除和过滤功能。

## 功能特性

- ✅ 添加新任务
- ✅ 标记任务完成/未完成
- ✅ 删除任务
- ✅ 任务过滤（全部/进行中/已完成）
- ✅ 数据本地持久化（localStorage）
- ✅ 响应式设计
- ✅ PWA 支持

## 技术栈

- React 19.2.0
- React Hooks
- CSS3
- Webpack (via Create React App)
- GitHub Pages (部署)

## 可用脚本

在项目目录中，你可以运行：

### `npm start`

在开发模式下运行应用。\
打开 [http://localhost:3000](http://localhost:3000) 在浏览器中查看。

页面会在你做出更改时重新加载。\
你可能会在控制台中看到任何 lint 错误。

### `npm test`

在交互式监视模式下启动测试运行器。\
有关运行测试的更多信息，请参阅 [running tests](https://facebook.github.io/create-react-app/docs/running-tests)。

### `npm run build`

将应用构建到 `build` 文件夹以进行生产。\
它正确地将 React 打包到生产模式中，并优化构建以获得最佳性能。

构建被压缩，文件名包含哈希值。\
你的应用已准备好部署！

### `npm run deploy`

构建应用并部署到 GitHub Pages。\
此命令会自动运行 `predeploy` 脚本（构建应用），然后使用 `gh-pages` 部署到 GitHub Pages。

### `npm run eject`

**注意：这是一个单向操作。一旦 `eject`，你就无法返回！**

如果你对构建工具和配置选择不满意，可以随时 `eject`。此命令将从你的项目中删除单个构建依赖项。

相反，它会将所有配置文件（webpack、Babel、ESLint 等）和传递依赖项复制到你的项目中，以便你可以完全控制它们。除了 `eject` 之外的所有命令仍然有效，但它们将指向复制的脚本，因此你可以调整它们。此时，你需要自己负责。

你不需要使用 `eject`。精选的功能集适用于小型和中型部署，你不应该觉得有义务使用此功能。但是，我们理解如果你在准备好时无法自定义它，这个工具将不会有用。

## GitHub Pages 部署指南

### 前提条件

1. 确保项目已推送到 GitHub 仓库
2. 在 GitHub 仓库设置中启用 GitHub Pages

### 部署步骤

1. **安装依赖**（如果尚未安装）：
   ```bash
   npm install
   ```

2. **部署到 GitHub Pages**：
   ```bash
   npm run deploy
   ```

3. **配置 GitHub Pages**：
   - 进入你的 GitHub 仓库
   - 点击 "Settings" 选项卡
   - 在左侧菜单中找到 "Pages"
   - 在 "Source" 下拉菜单中选择 "gh-pages" 分支
   - 点击 "Save"

4. **访问你的应用**：
   - 你的应用将部署在：`https://[你的用户名].github.io/[仓库名]`

### 手动部署（如果需要）

如果自动部署失败，可以手动执行以下步骤：

```bash
# 1. 构建应用
npm run build

# 2. 创建并切换到 gh-pages 分支
git checkout --orphan gh-pages

# 3. 添加构建文件
git --work-tree build add --all

# 4. 提交更改
git --work-tree build commit -m "Deploy to GitHub Pages"

# 5. 推送到远程仓库
git push origin gh-pages

# 6. 切换回主分支
git checkout -f main
git branch -D gh-pages
```

## 了解更多

你可以在 [Create React App 文档](https://facebook.github.io/create-react-app/docs/getting-started) 中了解更多信息。

要学习 React，请查看 [React 文档](https://reactjs.org/)。

### 代码分割

此部分已移至：[https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### 分析包大小

此部分已移至：[https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### 制作渐进式 Web 应用

此部分已移至：[https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### 高级配置

此部分已移至：[https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### 部署

此部分已移至：[https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` 压缩失败

此部分已移至：[https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
