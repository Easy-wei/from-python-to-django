# 第一步
=======

现在,我们将看到在Python中如何运行一个传统的“Hello World”程序。这将教你如何写、保存和运行Python程序。

使用Python运行你的程序有两种方法——使用交互式解释器提示符或使用一个源文件。现在,我们将看到如何使用这两种方法。

## 使用解释器提示符

在您的操作系统中打开终端(如前面[安装](a-byte-of-python3/install.md)所述),然后，输入`python3`按回车键，打开Python提示符。

一旦你启动python 3,您应该看到'>>>”,这被称为_Python解释器提示符_，你可以开始输入Python程序。

在Python解释器提示符下，输入

```python
print("Hello World")
```

然后按回车键。您应该看到输出了单词“Hello World”。

当使用一个Mac OS X计算机，下面是你将看到的一个例子。Python软件的细节会根据你的电脑不同而有所不同，但从提示符(即从“>>>”开始)与操作系统无关，应该是相同。

```python
> python3
Python 3.5.2 (default, Jan 14 2016, 06:54:11)
[GCC 4.2.1 Compatible Apple LLVM 7.0.2 (clang-700.1.81)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello World")
Hello World
```

注意,Python让你的代码行立即输出了!你刚才输入的是一个Python_语句_。我们使用`print`输出(不出所料)你提供给它的任何值。在这里,我们提供的是文本“Hello World”,并立即打印到屏幕上。

### 如何退出解释器提示符

如果你正在使用一个Linux或Unix shell,您可以通过按下`[ctrl - d]`或输入`exit()`(注意:记得包含括号,`()`)，然后输入回车键。

如果您使用的是Windows命令行提示符,按`[ctrl - z]`键再按回车键，退出解释器提示符。

## 选择一个编辑器

我们不能在每次想要运行一些东西的时候都要在解释器提示符下输入我们的程序，所以我们必须把它们保存为文件，这样我们可以任意次地运行我们的程序。

要创建我们的Python源文件,我们需要一个可以输入并保存它们的编辑软件。一个优秀的程序员的编辑器将使你写源代码文件的生活更容易。因此，选择一个编辑器确实至关重要。你必须选择一个编辑器，就像你选择要买的汽车一样。一个好的编辑器会帮助您很容易地编写Python程序，（就像一辆车可以让你）以一个更快和更安全的方式，让你的旅程更舒适，并且可以帮助你实现你的目标。

一个非常基本的需求是_语法高亮显示_，分别以不同的彩色显示你的Python程序所有的不同部分，以便您可以看到你的程序且使其运行可视化。

如果你不知道从哪里开始，我推荐可以在Windows、Mac OS X和GNU/Linux上使用的[PyCharm Educational Edition](https://www.jetbrains.com/pycharm-edu/)软件。

如果您使用的是Windows，*不要使用记事本*——这是一个糟糕的选择，因为它不做语法高亮显示，而且更重要的是它不支持文字的缩进——之后我们在我们的例子中会看到，缩进是非常重要的。好的编辑器如Komodo Edit会自动地做到这一点。

如果你是一名有经验的程序员，那么你一定已经使用[Vim](http://www.vim.org/)或[Emacs](http://www.gnu.org/software/emacs/)了。不用说，这是两个最强大的编辑器，使用它们来写你的Python程序，你会从中受益。就我自己而言，在我的大多数项目,甚至写一[整本书都在用Vim](http://www.swaroopch.com/notes/vim)。

从长远来看Vim或者Emacs是非常有用的，如果你愿意花时间去学习，那么我强烈建议你使用它们。然而,正如我之前提到的,初学者可以从PyCharm开始学习Python而不是编辑器。

再次重申，请选择一个适当的编辑器，它可以使编写Python程序更有趣和更容易。

## PyCharm

[PyCharm Educational Edition](https://www.jetbrains.com/pycharm-edu/) is a free editor which you can use for writing Python programs.

When you open PyCharm, you'll see this, click on `Create New Project`:

![When you open PyCharm](./img/pycharm_open.png)

Select `Pure Python`:

![PyCharm New Project](./img/pycharm_create_new_project.png)

Change `untitled` to `helloworld` as the location of the project, you should see details similar to this:

![PyCharm project details](./img/pycharm_create_new_project_pure_python.png)

Click the `Create` button.

Right-click on the `helloworld` in the sidebar and select `New` -> `Python File`:

![PyCharm -> New -> Python File](./img/pycharm_new_python_file.png)

You will be asked to type the name, type `hello`:

![PyCharm New File dialog box](./img/pycharm_new_file_input.png)

You can now see a file opened for you:

![PyCharm hello.py file](./img/pycharm_hello_open.png)

Delete the lines that are already present, and now type the following:

<!-- TODO: Update screenshots for Python 3 -->

```python
print("hello world")
```
Now right-click on what you typed (without selecting the text), and click on `Run 'hello'`.

![PyCharm Run 'hello'](./img/pycharm_run.png)

You should now see the output (what it prints) of your program:

![PyCharm output](./img/pycharm_output.png)

Phew! That was quite a few steps to get started, but henceforth, every time we ask you to create a new file, remember to just right-click on `helloworld` on the left -> `New` -> `Python File` and continue the same steps to type and run as shown above.

You can find more information about PyCharm in the [PyCharm Quickstart](https://www.jetbrains.com/pycharm-educational/quickstart/) page.

对Vim用户
> John M Anderson有一个很好的如何[使Vim成为强大的Python IDE](http://blog.sontek.net/blog/detail/turning-vim-into-a-modern-python-ide)的介绍。还推荐[jedi-vim插件](https://github.com/davidhalter/jedi-vim)和[我自己的dotvim配置](https://github.com/swaroopch/dotvim)。

对Emacs用户
> Pedro Kroger有一个很好的如何[使Emacs成为强大的Python IDE](http://pedrokroger.net/2010/07/configuring-emacs-as-a-python-ide-2/)的介绍。还建议[BG的dotemacs配置](https://github.com/ghoseb/dotemacs)。

## 使用一个源文件

现在让我们回到编程。每当你学习一种新的编程语言时，有一个传统，你编写和运行的第一个程序是“Hello World”程序——当你运行它时，它所做的只是说“Hello World”。正如Simon Cozens(神奇的"Beginning Perl"的作者)所说，这是“向编程神祈求帮你更好学习语言的传统咒语。”

开始你选择的编辑器，输入以下程序并将其保存为“hello.py’。

如果你使用Komodo编辑器，点击File --- New --- New File,输入下行:

```
print('Hello World')
```

在Komodo编辑器，选File --- Save保存文件。

你应将文件保存在哪里？你知道位置的任何文件夹。如果你不明白这是什么意思，创建一个新文件夹，并使用该位置保存和运行你所有的Python程序:

* C:\\py 在Windows上
* /tmp/py 在Linux上
* /tmp/py 在Mac OS X上

使用'mkdir'命令在命令行创建一个文件夹，例如,“mkdir /tmp/py”。

重要的
> 总要确保你给它的文件扩展名是.py，例如，“foo.py”。

在Komodo Edit，请单击“Tools”---“Run Command”，输入"c:\python33\python hello.py",单击“Run”,你应该看到像下面截图的打印输出。

![“Hello world”程序在Komodo编辑器中的截图](https://raw.github.com/borisliu/from-python-to-django-cms/master/docs/a-byte-of-python3/hello.png)
“Hello world”程序在Komodo编辑器中的截图

尽管最好的方式是在Komodo中输入它，但在命令行也可以：

1. 打开在安装章节中介绍的一个命令行。
2. Change directory（改变路径）到你保存文件的目录，例如cd c:\py
3. 在命令行输入c:\python33\python hello.py命令运行程序。
 
输出如下所示：

```
D:> c:\python33\python hello.py
Hello World
```

如果你得到了如上所示有输出，祝贺你!——你已经成功地运行了你的第一个Python程序。您已经成功地越过学习编程最难的部分－－开始你的第一个程序!

如果你得到了一个错误，请完全输入如上所示程序，再次运行这个程序。注意，Python是区分大小写的，即“print”并不等于“Print”——注意，前者是小写字母“p”和后者是大写字母“P”。同样，确保每一行的第一个字母之前没有空格或制表符——之后我们将明白为什么这很重要。

**它是如何工作的**

Python程序是由语句组成，在我们的第一个程序中，我们只有一个语句，在这个语句中，我们调用“print”*函数*，它只是打印文本“Hello World”。我们在稍后章节([函数](a-byte-of-python3/function))将详细学习函数——你现在应该理解的是,无论你在括号提供什么，都将打印到屏幕上。在本例中，我们提供了文本“Hello World”。

## 可执行的Python程序

这只适用于Linux和Unix用户，但Windows用户应该知道。

每次，你想要运行一个Python程序，我们必须显式地调用的“python foo.py”，但是我们为什么不能像运行我们电脑中的其它任何程序一样运行它呢？我们通过使用叫hashbang行代码可以实现。

添加下面的一行作为程序的第一行:

```
#!/usr/bin/env python
```

这样，你的程序应该像现在这样:

```
#!/usr/bin/env python
print('Hello World')
```

第二，我们必须给程序的可执行权限－－使用' chmod '命令，然后运行源程序。

这里使用的chmod命令是*change the mode of the file* （改变文件的模式），通过给系统All(所有)用户execute（可执行）权限。

```
$ chmod a+x hello.py
```

现在，我们可以直接运行我们的程序，因为我们的操作系统调用“/usr/bin/env”，它按次序找到我们的Python 3软件，然后知道如何运行我们的源文件:

```
$ ./hello.py
Hello World
```

我们使用“./”用来指示程序在当前目录中。

为了让事情变得更有趣，你可以将文件重命名为“hello”然后像“./hello”这样运行它，因为系统知道它必须使用源代码文件中第一行指定位置的解释器运行它，所以它仍将工作。

到目前为止,我们已经能够运行我们的程序,只要我们知道确切的路径。如果我们希望能够运行该程序从文件夹?您可以通过将程序存储在列在“路径”环境变量中的一个文件夹中来实现。

无论你何时运行任何程序，系统在列在“PATH”（路径）环境变量中的每个文件夹查找该程序，然后运行程序。我们通过简单地复制这个源文件到“PATH”（路径）列出的目录中，可以让这个程序到处可用。

```
$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/X11R6/bin:/home/swaroop/bin
$ cp hello.py /home/swaroop/bin/hello
$ hello
Hello World
```

使用'echo'（回响）命令和变量（PATH）名称加前缀'$'，指示shell我们需要“环境变量”的值，我们可以显示“PATH”（路径）变量的值。我们看到,“/home/swaroop/bin”是PATH变量中的一个目录，*swaroop*是在我的系统中我用的用户名，通常在你的系统中为你的用户名，会有一个类似的目录。

如果你想添加您所选择的目录到“PATH”变量中——这可以通过运行“export PATH=$PATH:/home/swaroop/mydir”,“:/home/swaroop/mydir”是我想添加到“PATH”变量中的目录。

如果你想写可以在任何时间、在任何地点运行的命令，这个方法非常有用。这就像创建你自己的在命令行使用的命令，就像“cd”或任何其他命令。

## 获得帮助

如果您需要快速获取任何的Python函数或语句的信息，那么您可以使用内置的“help”(帮助)功能。这是非常有用的，尤其是当使用翻译提示符时，例如，运行‘help(print)”——这将显示print函数的帮助－－用于打印东西到屏幕上。

注意
> 按q退出帮助

类似地,您可以获得Python中几乎任何事情的信息，使用“help()”去学习更多关于使用“help”本身的信息!

如果你需要获取操作符，如“return”的帮助，那么你只需要把这些放到引号内部，如“help('return'），所以，对于我们试图要做的事情，Python并不感到困惑。

## 总结

现在，你可以自由自在地编写、保存和运行Python程序了。

既然你是一名Python用户，让我们学习一些Python概念。

## 基础

只是打印“Hello World”是不够的，是吗？你想要做的不仅仅是这些，你想带一些输入，操纵它，得到些输出。在Python中，我们使用常量和变量可以实现这些。在这一章，我们还将学习一些其他的概念。

### 注释

*注释*是#符号右边的任何文字，它对读程序的人有很大注释用处。

例如：

```
print('Hello World') # 注意：print是一个函数
```

或者:

```
# 注意：print是一个函数
print('Hello World')
```

在你的程序中，你尽可能使用有用的注释:

* 解释设想
* 解释重要决策
* 解释重要细节
* 解释你在试图解决的问题
* 解释程序中你在努力克服的问题，等等。

[代码告诉你怎样做，注释告诉你这样做的原因。](http://www.codinghorror.com/blog/2006/12/code-tells-you-how-comments-tell-you-why.html)

这对你的程序的读者是有用的，他们可以很容易地理解程序做什么。记住，六个月后这个人可以是你自己！

### 字面常量

字面常量的一个例子是一个数字就像“5”、“1.23”，或一个字符串像“这是一个字符串”或“它一个字符串!”。它被称为字面，因为它是字面的——你使用它的字面值。数字'2'总是代表本身并没有什么其他的——它是一个常数，因为它的价值是不能改变的，因此，所有这些被称为字面常量。

### 数字

数字主要有两种类型--整型和浮点数。

‘2’是整数的一个例子，它只是一个完整的数。

浮点数(或简称为浮点)的例子有3.23和52.3E-4。符号E表示10的次方。在这种情况下，52.3E-4的意思是52.3的-4次方。

有经验的程序要注意：
> Python中没有单独的long(长)整型。int(整型)可以是任意大小的整数。

### 字符串

字符串是字符的一个序列，字符串通常只是一串单词。

在你写的每一个Python程序中都要使用字符串，因此要注意以下部分：

#### 单引号

你可以使用单引号例如'Quote me on this'指定字符串。所有的空白，例如空格和制表符都按原样保留。

#### 双引号

在双引号中的字符串和在单引号中的字符串工作起来完全一样。例如"What's your name?"

#### 三重引号

您可以使用三重引号-("""或''')指定多行字符串。在三重引号中您可以自由使用单引号和双引号。例如:

```
'''This is a multi-line string. This is the first line.
This is the second line.
"What's your name?," I asked.
He said "Bond, James Bond."
'''
```

#### 字符串是不可改变的

这意味着，一旦您已经创建了一个字符串，你就不能改变它。虽然这看起来似乎是一件坏事，但它真不是(坏事)。在我们后面看到的各种程序中，将会明白这不是一个限制。

C/C++程序员要注意
> 在Python中没有单独的“char”(字符型)数据。这里没有真正的需要它，我相信你不会错过它。

Perl/PHP程序员要注意
> 记住，单引号字符串和双引号字符串是相同的——他们不以任何方式不同。

#### 格式方法

有时，我们可能想要从其它信息构建字符串。这就是“format()”方法有用之处。

保存下面几行到文件"str_format.py"中:

```
age = 20
name = 'Swaroop'

print('{0} was {1} years old when he wrote this book'.format(name, age))
print('Why is {0} playing with that python?'.format(name))
```

输出结果为:

```
python str_format.py
Swaroop was 20 years old when he wrote this book
Why is Swaroop playing with that python?
```

它是如何工作的:

一个字符串可以使用特定的格式，随后调用format方法，用format方法替代那些使用适当参数的格式。

观察使用第一处，我们使用“{0}”对应于变量‘name’,这是format(格式)方法的第一个参数。类似的,第二个格式是“{1}”对应的“age”,这是格式方法的第二个参数。注意，Python从0开始计数，这意味着第一位置的索引是0，第二个位置的索引是1，等等。

注意，我们可以使用字符串的连接，name+'is'+str(age)+'years old' 实现同样的目的，但这非常讨厌、容易出错。第二，在这种情况下，通过format方法自动转换为字符串，而不是显式地转换为需要的字符串。第三，当使用的format 方法，我们可以改变消息，而无需处理使用的变量，反之亦然。

还要注意，这些数字(索引)都是可选的，所以你也可以写成:

```
age = 20
name = 'Swaroop'

print('{} was {} years old when he wrote this book'.format(name, age))
print('Why is {} playing with that python?'.format(name))
```

这将给与前面的程序相同的输出。

Python在format方法中做的是，用每个参数值替代规格的地方。这里有更详细的规格，如:

```
 decimal (.) precision of 3 for float '0.333'
>>> '{0:.3}'.format(1/3)
 fill with underscores (_) with the text centered
 (^) to 11 width '___hello___'
>>> '{0:_^11}'.format('hello')
 keyword-based 'Swaroop wrote A Byte of Python'
>>> '{name} wrote {book}'.format(name='Swaroop', book='A Byte of Python')
```

### 变量

仅仅使用字面常量会很快变得无聊——我们需要某种方式存储任何信息，同样操作它们。这就要引入变量。变量是它的名字所指示的东西——他们的值会有所不同。例如，你可以用变量存储任何值。变量是你电脑中存储信息的内存的一部分。不像字面常量，您需要某种方法来访问这些变量，因此你要给出他们的名字。

### 标识符命名

变量是标识符的一个示例。标识符是用来识别一些东西的名字。这里有一些你必须遵循的标识符命名规则:

* 标识符的第一个字符必须是字母表中的一个字母(大写或小写的ASCII或Unicode字符)或下划线(“_”)。
* 标识符名称的其余部分可以包含字母(大写或小写的ASCII或Unicode字符)、下划线(“_”)或数字(0 - 9)。
* 标识符的名称都是区分大小写的。例如,“myname”和“myName”**不**相同。注意前者中“n”小写和后者中'N'大写。
* *有效*的标识符名称的例子有：“i”,“myname”,“name23”。*无效*的标识符名字的例子有：“2things”,“this is spaced out”,“my-name”、“>a1b2_c3”和"this_is_in_quotes"。

### 数据类型

变量可以保存不同的被称为**数据类型**的数值。基本类型是数字和字符串，我们已经讨论了。在后面的章节中，我们将看到如何使用类创建自己的类型。

### 对象

记住，Python把程序中使用的任何东西作为一个*对象*。在常识中这意味着，我们说‘*对象*’，而不是说‘*一些东西*’,

面向对象编程的用户要注意
> 一切东西都是对象，包括数字、字符串和函数，在这个意义上讲，Python是坚定的面向对象的。

现在，我们将看到如何使用变量以及字面常量。保存下面的示例，运行这个程序。

## 怎样写Python程序

从此以后，保存和运行一个Python程序的标准过程如下:

1. 打开选择的编辑器，例如Komodo Edit。
2. 输入例子中给出的程序代码。
3. 用提到的文件名保存为文件。
4. 在命令行使用python program.py命令运行程序。

例如: 使用变量和常量

Filename : var.py

```
i = 5
print(i)
i = i + 1
print(i)

s = '''这是一个多行字符串。
这是第2行。'''
print(s)
```

输出结果为:

```
D:> python var.py
5
6
这是一个多行字符串。
这是第2行。
```

它是如何工作的:

下面介绍这个程序如何工作的。首先，我们使用赋值运算符('=')为变量'i'指定了文字常量值‘5’,这一行叫做一个声明，因为它指出应该做一些事情，在这个例子中，我们将名为'i'的变量与值‘5’相联系。接下来,我们使用'print'函数打印'i'的值，不出所料，恰恰打印变量的值到屏幕上。

然后，我们给存储在变量'i'中的值加'1'后，再存回到'i'中。然后，我们把它打印出来，我我们想的一样，我们得到值'6'。

同样，我们为字符串变量's'指定了文字字符串，然后打印它。

静态语言程序员应注意
> 变量的使用只是通过给他们指定一个价。不需要/不使用声明或数据类型定义。


### 逻辑行与物理行

物理行是当你写程序时看到的一行。逻辑行是Python 看到的一个单独语句。Python默认一个物理行为一个逻辑行。

一个逻辑行是一个语句，像print('Hello World')－－如果它本身在一行上（像你在一个编辑器中看到的），那么，它也是一个物理行。

默认情况下，Python鼓励一行写一个语句的用法，这使代码更可读。

如果您想要在一个物理行列举多个逻辑行，那么您必须使用一个表示逻辑行/语句结束的分号“;”显式地指明。例如：

```
i = 5
print(i)
```

与

```
i = 5;
print(i);
```

等效。

同样可写成：

```
i = 5; print(i);
```

甚至是

```
i = 5; print(i)
```

然而，我**强烈建议**你坚持**在每一个物理行编写一个最大的逻辑行**。这就是你永远都不要使用分号。事实上，我**从未**使用，甚至在python程序中从来没有见过一个分号。

这个观念是很有用的，还有一种情况：如果你有一个长代码行，你可以通过使用反斜杠把它分解为多个物理行。这是被称为**显式行连接**:

```
s = '这是一个字符串。 \
这是字符串的继续。'
print(s)
```

输出结果为：

```
这是一个字符串。这是字符串的继续。
```

同样的，

```
print\
(i)
```

与

```
print(i)
```

相同

有时有一种隐含的假设，您不需要使用一个反斜杠。在这种情况下，逻辑行有一个开始圆括号、开始方括号或开始花括号，但不是一个结束的括号。这被称为**隐式连接**。当我们在以后的章节－－编写程序使用列表时，你可以看到它的作用。

### 缩进

在Python中的空白是重要的。实际上，**在一行开始的空格是重要的**。这被称为**缩进**。在逻辑行开头的前导空白(空格和制表符)用于确定逻辑行的缩进级别，它用于依次确定语句的分组。

这意味着一起的语句**必须**有相同的缩进。每一个这样的语句组被称为**块**。在后面的章节，我们将看到的块是何等重要的例子。

你应该记住的一件事是，错误的缩进可以产生错误。例如:

```
i = 5
 print('值是 ', i) # 错误! 注意在行的开头有一个空格
print('重复，值是 ', i)
```

当运行它时，将会发生下面的错误：

```
  File "whitespace.py", line 4
    print('Value is ', i) # Error! Notice a single space at the start of the line
    ^
IndentationError: unexpected indent
```

请注意，这里第二行的开头有一个空格。这个错误表明：Python告诉我们程序的语法是无效的，即程序写的不正确。这意味着，你不能任意开始语句中的新块(当然，除了默认的主块，您一直已经使用的)。您可以使用新块的情况，将在后面的章节详细，如"控制流"。

如何缩进
> 缩进只使用空白，用制表符使用4个空格。好的编辑器如Komodo Edit会为你自动这样做。确保你使用一致的数量的缩进空格，否则你的程序将显示错误。

静态语言程序员应注意
> Python为块总是使用缩进，从来不用花括号。运行from __future__ import braces可以了解更多。

### 小结

现在，我们已经经历了许多细节,我们可以转到更有趣的东西，如控制流语句。一定要熟悉这一章你所读的。

## 操作符和表达式

你编写的大多数语句（逻辑行）都将包含*表达式*。一个表达式的简单例子是2+3。一个表达式可分解成操作符和操作对象。

*操作符*的功能是做一些事，通过符号，如+或特别的关键字表现。操作符需要一些数据来操作，这些数据被你作*操作对象*。在这个例子中2和3是操作对象。

### 操作对象

我们将简单地看一下操作符和它的用法：

注意，您可以使用交互式解释器计算例子中给出的表达式。例如,为了测试表达式“2 + 3”,使用交互式Python解释器提示符:

```
>>> 2 + 3
5
>>> 3 * 5
15
>>>
```

\+ (加号)

  两个对象相加

  3 + 5 得 8. 'a' + 'b' 得 'ab'.

\- (减号)

  给出一个数减去另一数的差；如果缺少第一个操作数，它默认为是0。

  -5.2 得到一个负数，50 - 24 得 26.

\* (乘法)

  给出两个数的乘积或返回重复多次的字符串。

  2 * 3 得 6. 'la' * 3 得到 'lalala'.

** (幂)

  返回x的y次幂

  3 ** 4 得 81 (也就是3*3*3*3)

/ (除法)

  用y分x（x除以y）

  4 / 3 得1.3333333333333333.

// (整除)

  得到除法的商

  4 // 3 得 1.

% (取模)

  返回除法的余数

  8 % 3 得 2. -25.5 % 2.25 得 1.5.

<< (向左移位)

  数字向左移动指定位数。(在内存中每个数字由比特或二进制数表示，例如：0和1）。 2 << 2 得 8. 2 用二进制表示为10。

  左移两位得到 1000，它表示数字8。

\>> (向右移位)

  数字向右移动指定位数。

  11 >> 1 得 5.

  11 用二进制表示为1011，向右移动1位后得到二进制101，表示数字5。

& (位与)

  数字的位相与

  5 & 3得 1。

| (位或)

  数字的位相或

  5 | 3得 7

^ (位异或)

  数字的位相异或

  5 ^ 3 得 6

~ (位求反)

  x的位求反结果为-(x+1)

  ~5 得 -6.

< (小于)
  
  返回x是否小于y。所有的比较运算符返回True或False。注意这些名字的大小写。

  5 < 3 返回 False 而 3 < 5 返回 True.

  比较运算符可以任意连接：3 < 5 < 7 返回 True.

\> (大于)

  返回x是否大于y

  5 > 3 返回 True。如果操作对象都是数字，它们首先转换为普通型，否则，将返回False。

<= (小于等于)
  
  返回x是否小于等于y

  x = 3; y = 6; x <= y 返回 True.

\>= (大于等于)

  返回x是否大于等于y

  x = 4; y = 3; x >= 3 返回 True。

== (等于)

  比较操作对象是否相等

  x = 2; y = 2; x == y 返回 True.

  x = 'str'; y = 'stR'; x == y 返回 False.

  x = 'str'; y = 'str'; x == y 返回 True.

!= (不等于)

  比较操作对象是否不相等

  x = 2; y = 3; x != y 返回 True.

not (逻辑非)

  如果 x 是 True,它返回 False。如果 x 是 False，它返回 True。

  x = True; not x 返回 False.

and (逻辑与)

  如果x是False, x and y 返回 False，否则它返回y的值。

  x = False; y = True; x and y 返回 False，因为 x 为假。在这种情况下，Python将不计算y，因为它知道and左边表达式是 False ，这意味着整个表达式将为 False ，而不论其它值为什么。这叫做求值捷径。

or (逻辑或)

  如果 x 为 True, 它返回真，否则它返回y的值。

  x = True; y = False; x or y 返回 True。求值捷径这也适用。

### 数学操作和赋值的快捷方式

对一个变量进行数学操作是常见的。然后将操作的结果返回给变量，今后，对这样的表达式有一个快捷方式:

你可以把：

```
a = 2
a = a * 3
```

写成：

```
a = 2
a *= 3
```

注意：将 var = var operation expression 写成 var operation= expression。

### 运算顺序

如果你有一个表达式如 2 + 3 * 4, 是先做加法还是先做乘法呢？我们的高中数学告诉我们，应该先做乘法。这意味着乘法操作符比加法操作符具有更高的优先级。

下面的表给出了Python运算顺序的优先表，从最低（最小约束力）到最高(最高约束力)。 意思是说，在给定的表达式中，Python将在计算表上方列出的对象和表达式之前，首先运算表下方的。

下面的表取自[Python参考手册](http://docs.python.org/py3k/reference/expressions.html#summary)，是为了提供完整性。为了显式地指定优先级，更好的做法是使用圆括号组织运算符和操作对象。这可使程序更加可读。详见下面更改运算顺序。

lambda

  Lambda表达式

or

  逻辑或

and

  逻辑与

not x

  逻辑非

in, not in

  成员检测

is, is not

  鉴别检测

<, <=, >, >=, !=, ==

  比较

|

  位或

^
  
  位异或

&

  位与

<<, >>

  移位

+, -

  加和减

*, /, //, %

  乘法，除法，浮点除和余数

+x, -x

  正，负

~x

  按位非

**

  乘方

x.attribute

  属性引用

x[index]

  索引

x[index1:index2]

  切片

f(arguments ...)

  函数调用

(expressions, ...)

  显示 Binding 或元组

[expressions, ...]

  显示列表

{key:datum, ...}

  显示字典

我们没有遇到的操作符将在后面的章节解释。

上表中在同一行列出的操作符具有*相同优先级*。例如，“+”和“-”具有相同的优先级。

### 改变运算顺序

为使表达式更具可读性，我们可以使用圆括号。例如2 + (3 * 4) 肯定比需要知道操作符运算优先级的 2 + 3 * 4 更容易理解。与其他方面一样，应该合理使用括号不应该冗余(不要过分使用),如(2 + (3 * 4))。

使用括号有一个额外的优势——它帮助我们更改运算顺序。例如，如果您想要在一个表达式中加法在乘法之前运算，那么你可以这样写 (2 + 3) * 4。

### 结合性

操作符通常从左到右。这意味着具有相同优先级的操作符从左到右的方式计算。例如2 + 3 + 4计算为 (2 + 3) + 4。一些操作符，像赋值操作符，有从右到左的结合性，即 a = b = c 被视为 a = (b = c)。

### 表达式

例子 (保存为expression.py):

```
length = 5
breadth = 2

area = length * breadth
print('Area is', area)
print('Perimeter is', 2 * (length + breadth))
```

输出:

```
D:> python expression.py
Area is 10
Perimeter is 14
```

它是如何工作的

矩形的长度和宽度以同样的名字存储在变量中，在表达式的帮助下，我们使用这些计算矩形的面积和周长。我们存储表达式length * breadth 的结果在变量area中，然后使用print函数打印它。在第二种情况下,在打印函数中我们直接使用表达式2 * (length + breadth)的值。

同样要注意，Python'完美打印'是如何输出的。即使我们没有在'Area is' 和变量area,之间指定一个空间，Python为我们得到一个干净漂亮的输出，而且这种方式使用程序的可读性更强(因为我们不需要担心为输入我们在字符串中间使用的空格)。这只是让Python程序员的生活更方便的一个例子。

### 小结

我们已经看到了如何使用操作符，操作对象和表达式——这是任何程序的基石。接下来,我们将看到在使用语句的程序中如何利用这些。

## 控制流

在程序中，到现在为止，我们看到，一直有一系列的语句被Python以由上而下的顺序如实地执行。如果你想改变它的流程，它会如何工作呢？例如，你想让程序作出一些决定，而且不同的情况做不同的事情，例如，根据一天的时间不同，打印“早上好”或“晚上好”？

正如你可能已经猜到的，这要通过使用控制流语句。在Python中有三个控制流语句-- if, for 和 while。

### if 语句

if 语句是用来检查一个条件:如果条件为真,我们运行一个语句块(你为if块)，(否则)else，我们执行另一个语句块(称为else块)。else子语句是可选的。

例如 (保存为 if.py):

```
number = 23
guess = int(input('请输入一个整数: '))

if guess == number:
    print('恭喜，你猜对了。') # 新块从这里开始
    print('(但你没有获得任何奖品！)') # 新块在这里结束
elif guess < number:
    print('不对，你猜的有点儿小') # 另一个块
    # 在一个块中你可以做你想做的任何事...
else:
    print('不对，你猜的有点大')
    # 你猜的数比number大时才能到这里

print('完成')
# if语句执行完后，最后的语句总是被执行
```

输出:

```
D:> python if.py
请输入一个整数: 50
不对，你猜的有点儿大
完成

D:> python if.py
请输入一个整数: 22
不对，你猜的有点儿小
完成

D:> python if.py
请输入一个整数: 23
恭喜，你猜对了。
 (但你没有获得任何奖品！)
完成
```

它是如何工作的:

在这个程序中，我们获取来自用户的猜测，并检查这个数是否是我们设定的数。我们给变量number设置我们想要的任何整数，比如 23。然后，我们使用input() 函数获取用户的猜的数。函数是可重用的程序块。我们在[下一章](a-byte-of-python3/function)中会阅读关于它们的更多东西。

我们给内置的input 函数提供一个字符串，该函数将其打印到屏幕上并等待用户输入。一旦我们输入一些东西并按下enter键，input()函数把我们的输入作为一个字符串返回。然后，我们使用int将这个字符串转换为整数，然后将其存储在变量guess中。实际上，int 是一个类，但现在所有你需要知道的是，您可以使用它来将一个字符串转变为一个整数(假设文本中的字符串包含一个有效的整数)。

接下来,我们比较用户猜的数和我们选择的数，如果他们相等，我们打印一条成功的消息。注意，我们使用缩进级别告诉Python语句属于哪个块。这就是为什么缩进P在ython中是如此重要。我希望你坚持"一致的缩进"的规则，好吗?

注意，if语句在最后有一个冒号——我们指示Python一个语句块将跟随其后。

然后,我们检查猜的数是否小于这个数字，如果是，我们通知用户，他们猜的数必须比那个数稍高。我们这里使用的是“elif”子句，实际上将两个相关的 if else-if else语句组合为一个语句if-elif-else，这使程序更简单且减少所需要的缩进。

elif和else语句也必须在逻辑行结束时有一个冒号，后跟相应的语句块(当然要通过适当的缩进)

你可以在if语句的if块中有另一个if语句——这称为if语句嵌套。

记住，elif 和else部分是可选的。一个最小的有效的if语句是：

```
python if True: print(是的，它为真)
```

在Python执行完成完整的if语句以及相关的elif和else子句，它移动到if包含语句的块中下一个语句块。在本例中，它是主要的块(程序开始执行的地方)，接下来的语句是 print(完成)。在这之后，Python将看到程序的结尾，并简单的完成。

尽管这是一个非常简单的程序，但你应该注意，我已经指出很多东西。所有这些都是相当的直截了当(对那些有c/c++背景的人是惊人的简单)。最初，你需要意识到所有这些事情，但经过一些练习，对它们你将感到舒服，自然将是你所有的感觉。

C/C++程序员需要注意
> 在Python中没有switch语句。您可以使用一个if..elif..else语句做同样的事(和在某些情况下,使用词典去做更快速)

### while语句

只要条件为真，while语句允许您多次执行一个语句块。while语句是被称为**循环语句**的一种。while语句可以有一个可选的else子句。

例如 (保存为while.py):

```
number = 23
running = True

while running:
    guess = int(input('输入一个整数 : '))

    if guess == number:
        print('恭喜，你猜对了。')
        running = False # 这使while循环停止
    elif guess < number:
        print('不对，你猜的有点儿小。')
    else:
        print('不对，你猜的有点儿大。')
else:
    print('while循环结束。')
    # 在这做你想做的任何事

print('完成')
```

输出:

```
D:> python while.py
输入一个整数 : 50
不对，你猜的有点儿大。
输入一个整数 : 22
不对，你猜的的点儿小。
输入一个整数 : 23
恭喜，你猜对了。
while循环结束。
完成
```

它是如何工作的：

在这个程序中，我们还是玩猜谜游戏，但优点在于，允许用户一直猜直到他猜对——每次猜测不需要重复运行该程序，正如我们在前一节中所做的。这演示了如何恰当的使用while语句。

我们移动input和if语句到while循环中，在while循环前，设置变量running为True。首先，我们检测变量running是否为True，然后往下执行相应的while块。在这个块执行完后，再检测条件，在这里是变量running，为真，我们再次执行while块，否则，我们执行可选的else块，然后执行下面的语句。

当while循环的条件变为False时--这也可能发生在条件检测时的第一次，执行else块。如果在while循环中有else子句，它将一直执行，除非你使用break语句打破循环。

在这里True和False被称为布尔类型，你可以认为它们分别相当于值1和0。

C/C++程序员注意：
> 记住， while循环可以的else子句。

### for循环

for..in语句是另一个循环语句，它迭代一个对象的序列，例如经历序列中的第一项。在后面的章节，我们将会看到更多关于序列的细节。现在，你需要知道的是一个序列只是一个有序的项目的集合。

例如 (保存为 for.py):

```
for i in range(1, 5):
    print(i)
else:
    print(`for循环结束`)
```

输出：

```
D:> python for.py
1
2
3
4
for循环结束
```

它是如何工作的：

打印一个数字*序列*。我们使用内置的range函数生成这个数字序列。

我们在这里所做的是提供两个数字，range返回一个从第一个数字到第二个数字的一个数字序列。例如, range(1,5)给出序列[1, 2, 3, 4]。默认情况下，range 步距取为1。如果我们提供第三个数字，range那么它变成了步距。例如range(1,5,2)得到[1,3]。请记住，范围扩展到第二号码，即它**不**包括第二个数字。

注意,range()生成一个数字序列，当for循环请求下一个项目时，它一次只生成一个数字。如果你想立刻看到完整的数字序列,使用list(range())。list(列表)将在数据结构中解释。

for循环然后遍历这个范围，for i in range(1,5)相当于 for i in [1, 2, 3, 4] 这就像把序列中的每一个数(或对象)分配给i,一次一个,然后为每个i值执行该语句块。在本例中，在语句块中我们只是打印它的值。

记住，else部分是可选的。当包括它时，除非遇到break语句，当for循环结束时，它执行一次。

记住,for..in循环可以作用于任何序列。在这里，我们对一个由内建的range函数生成的一个数字列表，但是一般来说，我们可以使用任何种类对象的任何类型的序列！在后面的章节，我们将详细探讨这个想法。

C/C++/Java/C#程序要注意
> Python的for循环完全不同于C/C++的for循环。C#程序员会注意到,在Python中for循环类似于c中的foreach循环C#。Java程序员会注意到，同样类似于在Java 1.5中的to for (int i : IntArray)。

> 在C/C++中，如果你想写for (int i = 0; i < 5; i++)，那么在Python中你只要写 for i in range(0,5)。正如您可以看到的,在Python中for循环更简单，更富有表现力且不易出错。

### break语句

break语句是用来*跳出*一个循环语句，即停止执行一个循环语句，即使循环条件还没有成为False或序列的项目没有被完全遍历。

很重要的一点是，如果你跳出for或while循环，任何相应的循环else块是不执行的。

例子 (保存为break.py):

```
while True:
    s = input('输入一些东西 : ')
    if s == 'quit':
        break
    print('字符串的长度是', len(s))
print('完成')
```

输出：

```
D:> python break.py
输入一些东西: Programming is fun
字符串的长度是 18
输入一些东西: When the work is done
字符串的长度是 21
输入一些东西 : if you wanna make your work also fun:
字符串的长度是 37
输入一些东西 : use Python!
字符串的长度是 12
输入一些东西 : quit
完成
```

它是如何工作的：

在这个程序中，我们重复获取用户输入的东西并打印每次输入字符串的长度。我们提供一个特殊的条件--通过检查用户输入是否是quit来结束程序。我们通过跳出k循环停止程序，达到该程序的结束位置。

输入字符串的长度可以使用内建的len函数。

记住， break语句同样适用于for循环。

### Swaroop 的诗意的Python

我在这里输入的是一个我写的、名为Swaroop的诗意的Python的迷你诗：

```
当工作完成时
编程是有趣的
如果你想让你的工作也很有趣:
    使用Python!
```

### continue语句

continue语句是用来告诉Python跳过当前循环块中其余的语句，继续循环的下一次迭代。

例子 (保存为continue.py):

```
while True:
    s = input('输入一些东西: ')
    if s == 'quit':
        break
    if len(s) < 3:
        print('太小')
        continue
    print('输入的东西有足够的长度')
    # 在这做其它各种处理...
```

输出:

```
D:> python continue.py
输入一些东西: a
太小
输入一些东西: 12
太小
输入一些东西: abc
输入的东西有足够的长度
输入一些东西: quit
```

它是如何工作的：

在这个程序中，我们接受来自用户的输入，但是只有在输入的字符串至少有3个字符时才处理。因此，我们使用内建的len函数来获得长度，如果长度小于3，通过使用continue句，我们跳过块中的其余语句。否则，在循环中的其余语句将被执行--在这做其它各种处理。

注意，continue语句同样适用于for循环。

### 小结

我们已经看到了如何使用三个控制流语句--if、while和for以及与它们相关的 break和continue语句。这些都是Python最常用的部分，因此，变得对他们感到舒适是至关重要的。

接下来，我们将学习如何创建和使用函数。


--------------------------------------------------

### 继续阅读[函数](a-byte-of-python3/function)