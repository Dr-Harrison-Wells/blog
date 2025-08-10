---
title: Fuwari 简要指南
published: 2025-08-09
description: "如何使用博客模板."
image: "./cover.jpeg"
tags: ["博客美化"]
category: 博客美化
draft: false
---

> 封面图源: [Source](https://image.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/208fc754-890d-4adb-9753-2c963332675d/width=2048/01651-1456859105-(colour_1.5),girl,_Blue,yellow,green,cyan,purple,red,pink,_best,8k,UHD,masterpiece,male%20focus,%201boy,gloves,%20ponytail,%20long%20hair,.jpeg)

博客模板使用[Astro](https://astro.build/)构建. 指南中未提及的部分，可以在[Astro Docs](https://docs.astro.build/)找到答案.

## 发布文章的Front-matter格式

```yaml
---
title: My First Blog Post
published: 2023-09-09
description: This is the first post of my new Astro blog.
image: ./cover.jpg
tags: [Foo, Bar]
category: Front-end
draft: false
---
```

| 属性     | 描述                                                                                                                                                                                                 |
|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `title`       | 文章的标题.                                                                                                                                                                                      |
| `published`   | 文章发布的日期.                                                                                                                                                                            |
| `description` | 文章的简述，在索引页面显示.                                                                                                                                                   |
| `image`       | 文章的封面图片路径.<br/>1. 使用网页图片，以`http://`或者`https://`开始。<br/>2. 对于在`public`下的图片，以`/`开始<br/>3. 没有前缀的，存放在相对md文件的路径 |
| `tags`        | 文章的标签.                                                                                                                                                                                       |
| `category`    | 文章的分类.                                                                                                                                                                                   |
| `draft`        | 如果文章是草稿，不会展示.                                                                                                                                                    |

## 文章该放在哪里

你的文章应该放在 `src/content/posts/`. 你也可以创建子文件夹来更好的组织你的文章和静态资源.

```
src/content/posts/
├── post-1.md
└── post-2/
    ├── cover.png
    └── index.md
```
