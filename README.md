# Docker Compose Stacks for Portainer

本仓库用于存储 Docker Compose 配置文件，配合 Portainer GitOps 部署使用。

## 目录结构

```
compose/
└── npm/           # NPMplus (Nginx Proxy Manager Plus)
    ├── compose.yml
    └── stack.env
```

## Portainer 部署

1. 在 Portainer 中创建新 Stack
2. 选择 "Repository" 方式
3. 填入本仓库 URL
4. Compose path: `compose/npm/compose.yml`
5. 根据需要配置环境变量

## 注意事项

- 部署前请修改 `stack.env` 中的 `DATA` 路径
- 确保 `ACME_EMAIL` 已设置为有效邮箱
