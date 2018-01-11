# Markdown User Guide

Markdown is an easy to use markup language to format text, that offers multiple ways to achieve the same result. Markdown was designed to be easy to learn as well as be easy to read and write. Markdown allows the author to keep their hands on the keyboard and focus on writing content. Markdown supports HTML, and HTML syntax can be used in combination with Markdown.

## Table of Contents 

1. [Headings](#1.-Headings)
2. [Text formatting](#2.-Text-formatting)
3. [Link formatting](#3.-Link-Formatting)
4. [Page formatting](#4.-page-formatting)
5. [Embedded content](#5.-embedded-content)
6. [List formatting](#6.-List-formatting)
7. [Table formatting](#7.-Table-formatting)
8. [Special formatting](#8.-Special-formatting)

## 1. Headings

Markdown allows for text to be resized by typing 1-6 # (hash or pound) symbols in front of the text that is to be resized, followed by a space. One # renders the largest text size, while six # symbols renders the smallest text size.Typically this is used at the beginning of a paragraph or section in a document, to make the title stand out from the rest of the text. 
> - # H1 
> - ## H2    
> - ### H3    
> - #### H4
> - ##### H5
> - ###### H6

## 2. Text Formatting

- **Indent size**: pressing the tab key will indent 4 spaces.

- **Single space**: pressing the tab key at the end of a line will single space the next line. Alternatively, pressing the space bar four times will single space the next line. 

- **Double space:** leaving no spaces at the end of the line will double space the next line. 

- **Bold**: used to show emphasis. Type two * (asterisk) symbols on each side of the text that is to be bolded.

  > \**Bold text**

- **Italic**: used to show emphasis or distinction. Type two _ (underline) on each side of text that is to be emphasized.

  > \_Italic text_

- **~~Strikethrough~~**: used to mark text that should not be included, but should not be removed from the document. Type two ~ (tilde) symbols on each side of text that should show a strikethrough.

  > \~~Strikethrough text~~ 

- **Escape character**: used to prevent text from being formatted into Markdown. Type a \ (backslash) at the beginning of the text that is to be escaped. 

  > \escaped text

- **Bullet**: used to separate and order  items in a list without using numbers

  > `-`

- **Inline code block**: used to provide a snippet of code that can be copied and pasted. Type a ` (backtick) on each side of the text that is to be displayed in the code block. The backtick is located above the tab key, to the left of the 1 key on the keyboard.

 > <code>`code block`</code> 

- **Fenced code block**: used to provide a programming language-specific code snippet. Type three ` (backticks) on each side of the text that should be displayed in the fenced code block. This should consume at least 3 lines in the text editor; the first line should display three backticks followed by the programming language name, the second line should display the code snippet, and the last line should only display three backticks. Markdown allows for more than one line to be used to display the code snippet. 

> ~~~Fenced_code_block
> ​```PowerShell
> get-service | stop-service -whatif
> ​```
> ~~~

## 3. Link formatting

- **Internal link**: Used to link to a specific section within a document. 
  > \[text to display](#link-location "optional link title")

- **External link**: Used to link to a page outside of the document.  

  > \[text to display](url "optional link title)

- **Relative link**: used to link to a page in the same directory without the need to display the full URL of the page.

  > \[text to display](../folder/file.htm "optional link title")

- **Reference link**: used to provide a link that will be referenced multiple times. The link can be referenced by typing the text value between the [ ] (square brackets). It is not necessary to include the full URL, as long as the text value in both sets of brackets is the same.   

  - **_Text lookup_**: 
    > \[Reference link text value]
    > \[Reference link text value]: URL "Optional link title"
  - **_Label lookup_**:
    > \[Reference link][Name of URL]
    > \[Name of URL]: URL "Optional link title"
  - **_Footnote style_**:
    > \[Reference link][1]
    > \[1]: URL "Optional link title"

 ## 4. Page formatting

- **Page break**: Used to separate content into pages. Separating into pages creates a next button that the student must click to navigate to the next page. This is useful for displaying small sections of instruction to the student at a time, rather than all instructions on the same page within the lab. Type three = (equals) symbols on the line where the current page should end. The new page will begin on the line following the three = symbols.

  > ===

- **Horizontal Line**: Used to separate content on the same page. Type three --- (dash or hyphen) on the line where the horizontal line should appear. 

  > \---

- **Block quote:** Used to quote information from other sources. Block quote text appears indented from other content in the document. Type a > (greater-than sign) before text that should appear in the block quote. Most Markdown syntax will render inside of block quotes.

    > \> text here
    >
    > \> additional text 
    >
## 5. Embedded content

- **Image**: Used to embed an image inline with other content. 

  > \![text to display]\(url)

- **Video:** Used to embed an image inline with other content. The syntax format should look the same as an image, except the video should begin with a ! (explanation mark), followed by the word VIDEO (all caps).

  > \!VIDEO[text to display]\(url)

- **Image with link:** Used to embed an image that can be clicked to navigate to a specific URL (internal or external). 

  > \[![text to display]url or filepath "Optional image title")]url "Optional link title")

- **Portal Link:** used to launch a hyperlink. In the Cloud Client, this will open the hyperlink in the left window. In the traditional virtualization client (vm-based labs), this will open the hyperlink in a new local browser window.

  > `!PORTALLINK[text to display](URL)`

- **Image Link:** used to display a link with a camera icon, to suggest that the hyperlink opens an image

  > `!IMAGELINK[text to display](URL to image)`

- **Video Link:** used to display a link with a videocamera icon, to suggest that the hyperlink opens a video

  > `!VIDEOLINK[text to display](URL to video)`

## 6. List formatting

- **Unordered list:** Used to list items in no particular order, separated by bullets rather than numbers. Type a - (dash or hyphen) followed by a space and then the text to be listed. Pressing enter at the end of the text will start the next line with a bullet. 

- **Ordered list:** Used to list items in a particular order, separated by numbers rather than bullets. Type the number 1, followed by a space and then the text to be listed. Pressing enter at the end of the text will start the next line with number 2.

- Both Unordered and Ordered lists can contain checkboxes for the learner to check off steps as completed. Both list types can be combined in the same list. 

 ### Unordered list **without** checkboxes: 
```- Item 1
    - Item 1.1
        - Item 1.1.1
        - Item 1.1.2
    - Item 1.2
- Item 2
```
### Ordered list **without** checkboxes:
```1. Item 1
    1. Item 1.1
        1. Item 1.1.1
        1. Item 1.1.2
    1. Item 1.2
1. Item 2
```
### Unordered list **with** checkboxes:
```Unordered_List
- [] Item 1
    - [] Item 1.1
        - [] Item 1.1.1
        - [] Item 1.1.2
    - [] Item 1.2
- [] Item 2
```

### Ordered list **with** checkboxes:
```Ordered_List
1. [] Item 1
    1. [] Item 1.1
        1. [] Item 1.1.1
        1. [] Item 1.1.2
    1. [] Item 1.2
1. [] Item 2
```

## 7. Table formatting
- Tables can be aligned left, right or center by placing a : (colon) on the head row of the table. Placing a colon on the left side, right side or both sides of the dashes in the header row, will align the text in the table accordingly. 

**Left-aligned text**

```
| column 1 | column 2 |
|:---------|:---------|
| data 1   | data 2   |
| data 3   | data 4   |
```

**Right-aligned text**
```
| column 1 | column 2 |
|---------:|---------:|
| data 1   | data 2   |
| data 3   | data 4   |
```

**Center-aligned text**
```
| column 1 | column 2 |
|:--------:|:--------:|
| data 1   | data 2   |
| data 3   | data 4   |
```

## 8. Special formatting 

- **Knowledge Block:** Used to provide additional information, to help students better understand lab steps or lab content. Knowledge blocks are limited to only show 4 lines of the lab content. After 4 lines, a _more_ link will be shown, allowing the student to expand the Knowledge Block and review additional information.

  > \> [!KNOWLEDGE] knowledge text here.

- **Alert:** Used to draw attention to important issues, such as showing additional information or steps that the student may need complete to avoid other issues. 

  > \> [!ALERT] alert text here.

- **Note:** used to provide additional information, similar to a Knowledge Block, with the only difference being that Notes do not collapse and show a _more_ link to expand the section. 

  > [!NOTE]

- **Include:**  used to input text from a GitHub raw link. This is useful to use to pull in content hosted on GitHub. Navigate to the GitHub page containing the content to be used, click the Raw button, then copy the URL of that page and include it in the below syntax. 

  **Note**: GitHub hosted content can be changed by the repo maintainer of the content and will change the instructions displayed in the lab using the _Include_ syntax. 

  >  `[!INCLUDE [label](url)]`

- **Copyable Text:** used to make text copy to the local clipboard when the student clicks the text. Type two + (plus) symbols on each side of the text that should be made copyable. 

  > \++copyable text++

- **Embed YouTube video:** used to embed a YouTube video inline with the lab instructions. URLs from YouTube.com automatically embed. Videos from any other URL will not embed.

  > `!VIDEO[text to display](url)` 



- **Replacement Token:** used to replace text in lab instructions with a variable that is unknown at the time of authoring the lab instructions. These variables may not be generated or created until the lab is launched by the student. These can include usernames, user first name, user last name, running lab instance ID number, etc. 
  > | Replacement token           |                                          |
  > | --------------------------- | ---------------------------------------- |
  > | @lab.LabInstanceId          | The unique ID of the running lab instance. |
  > | @lab.GlobalLabInstanceId    | The globally unique ID of the running lab instance. |
  > | @lab.LabProfileId           | The unique ID of the lab profile.        |
  > | @lab.UserId                 | The unique ID of user running the lab.   |
  > | @lab.UserFirstName          | The first name of the user running the lab. |
  > | @lab.UserLastName           | The last name of the user running the lab. |
  > | @lab.UserEmail              | The e-mail address of the user running the lab. |
  > | @lab.UserExternalId         | The external ID of the user running the lab (if launched via API). |
  > | @lab.Tag                    | The tag associated with the lab instance (if specified when launched via API). |
  > | @lab.CloudPortalLink        | A link to the cloud portal.              |
  > | @lab.CloudPortalUrl         | The cloud portal URL (rendered as text, not a link). |
  > | @lab.CloudPortalSignInLink  | A cloud portal sign-in link.             |
  > | @lab.CloudPortalSignInUrl   | The cloud portal sign-in URL (rendered as text, not a link). |
  > | @lab.CloudPortalSignOutLink | A cloud portal sign-out link.            |
  > | @lab.CloudPortalSignOutUrl  | The cloud portal sign-out URL (rendered as text, not a link). |

---
