# 知识库文件管理系统（KBMS）

基于 B/S 架构的企业级知识库文件管理系统，支持多用户、角色权限管理、文件/文件夹管理、标签分类等功能。

## 技术栈

| 层次 | 技术 |
|------|------|
| 后端 | Java / Spring Boot |
| 数据库 | MySQL 8.0+ |
| 文件存储 | 本地文件系统 |
| 前端 | Vue.js 3 + Element Plus |
| 认证 | JWT（Access + Refresh Token） |
| 文件打包 | ZIP4J / Apache Commons Compress |
| 密码加密 | BCrypt |
| 数据库迁移 | Flyway / Liquibase |

## 核心功能

- **用户管理** — 注册/登录、JWT 无状态认证、多设备同时在线、存储配额管理
- **文件管理** — 上传/下载/重命名/移动/软删除、单文件及批量下载（ZIP 打包）、文件冲突检测
- **文件夹管理** — 树形多层级目录、创建/重命名/移动、面包屑导航
- **标签系统** — 自定义标签、中英文混合命名、按标签筛选文件
- **管理员功能** — 查看所有用户文件、配置文件扩展名白名单、配置初始文件夹模板、用户管理、操作审计日志

## 角色权限

| 角色 | 权限 |
|------|------|
| 超级管理员 (ADMIN) | 管理所有用户文件、系统配置、用户账户、操作日志 |
| 普通用户 (USER) | 仅管理自己的文件、文件夹和标签 |

## 项目结构

```
knowledge-base-management-system/
├── docs/
│   └── kbms-srs.docx          # 软件需求规格说明书（SRS）
├── backend/                     # Spring Boot 后端（待开发）
│   ├── src/main/java/
│   └── pom.xml
├── frontend/                    # Vue.js 前端（待开发）
│   ├── src/
│   └── package.json
├── sql/                         # 数据库脚本（待开发）
│   └── schema.sql
└── README.md
```

## 文档

- [软件需求规格说明书（SRS）](docs/kbms-srs.docx)

## License

MIT
