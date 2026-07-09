## 项目目标

这个仓库用于维护 Ai路人的 IP 插画 / 配图 Codex Skill。
当前目标是维护 Ai路人自己的 IP 形象、画风规则、prompt 模板、示例说明和验收标准。

## 目录约定

- `README.md`：GitHub 对外说明、安装方式、使用示例和展示图。
- `NOTICE.md`：来源、署名和改编说明。保留原作者 attribution，不直接删除。
- `examples/`：对外示例 prompt 和展示图片。
- `ailuren-illustrations/`：当前可安装的 Codex Skill 主目录。
- `ailuren-illustrations/SKILL.md`：Skill 触发描述、工作流和默认规则入口。
- `ailuren-illustrations/references/`：IP、画风、构图、prompt 模板和 QA 检查清单。
- `ailuren-illustrations/agents/openai.yaml`：Skill 在 Codex / OpenAI 环境中的展示配置。

## 命名规则

- Skill 调用名统一使用 `ailuren-illustrations`。
- 替换 IP 或改动规则时，必须同步检查上游旧关键词残留。`NOTICE.md` 和 `LICENSE` 中的原作者 attribution 可以保留。
- 新增图片、示例和文档文件使用小写英文、连字符命名，例如 `01-topic-name.png`。

## 验证命令

- 查看上游旧关键词残留：按需搜索 README、AGENTS、examples 和 `ailuren-illustrations/`，确认非 attribution 文件里没有旧项目名、旧角色名、旧调用名和旧资产名。

- 查看 Skill 关键文件：

```bash
rg --files ailuren-illustrations examples README.md NOTICE.md
```

- 本仓库目前没有构建脚本或自动测试；文档和规则修改后以关键词检查、文件路径检查、人工通读为主。

## 清理规则

- 不自动删除原作者署名、LICENSE、NOTICE 或示例图片；如需删除或替换，先列出范围并等待确认。
- 不覆盖已有示例图片；新图先另存为新文件，再决定是否替换 README 引用。
- 不修改 git 历史，不自动 push。
