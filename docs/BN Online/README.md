# BetterNemo Online

BetterNemo 的 Web 版本，无需安装即可在浏览器中编辑和运行 BN 作品。

## 访问

在线地址：**[https://hhcl233.github.io/betternemo-online/](https://hhcl233.github.io/betternemo-online/)**

## 功能特性

### 文件操作
- **新建作品** — 创建一个默认示例作品
- **打开 .json 作品** — 加载本地 JSON 格式的 BCM 作品文件
- **打开 .bcmbn 作品** — 加载本地 BCMBN 压缩包格式作品（包含素材资源）
- **下载 .json / .bcmbn** — 保存当前作品到本地

### 编辑器功能
- **积木编辑** — 通过 iframe 嵌入 BN 原生 workspace，支持完整的积木编程体验
- **角色查看** — 切换视图查看作品角色列表
- **JSON 编辑器** — 内置 Monaco Editor，可直接编辑作品的原始 JSON 数据
- **运行/暂停** — 一键切换作品运行状态
- **编辑器 UI 类型** — 支持在 Pad/手机模式间切换

### 账号系统
- **编程猫账号登录** — 支持通过编程猫账号登录
- **离线模式** — 无需登录即可使用基础功能
- **用户信息查看** — 登录后可查看昵称、性别、UID

### 扩展管理
- 打开 `.bcmbn` 作品时自动检测扩展冲突
- 支持选择使用本地版本或从远程下载扩展
- 预设加载 [FastSet] 扩展

### 其他功能
- **作品重命名** — 修改作品名称
- **修改作品 ID** — 启用云功能（需作品 JSON 与云端一致）
- **主题色自定义** — 可自由调整编辑器主题色
- **Q&A 帮助** — 内置常见问题解答

## 使用说明

### 新建作品
点击菜单 `文件 → 新建作品`，会加载一个默认的"摇一摇大黄鸡"示例作品。

### 打开作品
- **JSON 格式**：点击 `文件 → 打开作品 → 打开 .json 作品`，选择本地的 `.json` 文件
- **BCMBN 格式**：点击 `文件 → 打开作品 → 打开 .bcmbn 作品`，选择本地的 `.bcmbn` 压缩包

### 保存作品
- `.json` 格式：点击 `文件 → 下载 .json 作品`
- `.bcmbn` 格式（含素材）：编辑含有素材的作品后，点击 `文件 → 下载 .bcmbn 作品`

### 登录账号
1. 点击 `账号 → 登录`
2. 输入编程猫账号和密码
3. 登录后可访问云端作品和社区功能

### 离线模式
启用离线模式可跳过登录，使用本地功能。
点击 `账号 → 启用离线模式` 即可。

## 本地部署

```bash
git clone https://github.com/BetterNemo-Team/betternemo-online.git
cd betternemo-online
npm install
npm run dev
```

## 技术栈

- **前端框架**：Vue 3 + TypeScript
- **构建工具**：Vite 8
- **UI 组件库**：mdui 2
- **代码编辑器**：Monaco Editor
- **路由**：Vue Router (Hash History)
- **状态管理**：Pinia

## 注意事项

- BN Online 使用的 BetterNemo 经过修改，不建议手动更新版本
- 如遇 Bug，请直接在 betternemo-online 项目提交 Issue
- 若 Bug 在原版 BetterNemo 中也存在，开发者会引导前往原仓库提交
