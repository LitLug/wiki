# 格式风格

!!! secondary "本章部分引用自 [Linux101](https://101.ustclug.org/)，在此表示感谢。"

## 标题 {#title}

全文标题请使用 H1 等级标题书写

```maarkdown
# 格式风格
```

!!! danger "警告"

    全文**有且仅有一个** H1 等级标题

## 正文 {#main-content}

我们使用了 Markdown 语法来进行 Wiki 的编写，因此我们需要对 Markdown 的语法格式进行一些规范。

章节里的主要内容都应该写在主体里。主体包括标题和正文：标题都从 H2 等级以下按层次编写，而正文则直接使用普通文本即可。

每一段主体应当有完整的内容、正确的逻辑和通顺的文字。请尽力避免诸如知识点依赖链缺失、逻辑错误和文笔零碎等影响读者阅读体验的问题。建议每次写完以后通过想象自己正是读者进行阅读的方式来查漏补缺，也可以通过同行交叉审阅的方式获取宝贵的建议。

!!! tip "H2 等级，即指 Markdown 中使用两个`#`号的标题等级。样例： `## 这是 H2 等级的标题`"

!!! quote "中文排版指北"

    我们建议你使用 Prettier 来使你的排版更加美观。当然，熟记[《中文文案排版指北》](https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-Hans.md){:target="_blank"}是必须的

### 超链接 {#hyperlinks}

我们强烈要求你在所有链接后添加 `{:target="_blank"}` 标签，使读者能在新的页面打开链接而不会破坏原先阅读体验。

!!! example "范例"

    :fontawesome-solid-circle-xmark:{: .orangered } **错误**格式：

    ```markdown
    [Wiki@LitLUG](//litlug.wiki)
    ```

    :fontawesome-solid-circle-check:{: .limegreen } **正确**格式：

    ```markdown
    [Wiki@LitLUG](//litlug.wiki){:target="_blank"}
    ```

### 代码块 {#codeblock}

请注意代码块的写法与高亮设定是否正确，如表示一行**独立的**代码，请使用多行代码块并设定正确的语法高亮

!!! example "范例"

    :fontawesome-solid-circle-xmark:{: .orangered } **错误**格式：

    ```markdown
    `cd /usr/local`
    ```

    :fontawesome-solid-circle-check:{: .limegreen } **正确**格式：

    ```markdown

     ```bash
        cd /usr/local
     ```

    ```

### 提示框 {#admonitions}

通常来说，主体要包含的内容如果需要写得很详尽，不免会带来主次不分的问题。因为很多知识点的结构很接近有向无环图，而文字毕竟都是线性的。非要说使用拓扑排序虽然可以保证不会出现知识点依赖编写颠倒的问题，但也难以让读者快速分析出主干和枝节。

请善用提示框，让读者对内容的主次、成分一目了然，也能让你的作品层次更加丰富。

!!! info "重点"

    建议用这种提示框来划出重要的知识点，可以是一段内容的核心总结。

    使用形如 `!!! info "重点"` 的方式添加一个重点框。

!!! example "范例"

    建议用这种提示框来列出一个范例。

    使用形如 `!!! example "范例"` 的方式添加一个范例框。

!!! tip "小知识"

    建议用这种提示框来在保留正文连贯性的同时添加细枝末节的知识。

    使用形如 `!!! tip "小知识"` 的方式添加一个小知识框。

    **注意：请勿拼写为 tips，否则格式会被识别为提示（note）框。**

!!! warning "请在提示框的标题行后面留一个空行"

    由于 Prettier 的解析方式问题，请在所有提示框的起始行后面添加一个空行，**不要像 Material 主题官网那样没有空行直接开始提示框内容**。

    :fontawesome-solid-circle-xmark:{: .orangered } **错误**格式：

    ```markdown
    !!! note
        提示框内容
    ```

    :fontawesome-solid-circle-check:{: .limegreen } **正确**格式：

    ```markdown
    !!! note

        提示框内容
    ```

更多种类的提示框请参考 [提示框一览](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)。

### 永久链接 {#permalink}

由于 MkDocs 只支持英文字符自动生成 Anchor ID 的功能，纯中文的标题会导致生成 `\_1`, `\_2` 这样的 ID。一方面这样的 ID 看起来不直观，另一方面每当标题发生增减时这些 ID 都会变，因此请为每个标题手动添加一个有意义的 ID（最开始的标题 H1 除外），方法如下：

```markdown
### 永久链接 {#permalink}
```

!!! warning "警告 1"

    `{#` **前面**需要有一个空格。
    ```markdown
    ✅ ### 永久链接 {#permalink}
    ❌ ### 永久链接{#permalink}
    ```

    出于风格一致性考虑，请不要在 `{#` **后面**加空格：

    ```markdown
    ✅ ### 为标题和小标题添加 ID {#heading-ids}
    ❌ ### 为标题和小标题添加 ID {# heading-ids}
    ```

!!! warning "警告 2"

    请不要在每页最开始的标题（唯一一个 H1）后添加 `{#id-tag}`，否则可能会出现一些意料之外的显示错误。

## 贡献 {#contribute}

我们欢迎您访问 Wiki 的 [Github 仓库](https://github.com/LitLug/wiki/){:target="\_blank"}来帮助我们修改和提升 [Wiki@LitLUG](//litlug.wiki) 的内容质量。

总的来说，你需要进行以下操作：

1. [Fork 本仓库](https://github.com/LitLug/wiki/fork)
2. 对即将修改的内容进行认领
3. 在你 Fork 后的仓库中进行修改
4. 提交 Pull Requests 并等待合并
5. 完成

## 更多自有样式

如果你发现自己使用 Markdown 语法无法实现与其他文章一样的效果，不妨查看一下那篇文章的源代码或使用 `F12` 打开开发者工具来了解更多。

!!! quote "Yurik 碎碎念"

    我们很推荐你在不会使用效果时直接复制你想参考的区块，这很方便。
