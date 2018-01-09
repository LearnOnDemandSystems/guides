<a href="https://learnondemandsystems.github.io/guides/idl2/markdown-user-guide.html" style="float:right;" title="A full user guide to authoring labs in IDL-flavored markdown.">Markdown User Guide</a>

| | |
| ------------------| ---------------------------------------- |
|<font size="4">**Headings:**</font> | |
| Heading 1 | `# Heading 1` |
| Heading 2 | `## Heading 2` |
| Heading 3 | `### Heading 3` |
| Heading 4 | `#### Heading 4` |
| Heading 5 | `##### Heading 5` |
| Heading 6 | `###### Heading 6` | 
|<br> | |
|<font size="4">**Text Formatting:**</font>| |
| Indent size | `equal to 4 spaces` |
| **bold** | `**bold**` or `__bold__` |
| *Italic* | `*italic*` or `_italic_` |
| ~~Strikethrough~~ | `~~strikethrough~~` |
| Escape character | `\escaped text\` |
| Bullet | `-` |
|<BR> | |
|<font size="4">**Link Formatting:**</font>| |
| Internal link | `[text to display](#link-location "optional link title")` |
| External link | `[External link](URL "Optional link title")` |
| Relative link | `[text to display](../folder/file.htm "optional link title")` | 
|<BR> | |
 |<font size="4">**Page Formatting**</font>    |                                          |
| Page break        | `===`                                    |
| Horizonal Line    | `---` or `***` or `___`                  |
| Block quote       | `> text to display in block quote`       |
|<BR> | |
 |<font size="4">**Embedded Content:**</font>|                                          |
| Image             | `![](url)`                               |
| Video             | `!VIDEO[text to display](url)`           |
| Image with link   | `[![image description](URL of image "image description")](URL to open when image is clicked)`    |
| Portal Link       |  `!PORTALLINK[text to display](URL)`     | 
| Image Link        |  `!IMAGELINK[text to display](URL to image)`| 
| Video Link        |  `!VIDEOLINK[text to display](URL to video)`| 
|<BR> | |
 |<font size="4">**Special Formatting:**</font>|                                          |
| Knowledge         | `> [!KNOWLEDGE] ## Knowledge blocks help students learn more` |
| Alert             | `> [!ALERT] Alert blocks draw attention to important issues!` |
| Note              | `> [!NOTE]`                              |
| Include           | `[!INCLUDE [label](url)]`                |
| Copyable Text     | `++copyable text++`                      |
| Replacement Token | `Click the @lab toolbar button or type "@lab." in your idl-md editor window.` |
| Embed YouTube video | `!VIDEO[text to display](url)` (URLs from YouTube.com auto embed)               |
|<BR> | |
 
**Code Blocks**

Inline code block  <code>`code block`</code>   

Fenced code block
~~~Fenced_code_block
​```PowerShell
get-service | stop-service -whatif
​```
~~~
---
**Reference links**

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
**List Formatting**

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
**Sample table**

Left aligned text
```
| column 1 | column 2 |
|:---------|:---------|
| data 1   | data 2   |
| data 3   | data 4   |
```

Right aligned text
```
| column 1 | column 2 |
|---------:|---------:|
| data 1   | data 2   |
| data 3   | data 4   |
```

Center aligned text
```
| column 1 | column 2 |
|:--------:|:--------:|
| data 1   | data 2   |
| data 3   | data 4   |
```



