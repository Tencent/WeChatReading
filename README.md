# 微信读书 Skills

为 AI Agent 提供微信读书能力的 Skill 集合，支持搜书、书架管理、笔记导出、阅读统计等功能。

## 安装

```bash
npx skills add Tencent/WeChatReading -g
```

## 配置

使用前需要设置微信读书 API Key：

1. 前往 [https://weread.qq.com/r/weread-skills](https://weread.qq.com/r/weread-skills) 获取你的 API Key
2. 设置环境变量：

```bash
export WEREAD_API_KEY=wrk-xxxxxxxx
```

> API Key 绑定用户身份，所有需要用户身份的接口会自动注入，无需手动传入。

## 使用

安装后直接用自然语言与 Agent 对话即可：

```
"帮我搜一下三体"
"看看我的书架"
"我这个月读了多久"
"导出我在这本书里的划线"
"给我推荐几本书"
"这本书有什么热门划线"
"三体有什么点评"
```

## 功能

| 能力 | 说明 | 详细文档 |
|------|------|----------|
| 搜索书籍 | 书城搜索，支持电子书/有声书/网文/作者/全文等类型 | [`search.md`](skills/search.md) |
| 书籍信息 | 书籍详情、章节目录、阅读进度 | [`book.md`](skills/book.md) |
| 书架管理 | 查看书架（电子书 + 有声书 + 文章收藏） | [`shelf.md`](skills/shelf.md) |
| 笔记划线 | 笔记概览、划线内容、个人想法、热门划线 | [`notes.md`](skills/notes.md) |
| 阅读统计 | 阅读时长、天数、排行、偏好分析 | [`readdata.md`](skills/readdata.md) |
| 书籍点评 | 公开点评浏览与筛选 | [`review.md`](skills/review.md) |
| 推荐发现 | 个性化推荐、相似书推荐 | [`discover.md`](skills/discover.md) |

## 版本

当前版本：**1.0.6**

每次请求自动携带版本号，服务端会通过 `upgrade_info` 字段通知升级。

## 许可证

[Apache-2.0](./LICENSE) — Copyright © 2026 Tencent
