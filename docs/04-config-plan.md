# 配置管理方案

## 主要配置项
| 配置项 | 文件名 | 存放位置 |
|--------|--------|----------|
| 项目说明 | README.md | 根目录 |
| 项目概况 | overview.md | docs/ |
| WBS文档 | wbs.md | docs/ |
| 进度计划 | schedule.md | docs/ |
| 配置管理文档 | configuration-management.md | docs/ |
| 冲突示例 | conflict.md | docs/ |
| 总结报告 | final-report.md | docs/ |
| 源代码 | *.py / *.js / 其他 | src/ |

## 分支策略

## 分支规则
- **main分支**：受保护，禁止直接推送，只能通过PR从dev合并
- **dev分支**：日常开发集成，功能分支完成后合并至此
- **feature分支**：从dev切出，完成后删除

## 提交规则
- 提交信息格式：`<type>: <subject>`
- 合并前需确保通过简单测试

## 版本标记
- 使用tag标记版本：v1.0.0、v1.1.0

## 主分支保护
- 在GitHub Settings中设置main分支保护：
  - 要求PR审核
  - 要求状态检查通过
  - 禁止强制推送