# ThopBlog

ThopBlog is a simple and informative blog website where I share detailed write-ups based on my YouTube videos. The blog covers topics like tech, HomeLab setups, and server management, providing step-by-step explanations to help readers easily follow along.

## Features
- Blogs based on YouTube videos
- Step-by-step tutorials on HomeLab and servers

## Installation
To run this project locally:

```sh
# Clone the repository
git clone https://github.com/yourusername/thopblog.git

# Navigate to the project folder
cd thopblog

# Start Hugo server
hugo server --disableFastRender
```

The site will be available at `http://localhost:1313`.

## Deployment
To deploy your Hugo site, you can use:
- Netlify
- Vercel
- GitHub Pages

---

# ThopBlog - Markdown Cheat Sheet

## Headings
```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

## Bold & Italic
```markdown
**Bold Text**  
*Italic Text*  
***Bold and Italic***
```

**Bold Text**  
*Italic Text*  
***Bold and Italic***

## Lists
### Unordered List
```markdown
- Item 1
- Item 2
  - Subitem 1
  - Subitem 2
```
- Item 1
- Item 2
  - Subitem 1
  - Subitem 2

### Ordered List
```markdown
1. First item
2. Second item
   1. Subitem 1
   2. Subitem 2
```
1. First item
2. Second item
   1. Subitem 1
   2. Subitem 2

## Links
```markdown
[Link Text](https://example.com)
```

## Images
```markdown
![Alt Text](https://example.com/image.png)
```

## Code Blocks
```markdown
Inline code: `code here`

Code block:
```javascript
console.log("Hello World");
```
```

## Blockquotes
```markdown
> This is a blockquote.
```
> This is a blockquote.

## Tables
```markdown
| Header 1 | Header 2 |
|-----------|------------|
| Data 1    | Data 2     |
| Data 3    | Data 4     |
```
| Header 1 | Header 2 |
|-----------|------------|
| Data 1    | Data 2     |
| Data 3    | Data 4     |

## Horizontal Line
```markdown
---
```
---

## Task List
```markdown
- [x] Completed task
- [ ] Incomplete task
```
- [x] Completed task
- [ ] Incomplete task

## Emojis
```markdown
:smile: :rocket: :tada:
```
:smile: :rocket: :tada:

## Footnotes
```markdown
Here is a reference[^1].

[^1]: This is the footnote.
```
Here is a reference[^1].

[^1]: This is the footnote.

---