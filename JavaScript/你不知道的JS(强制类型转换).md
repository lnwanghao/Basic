## 宽松相等和严格相等

> 宽松相等(loose equals) `==` 和严格相等(strict equals) `===` 都用来判断两个值是否“相等”,但是它们之间有一个很重要的区别,特别是在判断条件上。

> 常见的误区是 `==` 检查值是否相等, `===` 检查值和类型是否相等”。听起来蛮有道理,然而还不够准确。很多 JavaScript 的书籍和博客也是这样来解释的,但是很遗憾他们都错了。

> 正确的解释是:“ `==` 允许在相等比较中进行强制类型转换,而 `===` 不允许。”

## 安全运用隐式强制类型转换

> • 如果两边的值中有 `true`或者 `false`,千万不要使用 `==` 。
> • 如果两边的值中有 `[]`、 `""`或者 `0`,尽量不要使用 `==` 。最好用 `===` 来避免不经意的强制类型转换。
