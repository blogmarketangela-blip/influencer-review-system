# 红人资源审核系统 Skill

把 Excel、CSV 或粘贴的 Instagram 账号与邮箱名单交给 Codex，生成可运行的中文人工审核系统。支持任意品牌，无需原作者的聊天记录或历史文件。

## 使用方法

1. 下载本仓库的 `influencer-review-system.zip` 并解压，保留完整目录。
2. 将技能包和自己的账号名单一起提供给 Codex。
3. 输入：

```text
请读取技能包内的 SKILL.md，把附件名单生成可运行的红人审核系统。
```

名单建议包含 Instagram 主页链接或用户名、邮箱；国家、粉丝数和来源可选。仅有邮箱无法可靠定位 Instagram 账号。

也可把完整的 `influencer-review-system` 文件夹放入 Codex 的 skills 目录，安装后输入：

```text
$influencer-review-system 请把这份名单生成资源审核系统
```

## 审核功能

- 默认优先显示待审核资源，每页 50 条。
- 点击账号打开主页；单条通过、不通过、撤销。
- 当前页全选、多选、批量审核。
- 已审核资源从待审核列表中移除。
- 审核记录保存到本地文件，并支持 JSON 备份与恢复。
- 导出通过名单及全量 CSV；需要 Excel 时可要求 Codex 生成真实 XLSX。

## 运行要求

需要能够运行 Node.js 的 Codex 工作环境。服务只依赖 Node 内置模块，无需 npm install。支持 Windows、macOS 和 Linux；云端环境需使用其端口预览功能。

这是人工审核工具，不会仅凭导入名单就自动判断达人是否适合合作。公开技能包不包含实际达人名单、私人邮箱或历史审核记录。
