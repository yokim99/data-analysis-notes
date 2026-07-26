# WorkBuddy 小程序 - GitHub 知识上传提示词

## 使用方法
复制下方提示词，把【要上传的内容】替换为你的实际内容，发送即可。

---

## 提示词

请帮我把以下内容上传到我的 GitHub 知识库。

### GitHub 配置
- 用户名：yokim99
- Token：【你的GitHub Personal Access Token，替换为你自己的】
- 默认分支：main

### 仓库映射表
| 内容类型 | 仓库 | 目录路径 | 可见性 |
|---------|------|---------|--------|
| 播客笔记 | yokim99/agent_learning | podcast-notes/ | 私有 |
| 读书笔记 | yokim99/agent_learning | 读书笔记/{书名}/ | 私有 |
| Skill技能 | yokim99/agent_learning | skills/{skill名}/ | 私有 |
| AI文章分析 | yokim99/ai-frontier-knowledge | 文章分析/ | 公开 |
| AI前沿知识 | yokim99/ai-frontier-knowledge | 前沿知识/ | 公开 |
| 职场经验 | yokim99/workplace-advancement | 按主题建子目录 | 公开 |
| 编程学习 | yokim99/yummy | 按日期或主题建子目录 | 公开 |
| 数据分析 | yokim99/data-analysis-notes | 按分类建子目录 | 公开 |

### 上传方法
使用 GitHub Contents API：
1. GET 检查文件是否存在（获取 sha）
2. 将内容 Base64 编码
3. PUT 上传（新文件不填 sha，更新文件必填 sha）

### 上传要求
1. 根据内容类型自动判断上传到哪个仓库和目录
2. 文件名要有意义，用中文命名
3. 格式为 Markdown
4. 上传后同步更新仓库 README.md 的索引表
5. 上传完成后告诉我：文件路径、访问链接
6. 私有仓库的内容提醒我其他人看不到

### 要上传的内容

【在这里粘贴你的内容】
