# site-alcohol-culture

酒文化网站仓，部署地址 `culture.hejiu.org`。

- 正文来源：`world-alcohol-encyclopedia/culture/`
- 应用：`apps/site/`（Astro 静态生成，包名 `@hejiu/site-culture`）
- 共享工程：`site-alcohol-core` 的 `packages/ui`、`packages/build-tools`、`packages/contracts`

## 命令

在 `implementation/` 工作区运行：

```text
npm run build -w @hejiu/site-culture
npm run build:preview
npm run build:prod
```

构建钩子生成本站 Pagefind 索引、entity registry、release manifest 和已发布搜索记录。主站总搜索只读取这些已发布记录。

## 边界

- 本站只通过配置设置 key、host、强调色与领域内容；底栏、语言切换、主题、搜索组件由共享 UI 提供。
- 本站不复制其他站完整正文，只显示摘要、关系与主要地址。
- 当前为 G2 样本，不代表全量迁移或正式线上发布。
