> 主观观点：从上至下，由差到好 :3

| **包管理工具** | **准备工作** | **依赖统一管理** | **添加本地子项目为依赖** | **注意点** |
| --- | --- | --- | --- | --- |
| yarn2 | 配置 `workspaces` 字段 | ✅ 默认支持 | ⚠️ 支持（使用的是 yarn2 的 workspace 协议） | - yarn2 自身可用性和稳定性尚待确认 |
| yarn | 配置 `workspaces` 字段 | ⚠️  默认不支持（需要关闭 `nohoist` ） | ⚠️ 支持（但第一次添加时需要添加版本号） | - 不支持子项目为依赖 <br> - bug 较多，官方不怎么维护了 |
| npm | 配置 `workspaces` 字段 | ⚠️ 默认支持（子项目需要通过专门的指令） | ✅ 原生支持 | - 起步较晚，需要很新版本的 npm |
| pnpm | 添加 `pnpm-workspace.yaml` 文件 | ✅ 默认支持 | ⚠️ 支持（使用的是 pnpm 的 workspace 协议） | - 好使 👍 |
