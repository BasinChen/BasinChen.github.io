---
title: Page With Sidebar
subtitle: A demo page with a sidebar
layout: page
show_sidebar: true
---

This is a demo page showing the sidebar.

To show the sidebar set show_sidebar to true in the page's frontmatter.

```yml
title: Page With Sidebar
subtitle: A demo page with a sidebar
layout: page
show_sidebar: true
```
## Problem of TeX code editor display Chinese PDF garbled

### Description
Some times, we use TeX Studio or other editor to coding TeX, the PDF view Chinese is garbled, like this:

![garbled](garbled.PNG)

Code:
```
\documentclass{article}
\usepackage{ctex}
\begin{document}
	你好
\end{document}
```
### Solution
Solve PDF Chinese display garbled in Texstudio problem:
Other editors is similar.

1. Change the **compiler** in the Menu Bar.
If the editor is TeXstudio:
Click ```options```then, ```configure TeXstudio``` , ```build```, select Default compiler ```XeLaTeX``` 
![configure](configure.PNG)

2. Click ```Build & View``` again.

![garbled2](garbled2.PNG)

Code:
```
\documentclass{article}
\usepackage{ctex}
\begin{document}
	你好
\end{document}
```