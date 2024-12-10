# Headings 

```md
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
# H1
## H2
### H3
#### H4
##### H5
###### H6

# Text Formatting

| Example                        | Output                            |
| ------------------------------ | --------------------------------- |
| `**bold**`                     | **bold**                          |
| `*italic*`                     | _italic_                          |
| `~~strike~~`                   | ~~strike~~                        |
| `==highlight==`                | ==highlight==                     |
| `x^2^`                         | x²                                |
| `H~2~O`                        | H₂O                               |
| `**bold and _nested italic_**` | **bold text and _nested italic_** |
| `***bold and italic***`        | ***bold and italic***             |
Formatting can be forced to display in plain text by adding a backslash `\` in front of it.

\*\*This line will not be bold\*\*
```md
\*\*This line will not be bold\*\*
```

\**This line will be italic and show the asterisks*\*
```md
\**This line will be italic and show the asterisks*\*
```

# Lists 

```md
- First list item
- Second list item
- Third list item
```

- First list item
- Second list item
- Third list item

```md
1. First list item
2. Second list item
3. Third list item
```

1. First list item
2. Second list item
3. Third list item

# Blockquotes

```md
> This is a blockquote.
```

> This is a blockquote.

# Horizontal Rule / Separator
```md
---
```

---

# Links & Images

| Syntax                    | Description         | Example                        |
| ------------------------- | ------------------- | ------------------------------ |
| `[Link Text](URL)`        | Hyperlink           | `[Google](https://google.com)` |
| `![Alt Text](Image URL)`  | Image               | `![Obsidian Logo](image.png)`  |
| `![[Internal Note Name]]` | Embed internal note | `![[MyNote]]`                  |
# Code 

### Inline code 
You can format code within a sentence using single backticks.

```md
Text inside `backticks` on a line will be formatted like code.
```

Text inside `backticks` on a line will be formatted like code.

### Code blocks 
To format a block of code, surround the code with triple backticks.

````md
```
cd ~/Desktop
```
````

```md
cd ~/Desktop
```

# Task lists 
To create a task list, start each list item with a hyphen and space followed by `[ ]`.
```md
- [x] This is a completed task.
- [ ] This is an incomplete task.
```

- [x] This is a completed task.
- [ ] This is an incomplete task.

# Footnotes 

You can add footnotes[^1] to your notes using the following syntax:
[^1]: This is the referenced text.

```md
This is a simple footnote[^1].

[^1]: This is the referenced text.
[^2]: Add 2 spaces at the start of each new line.
  This lets you write footnotes that span multiple lines.
[^note]: Named footnotes still appear as numbers, but can make it easier to identify and link references.
```

You can also inline footnotes in a sentence. Note that the caret goes outside the brackets.

```md
You can also use inline footnotes. ^[This is an inline footnote.]
```

# Tables

```md
| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Cell 1   | Cell 2   | Cell 3   |
| Cell 4   | Cell 5   | Cell 6   |
```

| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Cell 1   | Cell 2   | Cell 3   |
| Cell 4   | Cell 5   | Cell 6   |

# Escaping Markdown Syntax 

In some cases, you may need to display special characters in Markdown, such as `*`, `_`, or `#`, without triggering their formatting. To display these characters literally, place a backslash (`\`) before them.

Common characters to escape
- Asterisk: `\*`
- Underscore: `\_`
- Hashtag: `\#`
- Backtick: `` \` ``
- Pipe (used in tables): `\|`
- Tilde: `\~`

# Obsidian-Specific Features

- **Internal Links**: `[[Note Name]]`
    - Links to another note in your vault.
- **Backlinks**: Use the `[[ ]]` syntax in any note to automatically create backlinks.
- **Embeds**: Use `![[Note Name]]` to embed another note.
- **Tags**: Use `#` to create tags, e.g., `#task` or `#project`.
- **Callouts**:
```md
> [!NOTE]
> This is a callout box.
```

> [!NOTE]  
> This is a callout box.

- **Frontmatter** (YAML Metadata):
```yaml
---
title: My Note
tags: [example, obsidian]
created: 2024-12-01
---
```    
