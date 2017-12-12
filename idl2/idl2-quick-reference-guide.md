|                   |                                          |
| ----------------- | ---------------------------------------- |
| Heading 1         | `# Heading 1`                            |
| Heading 2         | `## Heading 2`                           |
| Heading 3         | `### Heading 3`                          |
| Heading 4         | `#### Heading 4`                         |
| Heading 5         | `##### Heading 5`                        |
| Heading 6         | `###### Heading 6`                       |
| **bold**          | `**bold**` or `__bold__`                 |
| *Italic*          | `*italic*` or `_italic_`                 |
| ~~Strikethrough~~ | `~~strikethrough~~`                      |
| Bullet            | `-`                                      |
| Task Checkbox     | `[ ]`                                    |
| Page break        | `===`                                    |
| Horizonal Line    | `---` or `***` or `___`                  |
| Block quote       | `> text to display in block quote`       |
| Escape character  | `\escaped text\`                         |
| Indent size       | `equal to 4 spaces`                      |
| Copyable Text     | `++copyable text++`                      |
| Image             | `![text to display](url)`                |
| Video             | `!VIDEO[text to display](url)`           |
| Image with link   | `[![text to display]url or filepath "Optional image title")]url "Optional link title")` |
| Knowledge         | `> [!KNOWLEDGE] ## Knowledge blocks help students learn more` |
| Alert             | `> [!ALERT] Alert blocks draw attention to important issues!` |
| Replacement Token | `Click the @lab toolbar button or type "@lab." in your idl-md editor window.` |
| Internal link     | `[text to display](#link-location "optional link title")` |
| External link     | `[text to display](url "optional link title)` |
| Relative link     | `[text to display](../folder/file.htm "optional link title")` |
| Inline code block | <code>`code block`</code>                |
---
Fenced code block
~~~Fenced_code_block
​```PowerShell
get-service | stop-service -whatif
​```
~~~
---
Reference links
```Text_lookup
[Reference link]
[Reference link]: URL "Optional link title"
```
```Label_lookup
[Reference link][Name of URL]
[Name of URL]: URL "Optional link title"
```
```Footnote_style
[Reference link][1]
[1]: URL "Optional link title"
```
---
Lists **without** checkboxes:       
```Unordered_List
- Item 1
    - Item 1.1
        - Item 1.1.1
        - Item 1.1.2
    - Item 1.2
- Item 2
```
```Ordered_List
1. Item 1
    1. Item 1.1
        1. Item 1.1.1
        1. Item 1.1.2
    1. Item 1.2
1. Item 2
```
---

Lists **with** checkboxes

```Unordered_List
- [] Item 1
    - [] Item 1.1
        - [] Item 1.1.1
        - [] Item 1.1.2
    - [] Item 1.2
- [] Item 2
```

```Ordered_List
1. [] Item 1
    1. [] Item 1.1
        1. [] Item 1.1.1
        1. [] Item 1.1.2
    1. [] Item 1.2
1. [] Item 2
```

---
Sample table:
```
| column 1 | column 2 |
| -------- | -------- |
| data 1   | data 2   |
| data 3   | data 4   |
```
