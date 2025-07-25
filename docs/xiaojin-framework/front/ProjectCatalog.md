# 前端项目架构

## 项目整体结构

```
├── apps/          # 应用程序目录
    ├── base       # 基座项目，负责继承所有子应用
├── packages/      # 共享包目录
├── utils/         # 公共工具类
├── package.json   # 工作空间配置
└── turbo.json     # Turborepo配置
```

## 主应用(base)结构

```
├── index.html     # 项目html模板
├── vite.config.js # vite配置信息
├── index.html     # 项目html模板
├── index.html     # 项目html模板
├── public         # 静态资源文件
└── src            # 源代码目录
    ├── assets
    ├── components
    ├── layout
    ├── router
    └── views

```