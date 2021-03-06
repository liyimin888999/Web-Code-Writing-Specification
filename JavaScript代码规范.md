#  JavaScript代码规范

## 1 代码风格

### 1.1 结构

#### 1.1.1 缩进

- 使用使用 `4` 个空格做为一个缩进层级，不允许使用 `2` 个空格 或 `tab` 字符。

#### 1.1.2 空格

- 二元运算符两侧必须有一个空格，一元运算符与操作对象之间不允许有空格。

- 用作代码块起始的左花括号 `{` 前必须有一个空格。

- `if / else / for / while / function / switch / do / try / catch / finally` 关键字后，必须有一个空格。

- 在对象创建时，属性中的 `:` 之后必须有空格，`:` 之前不允许有空格。

- 函数声明、具名函数表达式、函数调用中，函数名和 `(` 之间不允许有空格。

- `,` 和 `;` 前不允许有空格。如果不位于行尾，`,` 和 `;` 后必须跟一个空格。

- 在函数调用、函数声明、括号表达式、属性访问、`if / for / while / switch / catch` 等语句中，`()` 和 `[]` 内紧贴括号部分不允许有空格。

- 单行声明的数组与对象，如果包含元素，`{}` 和 `[]` 内紧贴括号部分不允许包含空格。

#### 1.1.3 换行

- 每个独立语句结束后必须换行。

- 每行不得超过 `120` 个字符。

- 在函数声明、函数表达式、函数调用、对象创建、数组创建、`for` 语句等场景中，不允许在 `,` 或 `;` 前换行。

#### 1.1.4 语句

- 不得省略语句结束的分号。

- 在 `if / else / for / do / while` 语句中，即使只有一行，也不得省略块 `{...}`。

### 1.2 命名

- `变量 / 函数 / 函数的参数 / 类的方法和属性`使用 `Camel命名法`。

- `常量` 使用 `全部字母大写，单词间下划线分隔` 的命名方式。

- `类` 使用 `Pascal命名法`。

- 由多个单词组成的缩写词，在命名中，根据当前命名法和出现的位置，所有字母的大小写与首字母的大小写保持一致。

- `boolean` 类型的变量使用 `is`  开头。

## 2 语言特性

### 2.1 变量

- 变量、函数在使用前必须先定义。
- 变量必须 `即用即声明`，不得在函数或其它形式的代码块起始位置统一声明所有变量。
- 创建对象与数组使用字面量创建新对象与数组，例`var obj = {} / var arr = []`。

### 2.2 条件

- 在 Equality Expression 中使用类型严格的 `===`。仅当判断 `null` 或 `undefined` 时，允许使用 `== null`。

### 2.3 字符串

- 只要不报错，引号全用单引号`''`。