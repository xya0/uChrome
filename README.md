# uChrome
Chrome(ungoogled-chromium) 便携版本



## 简介

ungoogled-chromium 是基于 Chromium 的衍生版本，其剥离了所有来自 Google 的网络服务组件，进一步屏蔽 Google 内置于浏览器中的各种数据收集行为。



## 特性

- 关闭浏览器左上角 "搜索标签页" 按钮
- Chrome++功能：双击关闭标签页、鼠标悬停标签栏时使用滚轮切换标签页等等
- 解决Ungoogled Chromium无法安装拓展的问题，允许直接从 Chrome Web Store 安装扩展程序
- 安装 [“停用 Google Analytics（分析）”](https://chrome.google.com/webstore/detail/google-analytics-opt-out/fllaojicojecljbmefodhfapmkghcbnh?hl=zh_CN) 浏览器插件，不向 Google Analytics（分析）提供您的网站活动数据。

- 集成crxMouse（支持鼠标手势）、iTab新标签页、沉浸式翻译、OneSearch（书签搜索Ctrl + B）等插件
- 修改为在无痕模式下阻止第三方 Cookie（ungoogled-chromium 在默认情况下，关闭浏览器时会清除所有网站的 Cookie）



## 步骤

制作基于 Ungoogled Chromium 的便携版浏览器可以通过 Chrome++ 工具实现。以下是详细的实现步骤：

### 1. 准备工作
- **下载 Ungoogled Chromium**：从 [Ungoogled Chromium 官方仓库](https://github.com/ungoogled-software/ungoogled-chromium-windows) 获取最新版本。
- **下载 Chrome++**：从 [Chrome++ 项目页面](https://github.com/Bush2021/chrome_plus) 获取最新版本。

### 2. 解压文件

- 新建一个本地空文件夹 `uChrome`，用于存放应用程序。

- 将Chrome++中x64下的所有文件夹解压到 `uChrome`，

- 将 Ungoogled Chromium的压缩包解压到`uChrome/App`目录。

### 3. 配置 Chrome++（可选）
- 进入APP目录，找到 `chrome++.ini` 文件，用文本编辑器打开，根据需求修改配置。

### 4. 创建启动脚本
- 在目录中新建一个批处理文件（如 `start.bat`），本项目使用的是 [RunningCheeseChrome](https://www.runningcheese.com/chrome) 中的脚本

### 5. 运行便携版
- 双击 `start.bat` 生成 Chrome 的快捷方式，点击即可启动便携版 Ungoogled Chromium。

### 6. 测试及打包
- 检查浏览器功能是否正常，确保配置生效。将整个目录打包成 ZIP 或 7z 文件，便于分享和移动。

