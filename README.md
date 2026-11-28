# Corokia Workflow

展示原 Corokia 示例源码的 Respo 页面。原运行时解释器已经退役，页面保留示例入口。

## 使用者注意

使用 Calcit 和 `@calcit/procs` 0.47.1，以及配套的 Respo 0.20.1 和 Respo UI 0.16.7。更新后重新安装依赖并构建；Respo 更新可能导致样式差异。

```bash
corepack enable
yarn install --immutable
caps --strict --ci
caps verify --toolchain
calcit --check-only
calcit fix --workflow strict --verify
yarn build
```

源码使用 `calcit.cirru`，生成的 `js-out/` 和 `dist/` 不提交。主分支推送按原路径部署前端；PR 仅构建，不部署到主站。
