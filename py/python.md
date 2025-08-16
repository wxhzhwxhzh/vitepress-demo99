# Python 入门教程

## 一、Python 是什么？
Python 是一种**简洁、易读、高效**的编程语言，由荷兰人 Guido van Rossum 于 1989 年圣诞节期间设计。它的设计哲学是“优雅、明确、简单”，语法简洁易懂，非常适合编程初学者入门。

Python 的应用领域非常广泛，包括：
- 网站开发（如 Django、Flask 框架）
- 数据分析与可视化
- 人工智能与机器学习
- 自动化脚本编写
- 游戏开发等

## 二、环境搭建：安装 Python
### 1. 下载 Python 安装包
访问 Python 官方网站（https://www.python.org/downloads/），根据你的操作系统（Windows、macOS、Linux）选择对应的安装包。建议下载 **Python 3.x 版本**（目前主流版本），因为 Python 2 已停止更新。

### 2. 安装步骤（以 Windows 为例）
- 运行下载的安装包，勾选 **“Add Python to PATH”**（非常重要，可避免手动配置环境变量）。
- 点击 **“Install Now”** 进行默认安装，或选择 **“Customize installation”** 自定义安装路径。
- 安装完成后，点击 **“Close”** 关闭窗口。

### 3. 验证安装是否成功
打开电脑的命令提示符（Windows）或终端（macOS/Linux），输入以下命令并回车：
```bash
python --version  # 或 python3 --version（部分系统）
```
如果显示类似 `Python 3.11.4` 的版本信息，说明安装成功。

## 三、第一个 Python 程序
### 1. 选择编辑器
推荐初学者使用以下工具：
- **IDLE**：Python 自带的简易编辑器，安装 Python 时已默认安装。
- **VS Code**：微软推出的轻量级编辑器，需安装 Python 插件。
- **PyCharm**：专业的 Python 集成开发环境（IDE），功能强大，有免费社区版。

### 2. 编写“Hello World”
打开编辑器，输入以下代码：
```python
# 这是一个注释，用于解释代码功能，不会被执行
print("Hello, World!")  # 打印输出内容
```
保存文件（扩展名为 `.py`，如 `hello.py`），然后运行程序。在 IDLE 中可直接点击 **Run → Run Module**，或在命令提示符/终端中输入：
```bash
python hello.py  # 或 python3 hello.py
```
运行后，屏幕将显示：`Hello, World!`

## 四、基本语法规则
### 1. 变量与数据类型
- 变量：无需声明类型，直接赋值即可，如 `name = "Python"`，`age = 30`。
- 常见数据类型：
  - 字符串（str）：用单引号或双引号包裹，如 `'Hello'`。
  - 整数（int）：如 `100`、`-5`。
  - 浮点数（float）：如 `3.14`、`-0.5`。
  - 布尔值（bool）：`True` 或 `False`。

### 2. 运算符
- 算术运算符：`+`（加）、`-`（减）、`*`（乘）、`/`（除）、`//`（整除）、`%`（取余）、`**`（幂）。
- 赋值运算符：`=`、`+=`、`-=` 等，如 `x += 1` 等价于 `x = x + 1`。
- 比较运算符：`==`（等于）、`!=`（不等于）、`>`、`<`、`>=`、`<=`，返回布尔值。

### 3. 条件语句
格式如下：
```python
age = 18
if age >= 18:
    print("已成年")
elif age >= 12:
    print("青少年")
else:
    print("儿童")
```
注意：**缩进**是 Python 的重要语法，通常用 4 个空格表示一层缩进。

### 4. 循环语句
- **for 循环**：用于遍历序列（如列表、字符串）。
```python
fruits = ["苹果", "香蕉", "橙子"]
for fruit in fruits:
    print(fruit)
```
- **while 循环**：当条件为真时重复执行。
```python
count = 0
while count < 3:
    print("计数：", count)
    count += 1
```

## 五、列表与字典
### 1. 列表（List）
有序的可变序列，用方括号 `[]` 表示。
```python
# 创建列表
numbers = [1, 2, 3, 4, 5]
# 访问元素（索引从 0 开始）
print(numbers[0])  # 输出 1
# 添加元素
numbers.append(6)
# 修改元素
numbers[2] = 10
# 切片操作
print(numbers[1:4])  # 输出 [2, 10, 4]
```

### 2. 字典（Dictionary）
键值对的无序集合，用花括号 `{}` 表示。
```python
# 创建字典
person = {"name": "小明", "age": 20, "gender": "男"}
# 访问值
print(person["name"])  # 输出 小明
# 添加/修改键值对
person["height"] = 175
person["age"] = 21
# 遍历字典
for key, value in person.items():
    print(key, ":", value)
```

## 六、函数
函数是可重复使用的代码块，用 `def` 关键字定义。
```python
# 定义函数
def greet(name):
    """这是一个打招呼的函数"""
    print("你好，", name, "！")

# 调用函数
greet("Python 学习者")  # 输出 你好， Python 学习者 ！

# 带返回值的函数
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # 输出 8
```

## 七、下一步学习建议
1. 多写代码：通过实际练习巩固语法知识。
2. 学习内置函数：如 `len()`、`range()`、`input()` 等。
3. 掌握文件操作：学习如何读写文本文件。
4. 了解模块与库：如 `math`、`random` 等标准库的使用。
5. 尝试小项目：如简易计算器、猜数字游戏等。

希望这个入门教程能帮助你开启 Python 的学习之旅！遇到问题时，可查阅 Python 官方文档（https://docs.python.org/）或加入编程社区提问。