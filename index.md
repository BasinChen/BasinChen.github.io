# Mathematics Programming Lover

## SinChen Blog

This is my first Blog page, welcone to [Math](gre_math).

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text
Code:
`  import time
Queen_n = 8#皇后数量
queens = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]#保存所有皇后的位置
QueenSolution_n = 0#有多少解
def IsConlict(now):#当前是第now个皇后,一个皇后占一行，所以它是第几个皇后也就表示，这个皇后在第几行
    for x in range(0,now):#在同一对角线，在同一斜对角线，在同一列上
        if (((x - now) == (queens[x] - queens[now])) or ((x - now) == -(queens[x] - queens[now])) or (queens[x] == queens[now])):
            return True#冲突
    return False
def nQueens():
    i=0
    while i<Queen_n:
        while (IsConlict(i) or queens[i] >= Queen_n):
            queens[i]+=1
            if queens[i]>=Queen_n:
                if queens[0]>=Queen_n:#越界结束
                    return
                queens[i]=0
                i-=1
                queens[i]+=1
                i-=1
        if i==Queen_n-1:
            queens[i]=0
            i-=1
            queens[i]+=1
            global QueenSolution_n
            QueenSolution_n+=1
            i-=1
        i+=1    
 
time0=time.clock()
nQueens()
print(Queen_n, "皇后问题有",QueenSolution_n,"种解,用时" ,int((time.clock()-time0)*1000),"ms")`


[Image1](pic1.jpg)

[Link](url) and ![Image](src)
```
[Image1](pic1.jpg)
For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/BasinChen/BasinChen.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
