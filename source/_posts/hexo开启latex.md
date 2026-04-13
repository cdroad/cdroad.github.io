---
title: hexo开启latex
date: 2026-04-14 01:08:53
tags:
mathjax: true
---

一、在博客根目录新建

```js
_config.next.yml

math:
  enable: true
  per_page: true
  mathjax:
    enable: true
    src: https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
  katex:
    enable: false

```

二、在文章顶部加上

```markdown
title: 测试公式
date: 2026-04-12 13:30:00
mathjax: true   # 👈 就加这行
---
这里写公式 $E=mc^2$

```

三、运行

```shell
hexo clean
hexo g
hexo s
```

