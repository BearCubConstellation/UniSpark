# UniSpark Starter项目目录结构,测试提交

## 目录概览

```
UniSpark/
├─ .cursor/                Cursor 配置
├─ .git/                   Git 仓库元数据
├─ .github/                GitHub 相关配置（如 CI）
├─ .husky/                 Git hooks
├─ .trae/                  Trae 相关配置
├─ .vscode/                VS Code 工作区配置
├─ env/                    环境变量文件
├─ node_modules/           依赖安装产物（可重新安装生成）
├─ scripts/                项目脚本
├─ src/                    业务源码
├─ vite-plugins/           自定义 Vite 插件
├─ .commitlintrc.cjs        Commitlint 配置
├─ .editorconfig            编辑器格式配置
├─ .gitignore               Git 忽略规则
├─ .npmrc                   npm/pnpm 配置
├─ eslint.config.mjs        ESLint 配置
├─ favicon.ico              站点图标
├─ index.html               入口 HTML
├─ LICENSE                  许可证
├─ manifest.config.ts       UniApp manifest 配置
├─ openapi-ts-request.config.ts  OpenAPI 代码生成配置
├─ package.json             项目信息与脚本
├─ pages.config.ts          页面路由配置
├─ pnpm-lock.yaml           依赖锁定文件
├─ README.md                项目说明
├─ tsconfig.json            TypeScript 配置
├─ uno.config.ts            UnoCSS 配置
└─ vite.config.ts           Vite 构建配置
```

## env（环境变量）
- `.env`：通用环境变量
- `.env.development`：开发环境
- `.env.test`：测试环境
- `.env.production`：生产环境

## scripts（脚本）
- `create-base-files.js`：初始化/生成基础文件
- `open-dev-tools.js`：开发工具相关脚本
- `postupgrade.js`：升级后处理脚本

## vite-plugins（自定义插件）
- `copy-native-resources.ts`：复制原生资源
- `sync-manifest-plugins.ts`：同步/处理 manifest 插件
- `README.md`：插件说明

## src（核心源码）

```
src/
├─ api/            接口定义
├─ components/     通用组件
├─ hooks/          组合式 hooks
├─ http/           网络请求封装
├─ layouts/        布局
├─ pages/          页面
├─ router/         路由封装
├─ service/        业务服务层
├─ static/         静态资源
├─ store/          状态管理
├─ style/          样式
├─ tabbar/         底部 TabBar 配置/资源
├─ types/          类型定义
├─ uni_modules/    uni-app 插件模块
├─ utils/          工具函数
├─ App.ku.vue      App 入口（KU 版本）
├─ App.vue         App 入口
├─ env.d.ts        Vite 环境类型
├─ main.ts         入口启动文件
├─ manifest.json   UniApp manifest（运行时）
├─ pages.json      UniApp pages（运行时）
├─ typings.d.ts    全局类型
├─ typings.ts      类型汇总
└─ uni.scss        全局样式变量
```

## 说明
- `node_modules/`、`pnpm-lock.yaml` 为依赖相关文件；生产环境可通过 `pnpm install` 重新生成。
- `manifest.config.ts` 与 `pages.config.ts` 通常用于生成 `manifest.json` 与 `pages.json`。
- `src/` 为核心业务目录，变更主要集中于此。
- Author：Cym
- Date：2026-02-02
- 说明：UniSpark（Uniapp 开发启动模板）基于 unibest 改动而来。


