## includes()、startsith()、endsWith()
```markdown
以上方法与JavaScript中的indexOf相似，但以上方法返回的布尔值(并且查找的时候区分大小写)。
  eg:
    let t="Welcome ES6";
    t.includes("ES") //true 表示是否在字符串“t”中找到字符串“ES”
    t.startsidth("W") //true 表示查找的字符串是否在“t”的头部
    t.endsWidth("6")  //true 表示查找的字符串是否在“t” 的尾部。
 
  当然以上三个方法也支持第二个参数，前两个方法加上第二个参数都表示从n个索引位置开始查找
      eg：includes("ES,n) / startsith("W",n)
          endsWith("6",9) 表示字符串6之前都有9个字符

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

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/LonelyAngul/ES6/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
