# JavaScriptNotesForProfessionals
### 第一章节 JavaScript 入门

#### 1.1章节 使用console.log()

#### 1.2章节 使用DOM API

DOM 代表文档对象模型。他是面向对象表示结构化文档（如 XML 和 HTML）

在网页上输出文本的方法是设置元素的 textContent 属性。

例如，思考下面的 HTML标签

```html
<p id="paragraph"></p>
```

可以运行下面的 JavaScript ，改变它的 textContent 属性。

```javascript
document.getElementById("paragraph").textContent = "Hello, World";
```

这将选择 id 为 paragraph 的元素并设置文本的内容为 "Hello, World"：
```html
<p id="paragraph">Hello, World</p>
```

你也可以使用 JavaScript 以编程的方式创建新的 HTML 元素。例如，思考具有下面 body 的 HTML 文档：

```html
<body>
<h1>Adding an element</h1>
</body>
```

在 JavaScript 中，我们创建具有 textContent 属性的新 `<p>`标签并添加到 html body 尾部。

```javascript
var element = document.createElement('p');
element.textContent = "Hello, World";
document.body.appendChild(element);
```

这将 HTML body 更改为以下内容：

```html
<body>
<h1>Adding an element</h1> 
<p>Hello, World</p>
</body>
```

请注意，为了使用 JavaScript 操作 dom 中的元素，必须在文档中创建了相关的元素之后运行 JavaScript 代码。这可以将 JavaScript `<script>` 标签放在所有其他 `<body>` 内容之后。或者你也可以使用事件侦听器侦听，例如 将你的代码添加到 window 的 onload 事件里面，代码会等到页面上的全部内容加载完才执行。

确保所有的 DOM 都已加载的第三种方法是使用 setTimeout 函数包裹 DOM操作的代码。这样， JavaScript 代码会在执行队列的末尾排队，从而使浏览器有机会完成一些非 JavaScript 的事情。JavaScript 代码会一直等待着。

#### 1.3章节 使用window.alert()

#### 1.4章节 使用window.prompt()

#### 1.5章节 使用window.confirm()

#### 1.6章节 使用DOM API（使用图形文本：Canvas、SVG或图像文件）

### 第二章节 JavaScript变量

#### 2.1章节 定义变量

#### 2.2章节 使用变量

#### 2.3章节 变量的类型

#### 2.4章节 数组和对象

### 第三章节 内置常量

#### 3.1章节 null

#### 3.2章节 使用isNaN()测试NaN

#### 3.3章节 NaN

#### 3.4章节 undefiend和null

#### 3.5章节 Infinity和-Infinity

#### 3.6章节 Number常量

#### 3.7章节 返回NaN的操作

#### 3.8章节 返回NaN的Math函数

### 第四章节 注释

#### 4.1章节 使用注释

#### 4.2章节 在JavaScript中使用HTML注释（不好的做法）

### 第五章节 Console控制台

#### 5.1章节 测量时间-console.time()

#### 5.2章节 格式化console的输出

#### 5.3章节 打印到浏览器的调试控制台

#### 5.4章节 记录包含堆栈跟踪 -  console.trace（）

#### 5.5章节 制表数值

#### 5.6章节 计数 - console.count()

#### 5.7章节 清空控制台 - console.clear()

#### 5.8章节 以交互方式显示对象和XML - console.dir(), console.dirxml()

#### 5.9章节 使用断言进行调试 - console.assert()

### 第六章节 JavaScript中的数据类型

#### 6.1章节 typeof

#### 6.2章节 寻找对象的class

#### 6.3章节 通过构造函数名称获得对象类型

### 第七章节 字符串Strings

#### 7.1章节 基本信息和字符串连接

#### 7.2章节 反转字符串

#### 7.3章节 按字典顺序比较字符串

#### 7.4章节 访问字符串中索引处的字符

#### 7.5章节 转义引号

#### 7.6章节 单词计数器

#### 7.7章节 Trim去除空格

#### 7.8章节 将字符串拆分为数组

#### 7.9章节 字符串为Unicode

#### 7.10章节 检测字符串

#### 7.11章节 带切片的子串

#### 7.12章节 字符二进制码

#### 7.13章节 数字Numbers的字符串表示

#### 7.14章节 字符串查找和替换的方法

#### 7.15章节 在字符串中查找子字符串的索引

#### 7.16章节 字符串变大写

#### 7.17章节 字符串变小写

#### 7.17章节 字符串重复

### 第八章节 日期Date

#### 8.1章节 创建日期对象

#### 8.2章节 转换为字符串格式

#### 8.3章节 从UTC创建日期

#### 8.4章节 格式化JavaScript日期

#### 8.5章节 获取自1970年1月1日00:00:00 UTC以来起经过的毫秒数

#### 8.6章节 获取当前时间和日期

#### 8.7章节 递增日期对象

#### 8.8章节 转换为JSON

### 第九章节 日期比较

#### 9.1章节 比较日期的值

#### 9.2章节 日期差异计算

### 第十章节 比较运算

#### 10.1章节 抽象等式/不等式与类型转换

#### 10.2章节 全局对象的NaN属性

#### 10.3章节 布尔运算符中的短路

#### 10.4章节 Null和Undefined

#### 10.5章节 抽象等式(==)

#### 10.6章节 具有布尔值的逻辑运算符

#### 10.7章节 自动类型转换

#### 10.8章节 具有非布尔值的逻辑运算符(布尔强制)

#### 10.9章节 空数组

#### 10.10章节 相等比较运算

#### 10.11章节 关系运算符(<，<=，>=)

#### 10.12章节 不等式

#### 10.13章节 比较运算符列表

#### 10.14章节 对多个逻辑语句进行分组

#### 10.15章节 位字段，用于优化多状态数据的比较

### 第十一章节 条件

#### 11.1章节 三目运算符

#### 11.2章节 Switch语句

#### 11.3章节 if/else if/else控制

#### 11.4章节 策略

#### 11.5章节 使用||和&&短路

### 第十二章节 数组

#### 12.1章节 将类数组对象转换为数组

#### 12.2章节 Reducing的值

#### 12.3章节 Mapping的值

#### 12.4章节 过滤对象数组

#### 12.5章节 排序数组

#### 12.6章节 迭代器Iteration

#### 12.7章节 解构数组

#### 12.8章节 删除重复元素

#### 12.9章节 数组比较

#### 12.10章节 反转数组

#### 12.11章节 浅克隆一个数组

#### 12.12章节 浅克隆一个数组

#### 12.13章节 将两个数组合并为键值对

#### 12.14章节 数组展开/剩余

#### 12.15章节 数组过滤值

#### 12.16章节 搜索数组

#### 12.17章节 将字符串转换为数组

#### 12.18章节 从数组中删除项目

#### 12.19章节 删除所有元素

#### 12.20章节 查找最小或最大元素

#### 12.21章节 标准数组初始化

#### 12.22章节 将数组元素连接到字符串中

#### 12.23章节 使用splice()删除/添加元素

#### 12.24章节 entry()方法

#### 12.25章节 从数组中删除值

#### 12.26章节 展平数组

#### 12.27章节 将项目追加/前置到数组

#### 12.28章节 要数组的对象键和值

#### 12.29章节 值的逻辑连接词

#### 12.30章节 检查对象是否为数组

#### 12.31章节 将项插入到特定索引处的数组中

#### 12.32章节 排序多维数组

#### 12.33章节 测试所有数组项是否相等

#### 12.34章节 复制数组的一部分

### 第十三章节 对象

#### 13.1章节 浅拷贝

#### 13.2章节 对象冻结Object.freeze

#### 13.3章节 对象克隆

#### 13.4章节 对象属性迭代

#### 13.5章节 Object.assign

#### 13.6章节 Object rest/spread 

#### 13.7章节 Object.defineProperty

#### 13.8章节 访问属性(Get和Set)

#### 13.9章节 动态/可变属性名称

#### 13.10章节 数组是对象

#### 13.11章节 Object.seal

#### 13.12章节 将对象的值转换为数组

#### 13.13章节 从对象中检索属性

#### 13.14章节 只读属性

#### 13.15章节 不可枚举属性

#### 13.16章节 锁定属性描述

#### 13.17章节 Object.getOwnPropertyDescriptor

#### 13.18章节 描述符和命名属性

#### 13.19章节 Object.keys

#### 13.20章节 具有特殊字符或保留字的属性

#### 13.21章节 创建一个Iterable对象

#### 13.22章节 迭代对象条目 -  Object.entries（）

#### 13.23章节 Object.values()

### 第十四章节 算术(数学)

#### 14.1章节 常量

#### 14.2章节 余数/模数(%)

#### 14.3章节 四舍五入

#### 14.4章节 三角

#### 14.5章节 按位运算符

#### 14.6章节 递增（++）

#### 14.7章节 求幂(Math.pow()或**)

#### 14.8章节 随机整数和浮点数

#### 14.9章节 加法(+)

#### 14.10章节 使用按位运算符时，类型数组的小/大字节序

#### 14.11章节 获取两个数字之间的随机数

#### 14.12章节 模拟不同概率的事件

#### 14.13章节 减法(-)

#### 14.14章节 乘法（*）

#### 14.15章节 获取最大值和最小值

#### 14.16章节 将数字限制为最小/最大范围

#### 14.17章节 向上取整和向下取整

#### 14.18章节 得到一个数字的根

#### 14.19章节 具有高斯分布的随机数

#### 14.20章节 Math.atan2寻找方向

#### 14.21章节 Sin＆Cos创建一个给定方向和距离的向量

#### 14.22章节 Math.hypot

#### 14.23章节 使用Math.sin的周期函数

#### 14.22章节 除法（/）

#### 14.22章节 递减（--）

### 第十五章节 按位运算符

#### 15.1章节 按位运算符

#### 15.2章节 移位运算符

### 第十六章节 构造函数

#### 16.1章节 声明构造函数

### 第十七章节 声明及赋值

#### 17.1章节 修改常量

#### 17.2章节 声明和初始化常量

#### 17.3章节 声明

#### 17.4章节 Undefined

#### 17.5章节 数据类型

#### 17.6章节 数学运算和赋值

#### 17.6章节 赋值

### 第十八章节 循环

#### 18.1章节 标准的for循环

#### 18.2章节 for ... of循环

#### 18.3章节 for ... in循环

#### 18.4章节 while循环

#### 18.5章节 继续循环

#### 18.6章节 中断特定的嵌套循环

#### 18.7章节 do ... while循环

#### 18.8章节 Break和continue标签

### 第十九章节 函数

#### 19.1章节 函数作用域

#### 19.2章节 函数柯里化

#### 19.3章节 立即调用的函数表达式

#### 19.4章节 命名函数

#### 19.5章节 绑定this和参数

#### 19.6章节 具有未知数量的参数的函数（可变函数）

#### 19.7章节 匿名函数

#### 19.8章节 默认参数

#### 19.9章节 Call和apply

#### 19.10章节 偏函数应用

#### 19.11章节 按引用或值传递参数

#### 19.12章节 函数参数，“参数”对象，REST剩余参数和展开参数

#### 19.13章节 复合函数

#### 19.14章节 获取函数对象的名称

#### 19.15章节 递归函数

#### 19.16章节 使用Return语句

#### 19.17章节 函数用作变量

### 第二十章节 JS函数式编程

#### 20.1章节 高阶函数

#### 20.2章节 同一Monad

#### 20.3章节 纯函数

#### 20.4章节 接受函数作为参数

### 第二十一章节 原型对象

#### 21.1章节 创建和初始化原型Prototype

### 第二十二章节 Classes类

#### 22.1章节 类构造函数

#### 22.2章节 类继承

#### 22.3章节 静态方法

#### 22.4章节 Getters and Setters

#### 22.5章节 私有成员

#### 22.6章节 方法

#### 22.7章节 动态方法名称

#### 22.8章节 使用类管理私有数据

#### 22.9章节 类名绑定

### 第二十三章节 命名空间

#### 23.1章节 通过直接赋值命名空间

#### 23.2章节 命名空间嵌套

### 第二十四章节 上下文（this）

#### 24.1章节 普通对象的this

#### 24.2章节 保存this以便在嵌套函数/对象中使用

#### 24.3章节 绑定函数上下文

#### 24.4章节 构造函数的this

### 第二十五章节 Setters and Getters

#### 25.1章节 使用Object.defineProperty定义Setter/getter

#### 25.2章节 在新创建的对象中定义Setter/getter

#### 25.3章节 在ES6类中定义getter和setter

### 第二十六章节 事件

#### 26.1章节 页面、DOM和浏览器加载

### 第二十七章节 继承

#### 27.1章节 标准函数原型

#### 27.2章节 Object.key and Object.prototype.key两者之间的区别

#### 27.3章节 原型继承

#### 27.4章节 伪古典继承

#### 27.5章节 设置对象的原型

### 第二十八章节 链式方法

#### 28.1章节 可链式对象设计和链式

#### 28.2章节 链式方法

### 第二十九章节 回调

#### 29.1章节 简单的回调用法示例

#### 29.2章节 延续(同步和异步)

#### 29.3章节 什么是回调

#### 29.4章节 回调和this

#### 29.5章节 使用箭头函数回调

#### 29.6章节 错误处理和控制流分支

### 第三十章节 Intervals and Timeouts

#### 30.1章节 递归setTimeout

#### 30.2章节 Intervals

#### 30.3章节 Intervals

#### 30.4章节 移除Intervals

#### 30.5章节 移除timeouts

#### 30.6章节 setTimeout，操作顺序，clearTimeout

### 第三十一章节 正则表达式

#### 31.1章节 创建一个RegExp对象

#### 31.2章节 RegExp标志

#### 31.3章节 使用.test（）检查字符串是否包含模式

#### 31.4章节 与.exec()匹配

#### 31.5章节 对字符串使用RegExp

#### 31.6章节 Regexp分组

#### 31.7章节 用回调函数替换字符串匹配

#### 31.8章节 使用带圆括号正则表达式的Regex.exec（）来提取字符串的匹配项

### 第三十二章节 Cookies

#### 32.1章节 测试是否启用了Cookie

#### 32.2章节 添加和设置Cookie

#### 32.3章节 读取Cookie

#### 32.4章节 删除Cookie

### 第三十三章节 网络存储

#### 33.1章节 使用localStorage

#### 33.2章节 更简单的存储处理方法

#### 33.3章节 存储事件

#### 33.4章节 sessionStorage

#### 33.5章节 localStorage长度

#### 33.6章节 错误条件

#### 33.7章节 清空存储

#### 33.8章节 删除存储项目

### 第三十四章节 Data属性

#### 34.1章节 访问data属性

### 第三十五章节 JSON

#### 35.1章节 JSON vs JavaScript文字

#### 35.2章节 使用reviver函数进行解析

#### 35.3章节 序列化一个值

#### 35.4章节 序列化和恢复类实例

#### 35.5章节 使用替换函数进行序列化

#### 35.6章节 解析简单的JSON字符串

#### 35.7章节 循环对象值

### 第三十六章节 AJAX

#### 36.1章节 通过POST发送和接收JSON数据

#### 36.2章节 添加Ajax预加载器

#### 36.3章节 通过Stack Overflow的API显示当月最热门的JavaScript问题

#### 36.4章节 使用带参数的GET

#### 36.5章节 通过HEAD请求检查文件是否存在

#### 36.6章节 使用没有参数的GET

#### 36.7章节 在全局级别侦听Ajax事件

### 第三十七章节 枚举

#### 37.1章节 使用Object.freeze（）定义枚举

#### 37.2章节 替代定义

#### 37.3章节 打印枚举变量

#### 37.4章节 使用Symbols实现枚举

#### 37.5章节 自动枚举值

### 第三十八章节 Map映射

#### 38.1章节 创建Map映射

#### 38.2章节 清空Map映射

#### 38.3章节 从Map映射中删除元素

#### 38.4章节 检查Map映射中是否存在键

#### 38.5章节 迭代Map映射

#### 38.6章节 获取和设置元素

#### 38.7章节 获取Map映射的元素数量

### 第三十九章节 时间戳

#### 39.1章节 高精度的时间戳

#### 39.2章节 以秒为单位获取时间戳

#### 39.3章节 低精度的时间戳

#### 39.4章节 支持旧版浏览器

### 第四十章节 一元运算符

#### 40.1章节 概述

#### 40.2章节 typeof操作符

#### 40.3章节 删除操作符

#### 40.4章节 一元加号运算符(+)

#### 40.5章节 void运算符

#### 40.6章节 一元否定运算符(-)

#### 40.7章节 按位NOT运算符（〜）

#### 40.8章节 逻辑NOT运算符（！）

### 第四十一章节 Generators

#### 41.1章节 Generator函数

#### 41.2章节 把值传给生成器

#### 41.3章节 委托给其他生成器

#### 41.4章节 迭代器

#### 41.5章节 带生成器的异步流

#### 41.6章节 迭代器-观察者接口

### 第四十二章节 Promises

#### 42.1章节 介绍Promise

#### 42.2章节 Promise的链式调用

#### 42.3章节 等待多个并发Promises

#### 42.4章节 数组Reduce()Promise的链式调用

#### 42.5章节 等待多个并发Promises中的第一个

#### 42.6章节 使用回调的“Promisiating”函数

#### 42.7章节 错误处理

#### 42.8章节 协调同步和异步操作

#### 42.9章节 延迟函数调用

#### 42.10章节 "Promisifying" 值

#### 42.11章节 使用ES2017 async / await

#### 42.12章节 使用final()执行清理

#### 42.13章节 forEach with promises

#### 42.14章节 异步API请求

### 第四十三章节 Set集合

#### 43.1章节 创建Set集合

#### 43.2章节 向Set集合添加值

#### 43.3章节 从Set集合中删除值

#### 43.4章节 检查Set集合中是否存在值

#### 43.5章节 清空Set集合

#### 43.6章节 获得Set集合长度

#### 43.7章节 将Set集合转换为数组

#### 43.8章节 Set集合中的交集和差异

#### 43.9章节 迭代Set集合

### 第四十四章节 模态框-Prompts提示

#### 44.1章节 关于用户提示

#### 44.2章节 持久提示模态框

#### 44.3章节 确认删除元素

#### 44.4章节 alert()的用法

#### 44.5章节 prompt()的用法

### 第四十五章节 模态框-Prompts提示

#### 45.1章节 监听内容可编辑的变化

#### 45.2章节 开始

#### 45.3章节 使用execCommand（“copy”）从textarea复制到剪贴板

#### 45.4章节 格式化

### 第四十六章节 History

#### 46.1章节 history.pushState()

#### 46.2章节 history.replaceState()

#### 46.3章节 从历史记录列表中加载特定的URL

### 第四十七章节 Navigator对象

#### 47.1章节 获取一些基本的浏览器数据并将其作为JSON对象返回

### 第四十八章节 BOM（浏览器对象模型）

#### 48.1章节 介绍

#### 48.2章节 Window对象属性

#### 48.3章节 Window对象方法

### 第四十九章节 事件循环

#### 49.1章节 Web浏览器中的事件循环

#### 49.2章节 异步操作和事件循环

### 第五十章节 严格模式

#### 50.1章节 对于整个脚本

#### 50.2章节 对于函数

#### 50.3章节 对属性的更改

#### 50.4章节 全局属性的更改

#### 50.5章节 重复参数

#### 50.6章节 严格模式下的函数作用域

#### 50.7章节 函数参数列表的行为

#### 50.8章节 非简单参数列表

### 第五十一章节 自定义元素

#### 51.1章节 扩展原生元素

#### 51.2章节 注册新元素

### 第五十二章节 数据操作

#### 52.1章节 将数字格式化为货币

#### 52.2章节 从文件名中提取扩展名

#### 52.3章节 在给定字符串名称的情况下设置对象属性

### 第五十三章节 二进制数据

#### 53.1章节 获取图像文件的二进制表示

#### 53.2章节 在Blob和ArrayBuffers之间转换

#### 53.3章节 使用DataViews操作ArrayBuffers

#### 53.4章节 从Base64字符串创建TypedArray

#### 53.5章节 使用TypedArray

#### 53.5章节 迭代arrayBuffer

### 第五十四章节 模板文字

#### 54.1章节 基本插值和多行字符串

#### 54.2章节 标记字符串

#### 54.3章节 原始字符串

#### 54.4章节 使用模板字符串模板化HTML

#### 54.5章节 介绍

### 第五十五章节 Fetch

#### 55.1章节 获取JSON数据

#### 55.2章节 设置请求头

#### 55.3章节 POST数据

#### 55.4章节 发送Cookie

#### 55.5章节 GlobalFetch

#### 55.6章节 使用Fetch从Stack Overflow API中展示问题

### 第五十六章节 作用域

#### 56.1章节 闭包

#### 56.2章节 提升

#### 56.3章节 var和let之间的区别

#### 56.4章节 Apply和Call语法和调用

#### 56.5章节 箭头函数调用

#### 56.6章节 bind调用

#### 56.7章节 方法调用

#### 56.8章节 匿名调用

#### 56.9章节 构造函数调用

#### 56.10章节 循环中使用let而不是var(单击处理程序示例)

### 第五十七章节 模块化

#### 57.1章节 定义模块

#### 57.2章节 默认导出

#### 57.3章节 从其他模块导入命名成员

#### 57.4章节 导入整个模块

#### 57.5章节 使用别名导入命名成员

#### 57.6章节 导入有副作用

#### 57.7章节 导出多个命名成员

### 第五十八章节 Screen屏幕

#### 58.1章节 获取屏幕分辨率

#### 58.2章节 获取屏幕的可用区域

#### 58.3章节 页面宽度和高度

#### 58.4章节 Window innerWidth和innerHeight属性

#### 58.5章节 获取有关屏幕的颜色信息

### 第五十九章节 可变强制/转换

#### 59.1章节 双重否定（!!x）

#### 59.2章节 隐式转换

#### 59.3章节 转换为布尔值

#### 59.4章节 将字符串转换为数字

#### 59.5章节 将数字转换为字符串

#### 59.6章节 原始到原始转换表

#### 59.7章节 将数组转换为字符串

#### 59.8章节 使用数组方法从数组到字符串

#### 59.8章节 使用数组方法从数组到字符串

#### 59.9章节 将数字转换为布尔值

#### 59.10章节 将字符串转换为布尔值

#### 59.11章节 整数到浮点数

#### 59.12章节 浮点数到整数

#### 59.13章节 将字符串转换为浮点数

### 第六十章节 解构赋值

#### 60.1章节 解构对象

#### 60.2章节 解构函数参数

#### 60.3章节 嵌套解构

#### 60.4章节 解构数组

#### 60.5章节 解构内部变量

#### 60.6章节 解构时的默认值

#### 60.7章节 解构时重命名变量

### 第六十一章节 WebSocket

#### 61.1章节 使用字符串消息

#### 61.2章节 建立WebSocket连接

#### 61.3章节 使用二进制消息

#### 61.4章节 建立安全的WebSocket连接

### 第六十二章节 箭头函数

#### 62.1章节 介绍

#### 62.2章节 词法范围和绑定(“this”的值)

#### 62.3章节 参数对象

#### 62.4章节 隐含的Return

#### 62.5章节 箭头函数用作构造函数

#### 62.6章节 显式的Return

### 第六十三章节 Worker

#### 63.1章节 Web Worker

#### 63.2章节 简单的service worker

#### 63.3章节 注册service worker

#### 63.4章节 与Web Worker进行通信

#### 63.5章节 终止worker

#### 63.6章节 填充缓存

#### 63.7章节 专用Worker和共享Worker

### 第六十四章节 请求动画帧requestAnimationFrame

#### 64.1章节 使用requestAnimationFrame淡入元素

#### 64.2章节 保持兼容性

#### 64.3章节 取消动画

### 第六十五章节 创造性设计模式

#### 65.1章节 工厂函数

#### 65.2章节 工厂与组成

#### 65.3章节 模块和揭示模块模式

#### 65.4章节 原型模式

#### 65.5章节 单例模式

#### 65.6章节 抽象工厂模式

### 第六十六章节 检测浏览器

#### 66.1章节 特征检测方法

#### 66.2章节 用户代理检测

#### 66.3章节 库方法

### 第六十七章节 Symbol

#### 67.1章节 Symbol原语类型的基础知识

#### 67.2章节 使用Symbol.for()创建全局共享符号

#### 67.3章节 将Symbol转换为字符串

### 第六十八章节 翻译

#### 68.1章节 翻译简介

#### 68.2章节 开始将ES6/7与Babel一起使用

### 第六十九章节 自动分号插入-ASI

#### 69.1章节 避免在return语句中插入分号

#### 69.2章节 自动分号插入规则

#### 69.3章节 受自动分号插入影响的语句

### 第七十章节 本地化

#### 70.1章节 数字格式化

#### 70.2章节 货币格式化

#### 70.3章节 日期和时间格式化

### 第七十一章节 地理定位

#### 71.1章节 当用户的位置更改时获取更新

#### 71.2章节 获取用户的经度和纬度

#### 71.3章节 更多描述性错误代码

### 第七十二章节 IndexedDB

#### 72.1章节 打开数据库

#### 72.2章节 添加对象

#### 72.3章节 检索数据

#### 72.4章节 IndexedDB可用性测试

### 第七十三章节 模块化技术

#### 73.1章节 ES6模块化

#### 73.2章节 通用模块定义（UMD）

#### 73.3章节 立即调用函数表达式（IIFE）

#### 73.4章节 异步模块定义 (AMD)

#### 73.5章节 CommonJS - Node.js

### 第七十四章节 代理Proxy

#### 74.1章节 代理属性查找

#### 74.2章节 非常简单的代理（使用set trap）

### 第七十五章节 .postMessage()和 MessageEvent

#### 75.1章节 开始

### 第七十六章节 WeakMap

#### 76.1章节 创建WeakMap对象

#### 76.2章节 获取与键关联的值

#### 76.3章节 为键赋值

#### 76.4章节 检查是否存在具有该键的元素

#### 76.5章节 删除具有键的元素

#### 76.6章节 Weak参考演示

### 第七十七章节 WeakSet

#### 77.1章节 创建WeakSet对象

#### 77.2章节 添加值

#### 77.3章节 检查值是否存在

#### 77.4章节 删除值

### 第七十八章节 转义序列

#### 78.1章节 在字符串和正则表达式中输入特殊字符

#### 78.2章节 转义序列类型

### 第七十九章节 行为设计模式

#### 79.1章节 观察者模式

#### 79.2章节 中介模式

#### 79.3章节 命令

#### 79.4章节 迭代器

### 第八十章节 服务器发送的事件

#### 80.1章节 设置服务器的基本事件流

#### 80.2章节 关闭事件流

#### 80.3章节 将事件侦听器绑定到EventSource

### 第八十一章节 异步函数（async/await异步/等待）

#### 81.1章节 介绍

#### 81.2章节 Await和运算符优先级

#### 81.3章节 异步函数与Promises对比

#### 81.4章节 带async await的循环

#### 81.5章节 减少缩进

#### 81.6章节 同步异步(并行)操作

### 第八十二章节 异步迭代器

#### 82.1章节 基础

### 第八十三章节 如何使迭代器在异步回调函数中可用

#### 83.1章节 错误的代码，你能发现为什么这种键的使用会导致bug吗？

#### 83.2章节 正确的写法

### 第八十四章节 尾调用优化

#### 84.1章节 什么是尾调用优化（TCO）

#### 84.2章节 递归循环

### 第八十五章节 按位运算符-真实世界示例(代码片断)

#### 85.1章节 使用按位XOR交换两个整数（无需额外的内存分配）

#### 85.2章节 更快的乘法或除以2的幂

#### 85.3章节 使用按位与的数字奇偶校验检测

### 第八十六章节 波浪号 ~

#### 86.1章节 ~ 整数

#### 86.2章节 ~ 运算符号 

#### 86.3章节 将非数字值转换为数字

#### 86.4章节 速记

#### 86.5章节 ~ 十进制数

### 第八十七章节 使用JavaScript获取/设置CSS自定义变量

#### 87.1章节 如何获取和设置CSS变量属性值

### 第八十八章节 选择API

#### 88.1章节 获取所选内容的文本

#### 88.2章节 取消选择所选的所有内容

#### 88.3章节 选择元素的内容

### 第八十九章节 文件API，Blob和FileReader

#### 89.1章节 将文件读取为字符串

#### 89.2章节 将文件读取为dataURL

#### 89.3章节 文件切片

#### 89.4章节 获取文件的属性

#### 89.5章节 选择多个文件并限制文件类型

#### 89.6章节 客户端使用Blob下载csv

### 第九十章节 通知API

#### 90.1章节 请求发送通知的权限

#### 90.2章节 发送通知

#### 90.3章节 关闭通知

#### 90.4章节 通知事件

### 第九十一章节 抖动API

#### 91.1章节 单次抖动

#### 91.2章节 检查支持

#### 91.3章节 抖动模式

### 第九十二章节 电池状态API

#### 92.1章节 电池事件

#### 92.2章节 获得当前的电池电量

#### 92.3章节 电池充电了吗

#### 92.4章节 获得电池用完的剩余时间

#### 92.5章节 获得电池充满电的剩余时间

### 第九十三章节 流畅的API

#### 93.1章节 用JS捕获HTML文章结构的流畅的API

### 第九十四章节 Web加密API

#### 94.1章节 创建摘要（例如SHA-256）

#### 94.2章节 加密随机数据

#### 94.3章节 生成RSA密钥对并转换为PEM格式

#### 94.4章节 将PEM密钥对转换为CryptoKey

### 第九十五章节 安全问题

#### 95.1章节 反射的跨站点脚本（XSS）

#### 95.2章节 持久性跨站点脚本（XSS）

#### 95.3章节 来自JavaScript字符串文字的持久跨站脚本

#### 95.4章节 为什么来自其他人的脚本会损害您的网站及其访问者

#### 95.5章节 摧毁JSON注入

### 第九十六章节 安全问题

#### 96.1章节 通过message进行安全的跨域通信

#### 96.2章节 规避同源政策的方法

### 第九十七章节 错误处理

#### 97.1章节 Error对象

#### 97.2章节 与Promise互动

#### 97.3章节 Error类型

#### 97.4章节 操作顺序加上先进思想

### 第九十八章节 浏览器中的全局错误处理

#### 98.1章节 处理window.onerror将所有错误报告给服务器端

### 第九十九章节 调试Debugging

#### 99.1章节 交互式解释器变量

#### 99.2章节 断点

#### 99.3章节 使用setter和getter来查找更改属性的内容

#### 99.4章节 使用控制台

#### 99.5章节 自动暂停执行

#### 99.6章节 元素检查器

#### 99.7章节 调用函数时中断

#### 99.8章节 单步执行代码

### 第一百章节 JavaScript单元测试

#### 100.1章节 Mocha，sinon，chai和Proxyquire的单元测试Promise

#### 100.2章节 基本断言

### 第一百零一章节 JavaScript eval

#### 101.1章节 计算JavaScript语句字符串

#### 101.2章节 介绍

#### 101.3章节 求值与数学

### 第一百零二章节 Linters - 确保代码质量

#### 102.1章节 JSHint

#### 102.2章节 ESLint / JSCS

#### 102.3章节 JSLint

### 第一百零三章节 反模式

#### 103.1章节 在var声明中链式赋值

### 第一百零四章节 性能小贴士

#### 104.1章节 在性能关键的函数中避免使用try/catch

#### 104.2章节 限制DOM更新

#### 104.3章节 对代码进行基准测试 - 测量执行时间

#### 104.4章节 使用记忆器进行重计算功能

#### 104.5章节 使用null初始化对象属性

#### 104.6章节 重复使用对象而不是重新创建对象

#### 104.7章节 首选局部变量而不是全局变量、属性和索引值

#### 104.8章节 数字的使用要一致

### 第一百零五章节 记忆效率

#### 105.1章节 创建真正私有方法的缺点


































