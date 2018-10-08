#ES6比较常用的各种方法
```markdown
## includes()、startsith()、endsWith()
以上方法与JavaScript中的indexOf相似，但以上方法返回的布尔值(并且查找的时候区分大小写)。
  eg:
    let t="Welcome ES6";
    t.includes("ES") //true 表示是否在字符串“t”中找到字符串“ES”
    t.startsidth("W") //true 表示查找的字符串是否在“t”的头部
    t.endsWidth("6")  //true 表示查找的字符串是否在“t” 的尾部。
 
  当然以上三个方法也支持第二个参数，前两个方法加上第二个参数都表示从n个索引位置开始查找
      eg：includes("ES,n) / startsith("W",n)
          endsWith("6",9) 表示字符串6之前都有9个字符

## repeat()
  该方法返回一个新的字符串，并且重复了n次该字符串（不能为负数否则会报错）
  's'.repeat(2) //"ss"
  's'.repeat(0) //""
  's'.repeat(0.5) //"" 正数都会向下取整，负数如果小于0到-1之间会报错

## padStart()、padEnd()
  表示根据第一个参数，自动补全字符串的长度
    's'.padStart(2,'k') //"ks" 在字符串s头部补全
    's'.padEnd(2,k) //"sk"  在字符串s尾部补全
  如果省略第二个参数表示自动补全“空格”
     's'.padStart(5) //"    s"

## Number.parseInt()、Number.parseFloat()、Number.isInteger()
  前两个方法和JavaScript中的parseInt()、parseFloat()极其相似，isInteger()判断是否为一个整数
  eg:
  Number.isInteger() // false
  Number.isInteger(null) // false
  Number.isInteger('15') // false
  Number.isInteger(true) // false
  
## Math.trunc()
  返回小数的整数部分（类似于 / 取整操作）
  Math.trunc(2.1) //2
  Math.trunc(2.8) //2
  
  Math.trunc(-2.1) //2
  Math.trunc(-2.8) //2
  注：如果参数是字符串、空、undefined等等一律返回NAN

## Math.sign()
  该方法用来判断一个数是正数、负数、零。
  返回值：正数（+1）、负数（-1）、【0（0） / -0(-0)】、其他一律返回NAN
  
  Math.sign(-5) // -1
  Math.sign(5) // +1
  Math.sign(0) // +0
  Math.sign(-0) // -0
  Math.sign(NaN) // NaN
  
## Math.cbrt()
  计算一个数的立方根
  Math.cbrt(8) //2
  Math.cbrt(-8) //-2
  注：如果参数是字符串、空、undefined等等一律返回NAN
  
## Math.imul()
  该方法返回一个乘积（并且是32位的，包含符号）
  Math.imul(2,6) //12
  Math.imul(-2,6) //-12
  注：如果输入的是小数无论正负都向下取整（Math.floor()）
  Math.imul(2,6.5) //12
  Math.imul(0.2,6)  //0

## Math.hypot()
  返回所有参数平方和的平方根
  eg:
    Math.hypot(3,4) //9+16=25  5
    Math.hypot(3,4,5) //9+16+25=50  7.0710678118654755
  注：无论多少个参数，只要参数中出现不是数值的字符串（“sfs”），一律返回NAN,如果是数值字符串（“5”）会自动转化成数值在计算。
  
# 函数扩展
  ```markdown
