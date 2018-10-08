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

##padStart()、padEnd()
  表示根据第一个参数，自动补全字符串的长度
    's'.padStart(2,'k') //"ks" 在字符串s头部补全
    's'.padEnd(2,k) //"sk"  在字符串s尾部补全
  如果省略第二个参数表示自动补全“空格”
     's'.padStart(5) //"    s"
     

