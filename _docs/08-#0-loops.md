---
# layout : rchive
title: "Loops"
permalink: /loops/
excerpt: "We learn about loops Syntax."
last_modified_at: 2019-02-20T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    

<hr style="border: solid 1px #dddddd ;">    

LESSON    

Loops allow you to quickly iterate over information in Python. In this lesson, we'll cover two types of loop: 'while' and 'for'.

**설명:** [ 학습방향 ]     
이 장에서는 while 문과, for문을 학습한다.     
반복문 while을 활용하여 데이타를 신속하게 처리하는 방법을 학습한다.
{: .notice--info}     
     


 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 1. While you're here    

The **`while`** loop is similar to an if statement: it executes the code inside of it if some condition is true. The difference is that the while loop will continue to execute as long as the condition is true. In other words, instead of executing if something is true, it executes while that thing is true.

Line 6 decides when the loop will be executed. So, "as long as count is less than 5," the loop will continue to execute. Line 8 increases count by 1. This happens over and over until count equals 5. 



**설명:** [ Learn ]     
• Ch1. While you're here 에서는 while 문에 대하여 학습한다.
• while 문은 if 문과 비슷하다.     
• while 문의 조건절이 True 이면, while 문 내부 구간이 실행 되는 구조이다.    
• if 문과 다른점은 while 문은 조건절 값이 True 이면, 계속 실행된다.    
• if 문은 조건절 값이 완료되면 끝난다. (i.g. 3번 실행하라고 하면 3번만 실행하고 종료)    
• while 문은 조건절 상태가 Ture(예를 들면, 0 < 5 )가 되면 무한대로 실행한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Change the loop so that it counts **from 0 up to 9** (inclusive).

* Be careful not to alter or remove the count += 1 statement. If your program has no way to increase count, your loop could go on forever and become an infinite loop which could crash your computer/browser!    


**설명:** [ Instruction ]          
• 반복문을 9(포함)까지 세는 프로그램으로 변경하라. (현재는 4까지 셈)   
• 변수 count 가 증가하지 않으면, 무한대로 반복되는 프로그램이 될 수 있다.    
• 이럴 경우 컴퓨터에 문제가 발생할 수 있으니 주의하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To make sure your loop counts up to 9, your condition should be 'count < 10' (or count <= 9).


**설명:** [ Hint ]         
• 9 까지만 실행되는 조건문을 만든다. ( count < 10 or count <= 9 )
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
count = 0

if count < 10:
  print "Hello, I am an if statement and count is", count

while count < 10:
  print "Hello, I am a while and count is", count
  count += 1
```

**설명:** [ Solution ]          
• if 문은 1번 출력한다.(조건문이 변수 count 가 10보다 작은지만 비교)    
• while 문은 9번 출력한다.(조건문이 변수 count 가 9 일때 까지, True이다.)
{: .notice--info}


**결과** 
``` 
Hello, I am an if statement and count is 0
Hello, I am a while and count is 0
Hello, I am a while and count is 1
Hello, I am a while and count is 2
Hello, I am a while and count is 3
Hello, I am a while and count is 4
Hello, I am a while and count is 5
Hello, I am a while and count is 6
Hello, I am a while and count is 7
Hello, I am a while and count is 8
Hello, I am a while and count is 9
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 2. Condition    

The **condition** is the expression that decides whether the loop is going to continue being executed or not. There are 5 steps to this program:

1. The loop_condition variable is set to True

2. The while loop checks to see if loop_condition is True. It is, so the loop is entered.

3. The print statement is executed.

4. The variable loop_condition is set to False.

5. The while loop again checks to see if loop_condition is True. It is not, so the loop is not executed a second time.    


**설명:** [ Learn ]     
• Ch2. Condition 에서는 조건절에 대하여 학습한다.    
• 조건절(loop_condition)은 반복(loop)을 계속할지 그만할지를 결정하는 표현이다.     
• 다음 5단계로 진행된다.     
• ① 조건절의 변수값을 True 로 설정한다.       
• ② 조건절의 상태가 True 이면, 반복문 안으로 들어간다.    
• ③ print문을 출력한다.     
• ④ 조건절의 상태를 False 로 설정한다.    
• ⑤ while 문의 조건절을 다시 True 인지 확인한다.(True가 아니면 반복 종료 )
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* See how the loop checks its condition, and when it stops executing? When you think you've got the hang of it, click Run to continue.


**설명:** [ Instruction ]          
• 실행이 멈췄을때, 반복문의 상태를 어떻게 확인 하는지 살펴보라.    
• 예상 한대로 실행되는지 Run을 실행해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* See how the source works.



**설명:** [ Hint ]          
• 소스가 어떻게 동작하는지 확인하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
loop_condition = True

while loop_condition:
  print "I am a loop"
  loop_condition = False
```

**설명:** [ Solution ]          
• 변수 loop_condition 을 True 로 설정한다.    
• 조건문이 True 이기에 while 문에 진입한다.    
• 'print "I am a loop" '를 출력한다.    
• 변수 loop_condition 을 강제로 False로 변경한다.    
• 다시 while 문의 조건절 loop_condition 이 True 인지 확인한다.    
• 조건문이 True 이면, while 문의 블럭문이 실행된다.    
• 조건문이 False 이면, while 문을 빠져나간다.
{: .notice--info}


**결과** 
``` 
I am a loop
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 3. While you're at it    

Inside a while loop, you can do anything you could do elsewhere, including arithmetic operations. 



**설명:** [ Learn ]         
• Ch3. While you're at it 에서는 while 문의 조건문을 추가 학습한다.    
• while 조건문 에는 사칙연산을 비롯하여 다른 곳에서 사용했던 어떤 것이든 들어갈수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a while loop that prints out all the numbers from 1 to 10 squared (1, 4, 9, 16, ... , 100), each on their own line.    
* Fill in the blank space so that our while loop goes from 1 to 10 inclusive.    
* Inside the loop, print the value of num squared. The syntax for squaring a number is num ** 2.    
* Increment num.



**설명:** [ Instruction ]          
• while 문을 사용하여 1부터 10까지 값의 제곱근 값을 출력하라.    
• while 문의 조건문을 넣는 곳에 1부터 10까지 돌도록 작성하라.       
• while 문의 내부실행 블럭에서는 'num ** 2' 제곱근 값을 출력하라.       
• 변수 num 을 1 씩 증가 시켜라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your condition will have to be num <= 10 (or num < 11) so that the loop will always print until num is 11.


**설명:** [ Hint ]          
• 조건문 num <= 10 or num < 11 로 10 이하 인지를 확인한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
num = 1

while (num <= 10):  # Fill in the condition
  # Print num squared
  	print (num ** 2)
  # Increment num (make sure to do this!)
  	num += 1
```

**설명:** [ Solution ]          
• 변수 num 에 값 1로 초기화 한다.    
• while 문에서 조건문 num <= 10 으로 정의하였다.    
• while 문 조건은 변수 num 이 10 이하 일때까지 실행한다.(True)      
• while 실행 블럭에서는 num ** 2 하여 제곱근을 구하고 출력한다.     
• 마지막으로 변수 num 을 값 1을 증가시킨다.     
• 다시, while 조건문에서 변수 num 이 10보다 같거나 작으면 실행블럭이 동작한다.(True)
{: .notice--info}



**결과** 
``` 
1
4
9
16
25
36
49
64
81
100
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 4. Simple errors    

A common application of a while loop is to check user input to see if it is valid. For example, if you ask the user to enter y or n and they instead enter 7, then you should re-prompt them for input.



**설명:** [ Learn ]         
• Ch4. Simple errors 에서는 연산자 같다( == ), 틀리다( != ) 를 학습한다.    
• 주로 while 조건문에서 사용한다.   
• 사용자가 입력한 값이 유효 한지를 체크하는 기능이다.    
• 예를들면, 당신은 사용자가 'y' or 'n' 을 입력하길 기대하고 있다.    
• 그런데, 사용자가 '7' 을 입력하면, 당신은 다시 입력하는 단계로 되돌아 갈 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Fill in the loop condition so the user will be prompted for a choice over and over while choice does not equal 'y' and choice does not equal 'n'.


**설명:** [ Instruction ]          
• Prompt 창에서 입력값이 'y' 또는 'n' 만 입력 되도록 하라.    
• while 조건문에서 통제 하도록 하라.    
• 만약 'y' or 'n' 이외의 값이 입력되면 다시 입력하도록 반복하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, use the != operator to test if two things are different, such as choice != "y", and the and operator to check more than one thing, such as A and B.


**설명:** [ Hint ]         
• 조건문에 연산자 ( != ) 를 사용한다.   
• 'y' or 'n' 이외에는 True 가 되지 않도록 한다.    
• 입력받은 비교 변수가 "y" 와 가 같지 않는지를 비교하는 것은 (i.g. !="y" ) 이다.    
• 연산자 ( and ) 는 A, B 모두 True 이어야 한다.(i.g. A and B )    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
choice = raw_input('Enjoying the course? (y/n)')

while choice != 'y' and choice != 'n':  # Fill in the condition (before the colon)
  choice = raw_input("Sorry, I didn't catch that. Enter again: ")
```

**설명:** [ Solution ]          
• 변수 choice 에 입력값을 받아 저장한다.    
• while 문에서 변수 choice 가 'y' 도 아니고, 'n'도 아니다 를 비교한다.    
• 조건문이 True 이면, 다시 입력문을 받는다.    
• 조건문이 False 이면, while 문을 실행하지 않고 빠져나간다.
{: .notice--info}



**결과** 
``` 
Enjoying the course? (y/n)x
Sorry, I didn't catch that. Enter again: z
Sorry, I didn't catch that. Enter again: y
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 5. Infinite loops    

An **infinite loop** is a loop that **never exits**. This can happen for a few reasons:

1. The loop condition cannot possibly be false (e.g. while 1 != 2)

2. The logic of the loop prevents the loop condition from becoming false.

Example:    
```python
count = 10
while count > 0:
  count += 1 # Instead of count -= 1
```



**설명:** [ Learn ]          
• Ch5. Infinite loops 에서는 무한반복(loop)을 방지하는 방법을 학습한다.    
• 무한 loop 는 프로그램을 빠져 나가지 않고 계속 반복되는 것이다.    
• 문한 loop 가 발생되는데는 다음과 같이 여러가지 이유가 있다.    
• ① 조건문 결과가 무조건 True 일때 ( while 1 !=2 )    
• ② 프로그램 로직상 false 가 발생할수 없는 경우 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* The loop in the editor has **two problems**: it's missing a colon (a syntax error) and count is never incremented (logical error). The latter will result in an infinite loop, so be sure to **fix** both before running!


**설명:** [ Instruction ]          
• while 반복문에 2개의 문제가 있다.    
• 첫째는 문법적으로 ( : ) 이 빠져 있다.    
• 둘째는 로직적으로 무한 반복이 되는 것이다.    
• 프로그램을 실행하기 전에 수정하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Since count is never incremented (count += 1), count is always 0, and since zero is less than ten, 0 will be printed over and over again forever.


**설명:** [ Hint ]          
• 변수 count 가 증가하지 않으면 count 값은 항상 0 이다.   
• while 조건문이 항상 10보다 작게 되며, 이경우, 조건문이 무조건 True가 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
count = 0

while count < 10: # Add a colon
  print count
  # Increment count
  count += 1
```

**설명:** [ Solution ]          
• 변수 count 가 0 부터 10 보다 작을때까지 변수 count를 출력하는 프로그램이다.    
• 변수 count 에 값 1을 증가시켜준다.   
• 변수 count 가 10 이 되면 while 조건문을 빠져나간다.
{: .notice--info}



**결과** 
``` 
0
1
2
3
4
5
6
7
8
9
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 6. Break    

The **break** is a one-line statement that means "exit the current loop." An alternate way to make our counting loop exit and stop executing is with the `break` statement.

* First, create a while with a condition that is always **true**. The simplest way is shown.

* Using an `if` statement, you define the stopping condition. Inside the if, you write break, meaning "exit the loop."

The difference here is that this loop is guaranteed to run at least once.





**설명:** [ ]          
`break`문을 만나면 현재 loop를 빠져나간다.    
• while문의 조건절을 항상 True 인 경우에만 진행 되도록 지정한다. Ture가 아닐때 그 loop를 빠져나간다.    

• while문의 내부 블럭에서 if문을 사용해서 멈춰도 된다. if 문에 조건을 걸어서 해당 조건이 되면 break 사용하여 해당 loop를 빠져나간다.     
이런 경우, 무조건 while 내부 내용이 1번은 실행된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** See what the break does? Feel free to mess around with it (but make sure you don't cause an infinite loop)! Click Run when you're ready to continue.


**설명:** [ ]          
① `break` 가 무슨일을 하는지 살펴보라. 가볍게 살펴보고, 실행 시켜 보아라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
count = 0

while True:
  print count
  count += 1
  if count >= 10:
    break

```

**설명:** [ ]          
변수 `count`가 10이 되면 강제로 break 문이 발동되어 loop를 빠져 나간다. 
{: .notice--info}



**결과** 
``` 
0
1
2
3
4
5
6
7
8
9
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 7. While / else    

Something completely different about Python is the **`while/else`** construction. **`while/else`** is similar to **`if/else`**, but there is a difference: the **else** block will execute anytime the loop condition is evaluated to False. This means that it will execute if the loop is never entered or if the loop exits normally. If the loop exits as the result of a break, the else will not be executed.

In this example, the loop will break if a 5 is generated, and the else will not execute. Otherwise, after 3 numbers are generated, the loop condition will become false and the else will execute.





**설명:** [ ]          
`while/else`는 python에 사용되는 독특한 구조이다.    
`if/else` 의 `else`와 비슷하지만, `if/else`는 `if`문이 실행되면 `else`문이 실행되지 않지만, `while/else`는 `while`문이 flase 되어 빠져 나오면 반드시 `else`문이 동작된다.  실습을 통해서 알아보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click Run to see while/else in action!


**설명:** [ ]          
① 실행해서, 소스가 어떻게 동작되는지를 확인해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
import random

print "Lucky Numbers! 3 numbers will be generated."
print "If one of them is a '5', you lose!"

count = 0
while count < 3:
  num = random.randint(1, 6)
  print num
  if num == 5:
    print "Sorry, you lose!"
    break
  count += 1
else:
  print "You win!"
```

**설명:** [ ]          
while문은 변수 `count`가 3보다 작을때까지 내부 블럭이 동작한다. 더불어 내부 블럭에는 변수 `num`이 5가 될때까지 실행된다.     
while문을 빠져나오면, `else`문의 `print "You win!"`이 출력된다. 
{: .notice--info}



**결과** 
``` 
Lucky Numbers! 3 numbers will be generated.
If one of them is a '5', you lose!
1
6
1
You win!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 8. Your own while / else    

Now you should be able to make a game similar to the one in the last exercise. The code from the last exercise is below:
```python
count = 0
while count < 3:
  num = random.randint(1, 6)
  print num
  if num == 5:
    print "Sorry, you lose!"
    break
  count += 1
else:
  print "You win!"
```
In this exercise, allow the user to guess what the number is 3 times.
```python
guess = int(raw_input("Your guess: "))
```
Remember, **`raw_input`** turns user input into a **string**, so we use **`int()`** to make it a number again.





**설명:** [ ]          
`while/else`문이 어떻게 사용되는지는 살펴 보자.     
참고로, `raw_input()`내재 함수는 return 값이 문자열(string)이다. 즉, 입력을 숫자로 입력해도 내부적으로는 문자열로 취급된다. 그러므로 `int(raw_input("Your guess: "))`로 숫자로 바꿔 줘야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Use a while loop to let the user keep guessing so long as guesses_left is greater than zero.

* Ask the user for their guess, just like the second example above.

* If they guess correctly, print "You win!" and break.

* Decrement guesses_left by one.

* Use an else: case after your while loop to print "You lose.".




**설명:** [ ]          
① 변수 `guesses_left`가 0 보다 클 동안 사용자가 계속 질문하는 while 문을 만든다.    
• 상단 처럼 질문하는 문을 만들자.    
• 만약, 질문한 값이 맞으면 "You win!" 이라고 출력하고, break문으로 빠져나오자.     
• 변수 `guess_left`를 1씩 줄여 나가자 `guess_left -=1`    
• `else`문을 사용하여 while 문을 빠져나오면 "You lose."라고 출력하자.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
This game will have a very similar structure to the example, but instead of losing right before the break, the user should win.

The if should check if guess == random_number. If it does, then it's the winning guess!


**설명:** [ ]          
앞의 예제와 비슷하지만, break 문이 걸리는게 이겼을때 이다.     
`if guess == random_number`인 경우가 승리하는 조건이다. 
random값은 while 문 시작 하기전에 산출된다.  
break문이 실행되어 while문을 빠져나갈때, else문은 실행되지 않는다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

# Generates a number from 1 through 10 inclusive
random_number = randint(1, 10)

guesses_left = 3
# Start your game!
while guesses_left > 0:
  guess = int(raw_input("Your guess: "))
  if guess == random_number:
    print "You win!"
    break
  guesses_left -= 1
else:
  print "You lose."

```

**설명:** [ ]          
미리 `random_number`값을 가진다.    
변수 `guess_left`가 0보다 클동안 while문이 진행된다.     
prompt 에서 `"Your guess: "`로 임의의 숫자를 입력 받는다. 입력받은 값은 변수 `guess`에 저장된다.      
`guess`값이 미리 산출한 `random_number`과 같으면 "You win!"을 출력한다.그리고 break 문이 작동되어 loop를 빠져나온다. 그렇지 않으면 변수 `guess_left`를 -1 하도 다시 loop를 돈다.     
`guesses_left` 값이 0이 되면 while문을 빠져나오고, `else`문이 실행되어 `print "You lose"`가 동작된다.  
{: .notice--info}



**결과**
`#` case : fail    
``` 
Your guess: 2
Your guess: 2
Your guess: 2
You lose.
```
`#` case : correct   
```
Your guess: 2
Your guess: 1
Your guess: 3
You win!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 9. For your health    

An alternative way to loop is the for loop. The syntax is as shown in the code editor. This example means "for each number i in the range 0 - 9, print i".



**설명:** [ ]          
앞에서 배운 for 문은 또다른 반복문이다. 즉, while문을 대체할 수 있다. edit 창에 있는 소스는  0부터 9까지 반복적으로 돌면서 산출하는 소스이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Make the loop print the numbers from 0 to 19 instead of 0 to 9.


**설명:** [ ]          
① 0부터 19까지 숫자를 출력하는 반복문으로 변경하라. (기존 0부터 9까지 산출하는 소스를 이용) 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Make sure to change the number inside of **`range`**.


**설명:** [ ]          
`rang()` 함수를 사용하자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print "Counting..."

for i in range(20):
  print i
  
  
```

**설명:** [ ]          
`range(20)` 함수는 20 미만의 숫자를 0부터 20개 출력하는 것이다. 
{: .notice--info}



**결과** 
``` 
Counting...
0
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 10. For your hobbies    

This kind of loop is useful when you want to do something a **certain number of times**, such as append something to the end of a list.



**설명:** [ ]          
for문은 내가 몇번 loop를 둘려야 하는지를 정확히 알때 사용한다. 예를 들면,
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a **`for`** loop that prompts the user for a **hobby 3 times**.

* Save the result of each prompt in a **`hobby`** variable

* append each one to `hobbies[]`.

* print hobbies after your for loop

Make sure to answer the prompts in the terminal when testing your code!


**설명:** [ ]          
① for문을 사용하여 취미를 3번 묻는 것을 만들어라.     
• 변수 `hobby`에 prompt에서 입력 받은 값을 저장하라.      
• 입력 받은 `hobby`를 리스트 `hobbies`리스트에 추가하라.    
• for 문을 빠져나오고 `hobbies`리스트 값을 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your for loop should use range(3). You should use the **`raw_input()`** function to get info from the user and **`hobbies.append(hobby)`** to add the **`hobby`** to the list.


**설명:** [ ]          
• `raw_input()`함수를 사용하라.     
• 리스트에 추가하는것은 `hobbies.append(hobby)`이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
hobbies = []

# Add your code below!

for num in range(3):
  hobby =  raw_input("Tell me one of your favorite hobbies: ")
  hobbies.append(hobby)

print hobbies
```

**설명:** [ ]          
`for num in range(3):`로 3번 입력 받는다.     
입력받은 값은 리스트 hobbies에 추가한다.    
for 문을 빠져나오면, 리스트 hobbies를 출력한다. 
{: .notice--info}



**결과** 
``` 
Tell me one of your favorite hobbies: swim
Tell me one of your favorite hobbies: ski
Tell me one of your favorite hobbies: cycle
[u'swim', u'ski', u'cycle']
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 11. For your strings    

Using a for loop, you can print out each individual character in a string.

The example in the editor is almost plain English: "for each character c in thing, print c". 



**설명:** [ ]          
loop 반복을 통하여 문자열을 문자 단위로 나눌수 있다.     
edit 창에 있는 소스는 문자열 단어를 스펠링으로 나누는 소스이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add a second for loop so that each character in **`word`** is printed one at a time.


**설명:** [ ]          
① for 문을 추가하여, 변수 `word`에 담겨 있는 "eggs"를 하나씩 출력 되게 하여라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Use the example on lines 3 - 4 as a model.


**설명:** [ ]          
3,4라인에 있는 for문을 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
thing = "spam!"

for c in thing:
  print c

word = "eggs!"

# Your code here!
for character in word:
  print character
```

**설명:** [ ]          
변수 `word`에 있는 문자열 "eggs!"를 알파벳 하나씩 읽어서 출력한다. 
{: .notice--info}



**결과** 
``` 
s
p
a
m
!
e
g
g
s
!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 12. For your A    

String manipulation is useful in for loops if you want to modify some content in a string.
```python
word = "Marble"
for char in word:
  print char,
```  
The example above iterates through each character in word and, in the end, prints out M a r b l e.

The `,` character after our print statement means that our next print statement **keeps** printing on **the same line**.





**설명:** [ ]          
for 문은 문자열 조작을 하기에 편리하다.    
예제에서 "Marble"가 M a r b l e 로 출력된다.    
여기에서 `print char ,` `,`는 문자열이 새로운 줄에서 출력되는 것이 아니라, 같은 라인에서 출력되는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's filter out the letter "A" from our string.

* Do the following for each character in the **`phrase`**.
* If char is an "A" or char is an "a", print "X", instead of char. Make sure to include the trailing comma.
* Otherwise (else:), please print char, with the trailing comma.



**설명:** [ ]          
① 문자열에서 "A"를 걸러내는 것을 해 보자.    
• 변수 `phrase`에 들어있는 문자열을 이용한다.    
• 문자 중 "A" or "a"는 해당 문자를 "X"로 출력되게끔 바꿔라. `,`를 사용하여 한줄에 출력되게 하라.        
• 그외는 `,`를 사용하여, 문자열을 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can use the same for syntax, for c in s, as before. Use an if to compare c to 'a' and 'A'. Print an 'X' in that case, and use an else to print the character otherwise.

Include a comma after the character to be printed in order to ensure it's not printed on its own line, like so:

```python
if c == "A" or c == "a":
  print "X",
```


**설명:** [ ]          
for 문을 돌면서 문자를 추출하고, 해당 문자가 "A" or "a"이면 "X"를 출력한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
phrase = "A bird in the hand..."

# Add your for loop
for char in phrase:
  if char == "A" or char == 'a':
    print 'X',
  else:
    print char,

#Don't delete this print statement!
print
```

**설명:** [ ]      
{: .notice--info}



**결과** 
``` 
X   b i r d   i n   t h e   h X n d . . .
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 13. For your lists    

Perhaps the most useful (and most common) use of for loops is to go through a list.

On each iteration, the variable **`num`** will be the next value in the list. So, the first time through, it will be **7**, the second time it will be **9**, then **12, 54, 99,** and then the loop will exit when there are no more values in the list.

 



**설명:** [ ]         
리스트를 사용할때 for 문이 많이 유용하다.     
for 문으로 리스트 `numbers`의 값들을 하나식 꺼집어 낼 수 있다. 변수 `num`에는 그 꺼집어낸 값들이 하나씩 들어 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a **second for loop** that goes through the **numbers list** and **prints** each **element squared**, each on its own line.




**설명:** [ ]          
① 두번째 for 문을 통하여, `numbers`의 값들을 꺼내어 그 값의 제곱근을 구하여 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Use the **`**`** operator for exponentiation. The rest of the loop should be very similar to the first one.


**설명:** [ ]          
`**`를 사용하여 제곱근을 구하라. for문 사용법은 첫번째 for문과 비슷하다. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
numbers  = [7, 9, 12, 54, 99]

print "This list contains: "

for num in numbers:
  print num

# Add your loop below!
for num in numbers:
  print num ** 2
```

**설명:** [ ]          
변수 `numbers`에 있는 값을 변수`num`에 넣고, `num`을 제곱근을 구하여 출력한다. 
{: .notice--info}


**결과** 
``` 
This list contains: 
7
9
12
54
99
49
81
144
2916
9801
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 14. Looping over a dictionary    

You may be wondering how looping over a dictionary would work. Would you get the key or the value?

The short answer is: you get the key which you can use to get the value.
```python
d = {'x': 9, 'y': 10, 'z': 20}
for key in d:
  if d[key] == 10:
    print "This dictionary has the value 10!"
```    
1. First, we create a dictionary with strings as the keys and numbers as the values.
2. Then, we iterate through the dictionary, each time storing the key in key.
3. Next, we check if that key's value is equal to 10.
4. If so, we print "This dictionary has the value 10!"




**설명:** [ ]          
딕셔너리의 경우 반복문을 어떻게 사용하는지를 알아보자. 먼저 간단하게 이야기하면, key 로 값을 얻어 낼수 있다.  
① 먼저, key와 value로 구성된 딕셔너리를 만든다.      
② 딕셔너리의 key를 반복적으로 꺼낸다.    
③ 꺼낸 key의 value 값이 10인지를 비교한다.    
④ value 값이 10이면 "This dictionary has the value 10!"    
x{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 5, print the **key**, followed by a space, followed by the value associated with that key.


**설명:** [ ]          
① 5라인에서, key를 출력하고, 공백을 하나 뛰고 key의 value를 출력하시오.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
An easy way to print in the requested format is to use the , character, like so:
```python
greeting = "Hello"
name = "World"

print greeting, name
# prints "Hello World"
```

**설명:** [ ]          
`,`를 사용하면, 같은 줄에 출력 할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
d = {'a': 'apple', 'b': 'berry', 'c': 'cherry'}

for key in d:
  # Your code here!
  print key, d[key]
```

**설명:** [ ]          
`key`는 'a'이고, 그 값은 `d[key]`로 나타 낼수 있다.  
{: .notice--info}


**결과** 
``` 
a apple
c cherry
b berry
```



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 15. Counting as you go    

A weakness of using this for-each style of iteration is that **you don't know the index** of the thing you're looking at. Generally this isn't an issue, but at times it is useful to know how far into the list you are. Thankfully the built-in **`enumerate`** function helps with this.

**`enumerate`** works by supplying a corresponding index to each element in the list that you pass it. Each time you go through the loop, index will be one greater, and item will be the next item in the sequence. It's very similar to using a normal for loop with a list, except this gives us an easy way to count how many items we've seen so far.



**설명:** [ ]         
for 문을 돌려 리스트의 항목을 뽑아 내더라도, 그 뽑아낸 값의 인덱스는 알려주지 않는다. 다만 그 값만 뽑아 내 준다. 이러한 약점은 `enumerate`내재 함수를 사용하면 해당 값의 인덱스 값을 알수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** We don't want the user to see things listed from index 0, since this looks unnatural. Instead, the items should appear to start at index 1. Modify the print statement to reflect this behavior. See the Hint for help. 


**설명:** [ ]          
① 리스트의 index를 출력하면 0부터 출력된다. 그런데, 우리는 흔히 4가지중 하나를 고를때 리스트 번호를 1번 부터 번호를 매기는게 더 자연스럽다. 비록 index값이 0부터 출력되지만, print 할때는 1부터 하는것 처럼 보이게 하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Instead of just printing index, print index + 1!


**설명:** [ ]          
출력할때, index 값에 +1을 하여라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
choices = ['pizza', 'pasta', 'salad', 'nachos']

print 'Your choices are:'
for index, item in enumerate(choices):
  print index + 1, item
```

**설명:** [ ]          
index 값에 +1을 하여 1 부터 보이게 한다. 
{: .notice--info}


**결과** 
``` 
Your choices are:
1 pizza
2 pasta
3 salad
4 nachos
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 16. Multiple lists    

It's also common to need to iterate over **two lists at once**. This is where the built-in **`zip`** function comes in handy.

**`zip`** will create pairs of elements when passed two lists, and will **stop at the end of the shorter list**.

**`zip`** can handle three or more lists as well!




**설명:** [ ]          
한번에 두개의 리스트를 반복적으로 사용해야 할 경우에, 우리는 `zip` 내장 함수를 이용할수 있다.     
`zip`은 2개의 리스트를 쌍으로 만들어주고, 잛은 리스트의 기준에 맞춰진다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Compare each pair of elements and print the larger of the two.


**설명:** [ ]          
① 각 원소들의 쌍을 비교하고, 두개중 더 큰것을 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
**`a`** is an element from **`list_a`** and **`b`** is an element of **`list_b`**.

You have two options: Use an **`if/else`** statement to compare the two and print whichever is larger. Alternatively, you can use the **`max`** function that you learned in unit 4.


**설명:** [ ]          
list_a를 변수 a로 받고, list_b를 변수 b로 값을 받는다. 그리고 각각의 변수를 `if/else`를 사용하여 어느것이 더 큰지를 비교한다. (또는 내장함수 `max()`를 활용해도 된다.)
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
list_a = [3, 9, 17, 15, 19]
list_b = [2, 4, 8, 10, 30, 40, 50, 60, 70, 80, 90]

for a, b in zip(list_a, list_b):
  # Add your code here!
    print max(a, b)
```

**설명:** [ ]          
각각의 리스트를 변수 a, b로 받아서, `max(a,b)`를 비교하여 큰값을 출력한다.
{: .notice--info}


**결과** 
``` 
3
9
17
15
30
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 17. For / else    

Just like with **`while`**, **`for`** loops may have an else associated with them.

In this case, the **`else`** statement is executed after the **`for`**, but only **`if`** the **`for`** ends normally—that is, not with a **`break`**. This code will break when it hits 'tomato', so the **`else`** block won't be executed.



**설명:** [ ]          
`for` 반복절은 `else`를 가질수 있다. `for`문이 다 실행되고, 빠져나오면 마지막으로 `else`문이 실행된다. 단, `for`문에서 `break`가 발생되면, `else`문은 실행되지 않는다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click Run to see how for and else work together.


**설명:** [ ]          
① `Run`을 실행시켜, 소스가 어떻게 동작되는지 확인한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
fruits = ['banana', 'apple', 'orange', 'tomato', 'pear', 'grape']

print 'You have...'
for f in fruits:
  if f == 'tomato':
    print 'A tomato is not a fruit!' # (It actually is.)
    break
  print 'A', f
else:
  print 'A fine selection of fruits!'
```

**설명:** [ ]          
`for`문을 돌면서, 리스트 `fruits`의 값이 "tomato" 이면 "A tomato is not a fruit!"가 출력되고 `break`가 실행된다. 이 경우는 `else`가 실행되지 않는다. 만약에 `for`문에서 `break`가 안걸리고 정상적으로 다 돌게 되면, `else`가 마지막에 실행된다.
{: .notice--info}



**결과** 
```
# break 문을 만난 경우 
You have...
A banana
A apple
A orange
A tomato is not a fruit!
```
**결과** 
```
# break 문을 만나지 못한  경우 
You have...
A banana
A apple
A orange
A tomato
A pear
A grape
A fine selection of fruits!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 18. Change it up 

As mentioned, the **`else`** block won't run in this case, since break executes when it hits **'tomato'**.



**설명:** [ ]          
`break`문이 실행되면(즉, 'tomato'가 있으면), `for/else`의 `else`는 실행되지 않는다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Modify the code in the editor such that the **`for`** loop's **`else`** statement is executed.


**설명:** [ ]          
① `for`문의 `else`구문이 동작되도록 소스를 수정하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can change the contents of fruits or the contents of the for statement such that the loop doesn't break on "tomato".


**설명:** [ ]          
리스트 `fruits`의 내용이 'tomato'가 없게 하거나, `if`문에서 'tomato'가 일치 하지 않게 만들어, `break`문이 작동하지 않게 하면, `else`문이 실행된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
fruits = ['banana', 'apple', 'orange', 'tomato', 'pear', 'grape']

print 'You have...'
for f in fruits:
  if f == 'tomato':
    print 'A tomato is not a fruit!' # (It actually is.)
  print 'A', f
else:
  print 'A fine selection of fruits!'
```

**설명:** [ ]          
이 경우엔, `break`문을 삭제 했다. `for`문이 실행되고, `else`문도 실행 된다.
{: .notice--info}


**결과** 
``` 
You have...
A banana
A apple
A orange
A tomato is not a fruit!
A tomato
A pear
A grape
A fine selection of fruits!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 19. Create your own    

To wrap up this lesson, let's create our own **`for/else`** statement from scratch.




**설명:** [ ]          
지금까지 배운것을 종합하여, `for/else`문을 활용하여 자신만의 소스를 만들어 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Build your **`for/else`** statement in the editor. Execution of the **`else`** branch is optional, but your code should print a string of your choice to the editor regardless.


**설명:** [ ]          
①  `for/else`문을 사용하여 프로그램을 짜 보자. `else`문이 실행되고 안되고는 자유다. 하지만, 당신이 원하는대로 출력이 되어야 한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
test = ["bleh", "blah", "bloh"]

for x in test:
    print x
else:
    print "ok"
```

**설명:** [ ]          
리스트 `test`에 3개의 값을 넣고, `for/else`문을 돌린다. 변수 `x`에 리스트이 값을 하나씩 추출하여, 출력하고, `for` 문이 다 돌고 나면, 마지막에 `else`문이 실행된다.
{: .notice--info}


**결과** 
``` 
bleh
blah
bloh
ok
```


<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>