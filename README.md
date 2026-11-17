# 更加适配的superpowers

这是基于 [Superpowers](https://github.com/obra/superpowers) 7.0.1 的 Codex 定制版。仓库包含插件清单、15 个技能及其参考资料。

## 主要改动

- `using-superpowers` 仅在显式调用时启动。明确、可逆的小改动可以直接实现和验证。
- 设计讨论用于仍有重要取舍的任务。普通多步任务采用简短计划，复杂迁移或交接可使用正式计划。
- 保留系统化调试和交付验证。优先复用现有测试，有明确的回归缺口时补充测试。用户或项目要求测试先行时采用 TDD。
- 默认由主代理执行。按任务需要和授权安排独立评审、委派及 worktree 隔离。

## 在 Codex 中使用

将本仓库克隆到本地。仓库根目录就是插件目录，包含 `.codex-plugin/plugin.json` 和 `skills/`。将这个目录加入 Codex 的个人或项目 marketplace，再从桌面端安装。切换到这个定制版时，关闭原版可避免同时加载两套同名技能。

[Codex 本地插件安装说明](https://developers.openai.com/plugins/build/plugins#install-a-local-plugin-manually)

## 许可证

基于 Jesse Vincent 的 [Superpowers](https://github.com/obra/superpowers) 项目发布。详见 [MIT 许可证](LICENSE)。
