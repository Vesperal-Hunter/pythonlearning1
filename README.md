课堂笔记（未整理）
名字开头是数字违法。_经常用到。
my_age += 1
------------
my_age = my_age + 1

修改后面的序号可以找回原来写过的程序
def---define定义一个function
parenthesis list of perameters
indented下一行注意

return
符号间要有空格
不然不行，

main impportant
冒号
缩进
return

3.2
debug调试

3.3
string-str去空格


4.1

boolean
not and or
<
>
<=
>=
==
!=

4.2
是进行程序设定的
具体操作，第一行记得加冒号！！
print 文本要记得加“”
if, elif, else 这些都要记得加：
且下一行开始位置要缩进，缩进多少没关系，但一定要缩进！！

4.3
讲各种错的处理方法

用random之前要加
import random

attribute errors

pi要小写

计算不能加“”比如“2+2”就是错的。
=是计算
而==是比较变量


三个双引号可以换行写注释
"""
ahfaskjghaldjfal
dafshdskj
"""

如果有if 要给定else
不然会有none出现没有信息的情况。
4.4是教如何做猜拳软件
没时间暂时过掉，之后做

5.1
编程模型
event driven program model

events:
input:button text book
keboard: key down key up
mouse: click drge
timer

event______handler

5.2
全局变量和局部变量的区别和用法
尽量用local

5.3
simplegui
program structure

globals(state)
helper functions
classes (later)
define event hanlders
create a frame
register event hanlders
start frame &times


6.1

import simplegui

store = 12
operand = 3

def output():
    print "store =", store
    print "operand =" , operand
    print ""

def swap():
    global store, operand
    store, operand = operand, store
    output()

def add():
    global store, operand
    store = store + operand
    output()

def sub():
    global store, operand
    store = store - operand
    output()

def mult():
    global store, operand
    store = store * operand
    output()

def div():
    global store, operand
    store = store / operand
    output()

def enter(inp):
    global operand
    operand = inp
    output()

frame = simplegui.create_frame("caculator", 200, 200)

frame.add_button("Print", output, 100)
frame.add_button("Swap ", swap, 100)
frame.add_button("Add ", add, 100)
frame.add_button("Sub", sub, 100)
frame.add_button("Mult ", mult, 100)
frame.add_button("Div", div, 100)
frame.add_input("Enter operand", enter, 100)

frame.start()


operand = inp 这里不对，inp这里是string不是数字运算
要用operand = int(inp)这个是无法计算小数点的。
operand = float(inp)这个可以计算小数点
 

6.3
global和local

New game. Range is from 0 to 100
Number of remaining guesses is 7

Guess the number

f = simplegui.create_frame("Gusess the number", 200, 200)

6.5
首先根据视频课程大致了解了整个流程和框架

核心是就是输入的数与随机random的数比较大小
用if，elif连接并输出。

不过两个范围转化怎么搞不清楚，而且有个每尝试一次少一个数的部分。
这里并不知道怎么搞==

所以，我先不一搞出这个，先一步步来，先做一个能再100内猜的游戏。

名字开头是数字违法。_经常用到。
my_age += 1
------------
my_age = my_age + 1

修改后面的序号可以找回原来写过的程序
def---define定义一个function
parenthesis list of perameters
indented下一行注意

return
符号间要有空格
不然不行，

main impportant
冒号
缩进
return

3.2
debug调试

3.3
string-str去空格


4.1

boolean
not and or
<
>
<=
>=
==
!=

4.2
是进行程序设定的
具体操作，第一行记得加冒号！！
print 文本要记得加“”
if, elif, else 这些都要记得加：
且下一行开始位置要缩进，缩进多少没关系，但一定要缩进！！

4.3
讲各种错的处理方法

用random之前要加
import random

attribute errors

pi要小写

计算不能加“”比如“2+2”就是错的。
=是计算
而==是比较变量


三个双引号可以换行写注释
"""
ahfaskjghaldjfal
dafshdskj
"""

如果有if 要给定else
不然会有none出现没有信息的情况。
4.4是教如何做猜拳软件
没时间暂时过掉，之后做

5.1
编程模型
event driven program model

events:
input:button text book
keboard: key down key up
mouse: click drge
timer

event______handler

5.2
全局变量和局部变量的区别和用法
尽量用local

5.3
simplegui
program structure

globals(state)
helper functions
classes (later)
define event hanlders
create a frame
register event hanlders
start frame &times


6.1

import simplegui

store = 12
operand = 3

def output():
    print "store =", store
    print "operand =" , operand
    print ""

def swap():
    global store, operand
    store, operand = operand, store
    output()

def add():
    global store, operand
    store = store + operand
    output()

def sub():
    global store, operand
    store = store - operand
    output()

def mult():
    global store, operand
    store = store * operand
    output()

def div():
    global store, operand
    store = store / operand
    output()

def enter(inp):
    global operand
    operand = inp
    output()

frame = simplegui.create_frame("caculator", 200, 200)

frame.add_button("Print", output, 100)
frame.add_button("Swap ", swap, 100)
frame.add_button("Add ", add, 100)
frame.add_button("Sub", sub, 100)
frame.add_button("Mult ", mult, 100)
frame.add_button("Div", div, 100)
frame.add_input("Enter operand", enter, 100)

frame.start()


operand = inp 这里不对，inp这里是string不是数字运算
要用operand = int(inp)这个是无法计算小数点的。
operand = float(inp)这个可以计算小数点
 


6.3
global和local

New game. Range is from 0 to 100
Number of remaining guesses is 7

Guess the number

f = simplegui.create_frame("Gusess the number", 200, 200)

6.5
首先根据视频课程大致了解了整个流程和框架

核心是就是输入的数与随机random的数比较大小
用if，elif连接并输出。

不过两个范围转化怎么搞不清楚，而且有个每尝试一次少一个数的部分。
这里并不知道怎么搞==

所以，我先不一搞出这个，先一步步来，先做一个能再100内猜的游戏。


尝试过程（未整理）

# template for "Guess the number" mini-project
# input will come from buttons and an input field
# all output for the game will be printed in the console
import simplegui
import random
import math

版本一：
 # initialize global variables used in your code here
num_range = 100
# helper function to start and restart the game
def new_game():
    global num_range
    print "New game. Range is from 0 to 100"
    random.randrange(1, 100)

def range100():
    # button that changes the range to [0,100) and starts a new game 
    print "New game. Range is from 0 to 100"

def get_input(guess):
    print "Guess was", guess
    if guess == random.randrange:
        print "correct!"
    elif guess < random.randrange:
        print "higher"
    elif guess > random.randrange:
        print "lower"
    output()

frame = simplegui.create_frame("Guess the number", 200, 200)
frame.add_button("Range is [0, 100)", range100, 200)
frame.add_button("Enter a guess", get_input, 200)

# register event handlers for control elements and start frame

# call new_game 
new_game()


# always remember to check your completed program against the grading rubric


版本二

# template for "Guess the number" mini-project
# input will come from buttons and an input field
# all output for the game will be printed in the console
import simplegui
import random
import math

 # initialize global variables used in your code here
num_range = 100
x =  0
# helper function to start and restart the game
def new_game():
    global num_range
    print "New game. Range is from 0 to 100"
    random.randrange(1, 100)
    
 # define event handlers for control panel
def range100():
    random(num_range)
    # button that changes the range to [0,100) and starts a new game 
    print "New game. Range is from 0 to 100"
    output()

    
def enter(guess):
    global x
    x = float(guess)
    if x == num_range:
        print "correct!"
    elif x < num_range:
        print "higher"
    elif x > num_range:
        print "lower"
    return x
    

frame = simplegui.create_frame("Guess the number", 200, 200)
frame.add_button("Range is [0, 100)", range100, 200)
frame.add_input("Enter a guess", enter, 200)




这个版本我调出了output可以输入了，但是random那里还是没有解决，
我不太懂global那里定义的num_range = 100是什么意思。
此时发现，现在就是100成了答案==没有随机到。

def new_game():
    global num_range
    print "New game. Range is from 0 to 100"
    num_range = random.randint(1, 100)
    return num_range

查看doc之后我发现可能是这样。然后成功做了一个猜100没计数的小程序，算是成功了第一步~
这里要特别主要加return，但我不太清楚return到底是什么意思？？？
反正我就return到global那个用到的参数==



然后我调试第一个“Range is [0, 100)”这个键
这里我直接复制了上面的内容，发现没问题。
所以，这个目前也成功。

开始尝试加1000范围的。直接复制上面“Range is [0, 100)”的内容加个0
发现没有问题哈哈哈哈哈~~
把这个存为版本三

import simplegui
import random
import math

 # initialize global variables used in your code here
num_range = 100
x =  0
# helper function to start and restart the game
def new_game():
    global num_range
    print "New game. Range is from 0 to 100"
    num_range = random.randint(1, 100)

def range100():
    global num_range
    print "New game. Range is from 0 to 100"
    num_range = random.randint(1, 100)
    return num_range

def range1000():
    global num_range
    print "New game. Range is from 0 to 1000"
    num_range = random.randint(1, 1000)
    return num_range
    
def enter(guess):
    global x
    x = float(guess)
    if x == num_range:
        print "correct!"
    elif x < num_range:
        print "higher"
    elif x > num_range:
        print "lower"
    return x

frame = simplegui.create_frame("Guess the number", 200, 200)
frame.add_button("Range is [0, 100)", range100, 200)
frame.add_button("Range is [0, 1000)", range1000, 200)
frame.add_input("Enter a guess", enter, 200)


new_game()


接下来我要尝试更复杂的加工，让这个程序变得丰满一些。比如那个计数==

我奇怪为什么视频只有一个global参数，看来个x不需要？？但是我要输入的话貌似又需要。这里先不管。
先加上    print "Guess was", x
测试一下发现没问题，但这里应该不用float即可，改为了int，发现ok。
比较美观了，然后我想加一个如果输入非数字提示的东西改成了：
def enter(guess):
    global x
    x = int(guess)
    print "Guess was", x
    if x == num_range:
        print "Correct!"
    elif x < num_range:
        print "Try a higher value"
    elif x > num_range:
        print "Try a lower value."
    else:
        print "just have fun"
    return x

发现不对报错了：Line 31: ValueError: invalid literal for int() with base 10: 'd'
我发现我没必要定义一个x啊，换回num_range,然后我发现自己乱了==
这个我开始游戏的时候num_range已经定义了，这里应该只是我多定义一个x即可。不用全局搞，但这里又
报错---
所以我又调回了原来的全局，还是先能用即可==
那么我再搞一个提示次数。这里我想应该有一个按回车就计数的程序，所以去查了count，发现好像不对，都是引入collect相关的内容。
再想到tick或者enter也不行==
原理上是我没回车上面的数就减少一个，想起提示给的math还没用，看了一下，并没思路，想起我coursera上的指示还没看。这里我陡然发现一个
问题，上面的提示有问题--，这里光搞一个higher也不知道是我输入结果高了还是我需要需要输入一个更高的值，或者是我英语不好==
我把提示改了一下。
看完指示我发现被视频里那个num_range名字误导了啊，应该先看课程介绍，这个num_range就是要猜的数，之后详细看病看code clinic才发现这个其实
是为了限制猜的范围的。
根据课程要求，我基本做完主框架，但还有两点没搞定。
上面提到用math.log和math.ceil来做，看来仔细阅读这个项目介绍太重要了，如果我先读的话，效率会高很多，不过可能少了一些乐趣==
看了上面俩个函数，不知道要干什么。怎么从猜对直接回去也还是没思路。
到这里已经不会了。。。开始翻群邮

为什么这里价格n = n - 1就行，啊是啊，不用上面enter键相关啊，这里是编程啊，这个n = n - 1 显然不是数学上的意思，我要回去看global和local那，记得有讲。


最终版本
# template for "Guess the number" mini-project
# input will come from buttons and an input field
# all output for the game will be printed in the console
import simplegui
import random
import math

 # initialize global variables used in your code here
num_range = 100
secret_number = 0
x = 0
remaining_number = 0
# helper function to start and restart the game
def new_game():
    global secret_number, remaining_number
    remaining_number = 7
    secret_number = random.randint(1, 100)
    num_range = 1000
    print "New game. Range is from 0 to 100"
    print "Number of remaining is 7" 
    print ""
    
def range100():
    global secret_number, num_range
    global remaining_number
    num_range = 100
    print "New game. Range is from 0 to 100"
    print "Number of remaining is 7"
    secret_number = random.randint(1, 100)
    remaining_number = 7
   

def range1000():
    global secret_number, num_range
    global remaining_number
    print "New game. Range is from 0 to 1000"
    print "Number of remaining is 10 "
    secret_number = random.randint(1, 1000)
    num_range = 1000
    remaining_number = 10
    return secret_number
    
def enter(guess):
    global secret_number
    global x
    global remaining_number
    x = int(guess)
    print "Guess was", x
    remaining_number = remaining_number - 1
    if x == secret_number:
        print "Correct!"
        print ""
    elif remaining_number < 1:
        print "Gime over! "
        print "Restart by clicking the uper button."
    elif x < secret_number:
        print "Number of remaining is", remaining_number
        print "Try a higher value."
        print ""
    elif num_range > x > secret_number:
        print "Number of remaining is", remaining_number
        print "Try a lower value."
        print ""
    elif x > num_range:
        print "Number of remaining is", remaining_number
        print "Your guess is out of the range "
        print ""
    
    else:
        print "[0, x) do not contain x"
        print "Number of remaining is", remaining_number
        print ""

# create frame
frame = simplegui.create_frame("Guess the number", 200, 200)
frame.add_button("Range is [0, 100)", range100, 200)
frame.add_button("Range is [0, 1000)", range1000, 200)
frame.add_input("Enter a guess", enter, 200)

# register event handlers for control elements and start frame

# call new_game 
new_game()

# always remember to check your completed program against the grading rubric



