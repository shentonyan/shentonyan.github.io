---
layout: post
title: "如何发布一篇新博客"
date: 2026-03-02 09:00:00 +0800
author: Shenton Yan
tags: [guide, jekyll, blogging]
---

每次想发布新博客，只需按照以下步骤操作即可。

## 第一步：创建新的 Markdown 文件

在 `_posts/` 目录下新建一个文件，文件名必须严格遵循以下格式：

```
YYYY-MM-DD-文章标题（英文，单词之间用短横线连接）.md
```

**示例：**

```
_posts/2026-04-15-my-new-article.md
```

---

## 第二步：添加 Front Matter（文章头部信息）

每篇文章的开头必须包含以下内容（用 `---` 包裹）：

```markdown
---
layout: post
title: "你的文章标题"
date: 2026-04-15 10:00:00 +0800
author: Shenton Yan
tags: [标签1, 标签2]
---
```

| 字段 | 说明 |
|------|------|
| `layout` | 固定填 `post`，不要改 |
| `title` | 文章标题，用引号包裹 |
| `date` | 发布日期和时间（`+0800` 表示北京时间） |
| `author` | 作者名，可选 |
| `tags` | 标签列表，可选，用方括号包裹，逗号分隔 |

---

## 第三步：写正文内容

Front Matter 之后，用 [Markdown 语法](https://www.markdownguide.org/basic-syntax/) 写正文即可。

**常用 Markdown 语法速查：**

```markdown
# 一级标题
## 二级标题

**加粗文字**
*斜体文字*

- 无序列表项
- 另一项

1. 有序列表项
2. 另一项

[链接文字](https://example.com)

![图片描述](图片链接)

> 引用文字

`行内代码`

​```python
# 代码块
print("Hello, World!")
​```
```

---

## 第四步：提交并推送到 GitHub

文件写好后，将其提交到 GitHub 仓库，GitHub Pages 会自动构建并发布。

**使用 Git 命令行：**

```bash
git add _posts/2026-04-15-my-new-article.md
git commit -m "Add new blog post: my-new-article"
git push
```

**或者直接在 GitHub 网页上操作：**

1. 打开 [https://github.com/shentonyan/shentonyan.github.io](https://github.com/shentonyan/shentonyan.github.io)
2. 进入 `_posts/` 目录
3. 点击右上角的 **「Add file」→「Create new file」**
4. 按照上述命名规则填写文件名
5. 粘贴 Front Matter 和正文内容
6. 点击页面底部 **「Commit changes」** 即可发布

---

## 小贴士

- 文件名中的日期必须和 Front Matter 中的 `date` 字段保持一致。
- 文章发布后可通过 `/blog/` 页面查看。
- 单篇文章的永久链接格式为：`/blog/YYYY/MM/DD/文章标题/`
