---
# layout : rchive
title: "Conditionals and Control Flow"
permalink: /conditionals-control-flow/
excerpt: "We learn about Conditionals, Control Flow Syntax."
last_modified_at: 2018-11-27T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
    
<hr style="border: solid 1px #dddddd ;">


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 
### 1. Go With the Flow

Just like in real life, sometimes we'd like our code to be able to make decisions.

The Python programs we've written so far have had one-track minds: they can add two numbers or print something, but they don't have the ability to pick one of these outcomes over the other.

**Control flow** gives us this ability to choose among outcomes based on what else is happening in the program.




**설명:** 현재까지, 우리는 Python의 여러가지 기능, 출력, 사칙연사, 문자열 처리 등을 을 연습했다.
지금부터는 우리는 **Control flow** 기능을 통하여 Python 프로그램에서 다중 선택을 할수 있는 방법을 연습한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Check out the code in the editor. You'll see the type of program you'll be able to write once you've mastered control flow. Click `Run` to see what happens!


**설명:** ① `Run` 시켜 Python 프로그램이 어떻게 동작 되는지 보아라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
**skip**


**설명:** `skip`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def clinic():
    print "You've just entered the clinic!"
    print "Do you take the door on the left or the right?"
    answer = raw_input("Type left or right and hit 'Enter'.").lower()
    if answer == "left" or answer == "l":
        print "This is the Verbal Abuse Room, you heap of parrot droppings!"
    elif answer == "right" or answer == "r":
        print "Of course this is the Argument Room, I've told you that already!"
    else:
        print "You didn't pick left or right! Try again."
        clinic()

clinic()
```

**설명:** 출력 창에서, right or r, left or l, or Enter를 입력하면 Python 프로그램에서 만들어 놓은 대로 출력 될 것이다. 
{: .notice--info}


**결과**
```
You've just entered the clinic!
Do you take the door on the left or the right?
Type left or right and hit 'Enter'.
```
<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 2.  Compare Closely!

Let's start with the simplest aspect of control flow: comparators. There are six:

Equal to (`==`)

```python
>>> 2 == 2
True
>>> 2 == 5
False
```


Not equal to (`!=`)

```python
>>> 2 != 5
True
>>> 2 != 2
False
```


Less than (`<`)

```python
>>> 2 < 5
True
>>> 5 < 2
False
```


Less than or equal to (`<=`)

```python
>>> 2 <= 2
True
>>> 5 <= 2
False
```


Greater than (`>`)

```python
>>> 5 > 2
True
>>> 2 > 5
False
```

Greater than or equal to (>=)

```python
>>> 5 >= 5
True
>>> 2 >= 5
False
```

Comparators check if a value is (or **is not**) **equal** to, **greater than** (or **equal** to), or **less than** (or **equal** to) another value.

Note that `==` compares whether two things are **equal**, and `=` assigns a value to a variable.



**설명:** `==` 같다, `!=` 같지 않다, `>` 크다, `>=` 크거나 같아, `<` 작다, `<=` 작거나 같다  `==`와 `=`는 틀린 표현이다. `==`는 ex) A == B, A와 B가 같은지를 표현하는 것이고, ex) A=3, 은 변수 A에 값 3을 넣으라는 뜻이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Set each variable to `True` or `False` depending on what you think the result will be. For example, `1 < 2` will be `True`, because **one** is **less than two**.

* Set bool_one equal to the result of 17 < 328
* Set bool_two equal to the result of 100 == (2 * 50)
* Set bool_three equal to the result of 19 <= 19
* Set bool_four equal to the result of -22 >= -18
* Set bool_five equal to the result of 99 != (98 + 1)



**설명:** ① 변수 `bool_one`, `bool_two`, `bool_three`, `bool_four`, `bool_five`에 `17 < 328`, `100==(2*50)`, `19 <= 19`, `-22 >= -18`, `99 !=(98+1)`의 계산값을 `True` or `False`로 각각 대입하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, you set variables like this:
```python
bool_one = True
```
Keep in mind that checking for equality uses a double equals sign:
```python
True == True
```


**설명:** 변수에 `True` or `False` 값을 대입하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
# skip
```

**설명:** 각 변수에 결과값이 맞으면 `True`, 틀리면 `False`를 대입하라. 
{: .notice--info}

**결과** 
```
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 3. Compare... Closelier!

Excellent! It looks like you're comfortable with **basic expressions** and **comparators**.

But what about extreme expressions and comparators?



**설명:** 대입과 `=` 와 `==`는 완전히 틀리다는 것을 안다. 수식을 표현하는것 ex) (3 + 2) x 100 과 비교하는것 ex) 3 > 2 를 Python 에서는 어떻게 표현하는지 이해해 본다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's run through the comparators again with more complex expressions. Set each variable to True or False depending on what you think the result will be.

* Set bool_one to the result of (20 - 10) > 15
* Set bool_two to the result of (10 + 17) == 3**16
* Set bool_three to the result of 1**2 <= -1
* Set bool_four to the result of 40 * 4 >= -4
* Set bool_five to the result of 100 != 10**2


**설명:** ① 각 변수에 각 계산을 할 경우 예상되는 결과값을 `True` or `False`로 각각 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
An Expression (20-10) > 15 is `False` 
```python
bool_one = False
```

**설명:** 수식 (20-10) >  15 , 10 > 15라는 표현은 틀린 표현이다. 즉 `False` 이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Assign True or False as appropriate on the lines below!

# (20 - 10) > 15
bool_one = False    # We did this one for you!

# (10 + 17) == 3 ** 16
# Remember that ** can be read as 'to the power of'. 3 ** 16 is about 43 million.
bool_two = False

# 1**2 <= -1
bool_three = False

# 40 * 4 >= -4
bool_four = True

# 100 != 10**2
bool_five = False
```

**설명:** 각 주석의 값을 `True` 인지 `False`인지를 판단해 보고, 그 결과값을 해당 변수에 대입한다. 
{: .notice--info}



**결과** 
```
#skip
```
<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 4. How the Tables Have Turned

Comparisons result in either `True` or `False`, which are **booleans** as we learned before in this exercise.
```python
# Make me true!
bool_one = 3 < 5
```
Let's switch it up: we'll give the boolean, and you'll write the expression, just like the example above.




**설명:** 이전에 우리는 `boolean`에 대하여 잠시 공부한적이 있다. Python은 수식을 변수에 대합하면(ex bool_one = 3 < 5) 그 결과 값이 참(True)인지 거짓(False)인지를 판단하여 해당 변수에 참 (True) 또는 거짓(False) 값이 대입된다. 우리는 변수 `bool_one`에 어떤 값이 들어 가 있을지를 생각해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
**①** For each boolean value in the editor, write an expression that evaluates to that value. Remember, comparators are: `==`, `!=`, `>`, `>=`, `<`, and `<=`.

Use at least three different ones!

Don't just use `True` and `False`! That's cheating!

 


**설명:** ① 주석을 보고, 주석에서 수식을 참(True)으로 만들라고 하면 `==`, `!=`, `>`, `>=`, `<`, `<=`를 사용하여 다음 예제와 같이 ex) bool_one = 3 < 5  참(True)을 만든다. 각 비교수식을 사용하여 표현하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
bool_two should store a false expression, so you could try:

bool_two = 8 < 7


**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    
```python
# Create comparative statements as appropriate on the lines below!

# Make me true!
bool_one = 3 < 5  # We already did this one for you!

# Make me false!
bool_two = 99 == "lettuce"

# Make me true!
bool_three = 44 / 2 <= 43

# Make me false!
bool_four = "potato" != "potato"

# Make me true!
bool_five = "tomato" == "tomato"
```

**설명:** 주석에서 요구하는 참(True), 거짓(False)을 비교수식을 통하여 만든다. 
{: .notice--info}



**결과** ``` ```
```
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 5. To Be and/or Not to Be

**Boolean** operators compare statements and result in boolean values. There are three boolean operators:

1 **and**, which checks if both the statements are True;
2 **or**, which checks if at least one of the statements is True;
3 **not**, which gives the opposite of the statement.
We'll go through the operators one by one.


**설명:** Boolean에는 `and`, `or`, `not` 이 있다. 다음 아래의 boolean 표를 참조하자. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/03-boolean-00.svg)    

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)  

**①** Check out the truth tables to the right. They show the results of using AND, OR, and NOT boolean operators given the boolean inputs A and B.

Click next to continue. 

**설명:** ① Boolean 표를 보고, boolean이 어떻게 동작되는지를 공부해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
**skip


**설명:** `skip`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
#skip
```

**설명:** `skip`
{: .notice--info}



**결과** 
```
#skip
```
<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 6. And

The boolean operator and returns `True` when the expressions on both sides of `and` are `true`. For instance:

* 1 < 2 and 2 < 3 is True;
* 1 < 2 and 2 > 3 is False.


**설명:** `And` 는 `and` 연산자 양 쪽의 값이 모두 참(True)이면, 참(True)이다. 한쪽이라도 거짓(False)이면 거짓(False)이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png) 

**①** Let's practice with `and`. Assign each variable to the appropriate `boolean` value.


* Set `bool_one` equal to the result of 
``` python
`False` and `False` 
```
* Set `bool_two` equal to the result of
```python
 `-(-(-(-2))) == -2` and `4 >= 16 ** 0.5`
```
* Set `bool_three` equal to the result of 
```python
`19 % 4 != 300 / 10 / 10` and `False`
```
* Set `bool_four` equal to the result of
```python
`-(1 ** 2) < 2 ** 0` and `10 % 10 <= 20 - 10 * 2`
```
* Set `bool_five` equal to the result of 
```python
`True` and `True`
```
   

**설명:** ① `AND` 연산자 양변의 계산하여, 각 변수에 양 변의 계산으로 예상되어 지는 참(True), 거짓(False)을 대입하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
bool_one = False and False
```


**설명:** 변수 `bool_one` 에 거짓(False) and 거짓(False)을 대입해 본다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
bool_one = False and False

bool_two = -(-(-(-2))) == -2 and 4 >= 16 ** 0.5

bool_three = 19 % 4 != 300 / 10 / 10 and False

bool_four = -(1 ** 2) < 2 ** 0 and 10 % 10 <= 20 - 10 * 2

bool_five = True and True
```

**설명:** Python은 오른쪽의 결과 값이 참(True) or 거짓(False)을 계산하여 각 변수에 저장된다. `and` 연산자는 양 변이 모두 참(True)여야, 참(Ture)를 반환한다. 
{: .notice--info}



**결과** 
```
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 7. Or

The **boolean** operator or returns `True` when at least one expression on either side of or is true. For example:
```python
1 < 2 or 2 > 3 is True;
1 > 2 or 2 > 3 is False.
```


**설명:** `OR` 연산자는 양 변이 하나라도 참(True)이면 참(True)를 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Time to practice with or!

Set bool_one equal to the result of
```python
2 ** 3 == 108 % 100 or 'Cleese' == 'King Arthur'
```
Set bool_two equal to the result of
```python
True or False
```
Set bool_three equal to the result of
```python
100 ** 0.5 >= 50 or False
```
Set bool_four equal to the result of
```python
True or True
```
Set bool_five equal to the result of
```python
1 ** 100 == 100 ** 1 or 3 * 2 * 1 != 3 + 2 + 1
```

**설명:** ① `OR` 연산자는 양변의 계산하여, 각 변수에 양 변의 계산으로 예상되어 지는 참(True), 거짓(False)을 대입하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Remember, or is True when either (or both!) of the expressions involved are true.

**설명:** `OR`의 경우 양변중 하나라도 참(True)이면 참(True)이 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
bool_one = 2**3 == 108 % 100 or 'Cleese' == 'King Arthur'

bool_two = True or False

bool_three = 100**0.5 >= 50 or False

bool_four = True or True

bool_five = 1**100 == 100**1 or 3 * 2 * 1 != 3 + 2 + 1
```

**설명:** `OR` 연산자 양 변의 값이 계산되어 자동으로 참(True), 거짓(False)값이 변수에 대입된다. 
{: .notice--info}



**결과** 
```
#skip 
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 8. Not

The **boolean** operator `not` returns `True` for `false` statements and `False` for `true` statements.

For example:

not `False` will evaluate to `True`, while not `41 > 40` will return `False`.



**설명:** `Not`은 `True`문은 `False`를 반환하고, `False`문은 `True`를 반환한다. `41 > 40`은 `True`이지만, 앞에 `!`연산자가 있으므로, `False`를 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's get some practice with not.

* Set `bool_one` equal to the result of
```python
not True
```
* Set `bool_two` equal to the result of
```python
not 3 ** 4 < 4 ** 3
```
* Set `bool_three` equal to the result of
```python
not 10 % 3 <= 10 % 2
```
* Set `bool_four` equal to the result of
```python
not 3 ** 2 + 4 ** 2 != 5 ** 2
```
* Set `bool_five` equal to the result of
```python
not not False
```


**설명:** ① 각 변수에 양변의 계산값을 대입하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, not True is False and not False is True. So, for example, bool_one should be:
```python
bool_one = False
```

**설명:** `!` 연산자는 양 변의 최종 결과값의 반대를 반환한다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
bool_one = not True

bool_two = not 3**4 < 4**3

bool_three = not 10 % 3 <= 10 % 2

bool_four = not 3**2 + 4**2 != 5**2

bool_five = not not False
```

**설명:** 각 변수의 반환값이 무엇일지 생각해 보자. 
{: .notice--info}



**결과**
``` 
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 9. This and That (or This, But Not That!)

**Boolean** operators aren't just evaluated from **left** to **right**. Just like with **arithmetic operators**, there's an order of operations for boolean operators:

1. `not` is evaluated **first**;
2. `and` is evaluated **next**;
3. `or`  is evaluated **last**.
For example, `True` or not `False` and `False` returns `True`. If this isn't clear, look at the Hint.

Parentheses `()` ensure your expressions are evaluated in the order you want. Anything in parentheses is evaluated as its own unit.


**설명:** `boolean`에서 계산되어지는 순서는 수의 계산과 값다. 그중 `not`이 제일 먼저 계산되고, `and` 그다음, `or`가 마지막에 계산된다. 즉 `not` -> `and` -> `or` 순으로 계산된다. `()`는 이들 보다 먼저 계산된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Assign True or False as appropriate for bool_one through bool_five.

* Set `bool_one` equal to the result of
```python
False or not True and True
```
* Set `bool_two` equal to the result of
```python
False and not True or True
```
* Set `bool_three` equal to the result of
```python
True and not (False or False)
```
* Set `bool_four` equal to the result of
```python
not not True or False and not True
```
* Set `bool_five` equal to the result of
```python
False or not (True and True)
```


**설명:** ① 각 변수에 값을 대입 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
`True or not False and False`. 
1. `not` gets evaluated **first**, 
2. so we have `True or True and False`. 
3. `and` goes next, 
4. so we get `True or False`. 
5. As we've seen, `True or False` is `True`, 
6. so the value finally returned is `True`!


**설명:** `not` -> `and` -> `or` 순으로 계산 되어진다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
bool_one = False or not True and True

bool_two = False and not True or True

bool_three = True and not (False or False)

bool_four = not not True or False and not True

bool_five = False or not (True and True)
```

**설명:** 각 변수에 `not`, `and`, `or` 순으로 계산한다. 
{: .notice--info}



**결과** 
``` 
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 10. Mix 'n' Match

Great work! We're almost done with **boolean** operators.

```python
# Make me false
bool_one = (2 <= 2) and "Alpha" == "Bravo"
```

**설명:** 변수 `bool_one`에는 `False`가 반횐 되어 진다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** This time we'll give the expected result, and you'll use some combination of **boolean** operators to achieve that result.

Remember, the **boolean** operators are `and`, `or`, and `not`. Use each one at least once!


**설명:** ① boolean 연산자 (`not`, `and`, `or`)를 활용하여, 주석에서 지시하는 대로 결과값을 만들어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Make sure to use at least one `and`, `or`, or `not`.

**설명:** boolean 연산자 `and`, `or`, or `not` 사용하여 만들어라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Use boolean expressions as appropriate on the lines below!

# Make me false!
bool_one = (2 <= 2) and "Alpha" == "Bravo"  # We did this one for you!

# Make me true!
bool_two = True and True

# Make me false!
bool_three = False and True

# Make me true!
bool_four = not False

# Make me true!
bool_five = True or True
```

**설명:** 주석에 주어진 지시대로 각 변수에 값을 대입하라. 
{: .notice--info}



**결과** 
``` 
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 11. Conditional Statement Syntax

`if` is a **conditional statement** that executes some specified code after checking if its expression is `True`.

Here's an example of `if` statement syntax:
```python
if 8 < 9:
  print "Eight is less than nine!"
```
In this example, `8 < 9` is the checked expression and print **"Eight is less than nine!"** is the specified code.

Pay **attention** to the **indentation** before the `print` statement. This space, called white space, is how Python knows we are entering a **new block** of code. Python accepts many different kinds of **indentation to indicate blocks**. In this lesson, we use four **spaces** but elsewhere you might encounter **two-space** indentation or tabs (which Python will see as different from spaces).

If the **indentation** from one line to the next is different and there is no command (like if) that indicates an incoming block then Python will raise an `IndentationError`. These errors could mean, for example, that one line had two spaces but the next one had three. Python tries to indicate where this error happened by printing the line of code it couldn't parse and using a `^` to point to where the indentation was different from what it expected.




**설명:** `if`는 **조건문** 이다. 주어진 조건이 `True`이면, 다음 정의 내용을 실행하는 것이다. `if`문을 사용할때, 주의할 것이 있다. `if`의 조건 뒤에 `;`으로 마무리 해주어, `if`문의 조건이 끝났음을 명시해야 하며, 다음 정의 내용은 `if`문의 위치보다 **space** 2칸을 들어간채 정의해야 한다.
Python은 `if`문의 범위를 자신보다 안쪽에 들여쓰기가 되어 있는 정의 문들을 자신의 범위로 여긴다.
들여쓰기가 space 2칸이 아니면, Python은 `IndentationError` 라는 Error를 출력하면, 잘못된 위치를 `^`로 표히해 준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** If you think the `print` statement will print to the console, set `response` equal to **'Y'*; otherwise, set response equal to **'N'**.


**설명:** ① 출력되어지는 문장의 내용이 맞다고 생각되면 변수 `response`에 'Y'를 대입하고, 그렇지 않다면 'N'를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Make sure to set response to "Y" or "N"!


**설명:** 변수 `response`에 "Y" or "N"를 입력한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
response = 'N'

answer = "Left"
if answer == "Left":
    print "This is the Verbal Abuse Room, you heap of parrot droppings!"
    
# Will the above print statement print to the console?
# Set response to 'Y' if you think so, and 'N' if you think not.
```

**설명:** 출력문의 내용이 마음에 들지 않으므로 나는 변수 `response`에  "N" 를 대입한다. 
{: .notice--info}



**결과** 
``` 
This is the Verbal Abuse Room, you heap of parrot droppings!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 12. If You're Having...

Let's get some practice with `if` statements. Remember, the syntax looks like this:

```python
if some_function():
  # block line one
  # block line two
  # et cetera
```  
Looking at the example above, in the event that `some_function()` returns `True,` then the indented block of code after it will be executed. In the event that it returns False, then the indented block will be **skipped**.

Also, make sure you notice the `colons` at the end of the `if` statement. We've added them for you, but they're important.


**설명:** `if`문이 `some_function()`의 결과값이 `True`이면 `if`문 보다 안쪽에 들여쓰진 #block line one, #block line two, # et cetera 의 정의문들이 실행된다. 그렇지 않고 `some_function()`의 결과값이 `False` 이면 정의문들은 실행되지 않는다. 그리고 `if`문의 끝에는 `;`이 항상 와야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** In the editor you'll see two functions. Don't worry about anything unfamiliar. We'll explain soon enough.

* Replace the underline on line 2 with an expression that returns `True`.
* Replace the underline on line 6 with an expression that returns `True`.
If you do it successfully, then both "Success #1" and "Success #2" are printed.


**설명:** ① 2라인과 6라인에 각 `True`가 되도록 계산식으로 대체하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Here's an example to remind you of the syntax:
```python
def true_function():
  if 1 < 2:
    return True
```
Don't forget the colon at the end of the line!


**설명:** `if`문 다음에 계산식을 만든다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def using_control_once():
    if 2 < 3:
        return "Success #1"

def using_control_again():
    if 3 == 3:
        return "Success #2"

print using_control_once()
print using_control_again()
```

**설명:** `if` 문 다음에 `True`값이 되도록 만든다. 그 결과 값이 반환되어 출력된다. 
{: .notice--info}



**결과** 
```
Success #1
Success #2
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 13. Else Problems, I Feel Bad for You, Son...

The `else` statement complements the if statement. An `if/else` pair says: "If this expression is true, run this indented code block; otherwise, run this code after the else statement."

Unlike if, else doesn't depend on an expression. For example:

```python
if 8 > 9:
  print "I don't printed!"
else:
  print "I get printed!"
```

**설명:** `else`문은 `if`문과 함께 쓰는 것으로 `if`문 조건에 해당되지 않으면 `else` 조건문이 실행된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Complete the `else` statements to the right. Note the indentation for each line!


**설명:** ① `else`문을 완성시켜라. 들여쓰기를 주의 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

To complete your else statement lines, the only thing you need to do is add False after the returns on lines 7 and 13.

**설명:** `else`문이 어떻게 사용되는지 해당 부분에 고쳐 보라. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
answer = "'Tis but aa scratch!"

def black_knight():
    if answer == "'Tis but a scratch!":
        return True
    else:
      	print ("else call")
        return False        # Make sure this returns False

black_knight()


def french_soldier():
    if answer == "Go away, or I shall taunt you a second time!":
        return True
    else:             
        return False        # Make sure this returns False
      
```

**설명:** 함수 `black_knight()`에서 `if`문이 `answer`와 비교하여 맞으면 `True`를 돌려주고, 틀리면 `else`문이 동작되어 `print ("else call")이 출력되고, `False`가 반환된다.
{: .notice--info}


**결과** 
``` 
#skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 14. I Got 99 Problems, But a Switch Ain't One

`elif` is short for **"else if."** It means exactly what it sounds like: "otherwise, if the following expression is true, do this!"

```python
if 8 > 9:
  print "I don't get printed!"
elif 8 < 9:
  print "I get printed!"
else:
  print "I also don't get printed!"
```
In the example above, the `elif` statement is only checked if the original if statement is `False`.


**설명:** `elif`는 "else if" 의 줄인 말이다. `if`조건절이 아닐때, 다른 조건절을 사용하고자 할때, `elif`를 사용한다. `else`차이는 `else`는 조건을 걸수 없지만, `elif`는 조건을 걸수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 2, fill in the `if` statement to check if answer is greater than `5`.

On line 4, fill in the `elif` so that the function outputs `-1` if answer is less than `5`.


**설명:** ① 2 라인에서 `if`문을 사용하여 변수 `answer`값이 `5`보다 크면 `1`을 반환하고, 4 라인에서 `elif`문을 사용하여 `5`보다 작으면 `-1`을 반환하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Make sure the if and elif statements end with colons :

Your code should look something like:

```python
if EXPRESSION:
  # do something
elif OTHER EXPRESSION:
  # do something
else:
  # do something
```

**설명:** `if`, `elif`, `else` 끝에 `:`를 잘 살펴봐라. 
{: .notice--info}

**결과** 
``` 
```

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
def greater_less_equal_5(answer):
    if answer > 5:
        return 1
    elif answer < 5:          
        return -1
    else:
        return 0
        
print greater_less_equal_5(4)
print greater_less_equal_5(5)
print greater_less_equal_5(6)

```

**설명:** 변수 `answer`이 5보다 큰지, 작은지, 같은지를 보여준다. 
{: .notice--info}


**결과** 
``` 
-1
0
1
```



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 15. The Big If

Really great work! Here's what you've learned in this unit:

**Comparators**
```python
3 < 4
5 >= 5
10 == 10
12 != 13
```

**Boolean operators**
```python
True or False 
(3 < 4) and (5 >= 5)
this() and not that()
```

**Conditional statements**
```python
if this_might_be_true():
  print "This really is true."
elif that_might_be_true():
  print "That is true."
else:
  print "None of the above."
Let's get to the grand finale.
```



**설명:** 우리는 비교교문, Boolean 연산자, 조건문(`if`, `elif`, `else`)를 배웠다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** In the workspace to your right, there is the outline of a function called `grade_converter()`.

The purpose of this function is to take a number grade **(1-100)**, defined by the variable `grade`, and to return the appropriate letter **grade (A, B, C, D, or F)**.

Your task is to complete the function by creating appropriate `if` and `elif` statements that will compare the input `grade` with a number and then return a letter `grade`.

Your function should return the following letter grades:

* 90 or higher should get an "A"
* 80 - 89 should get a "B"
* 70 - 79 should get a "C"
* 65 - 69 should get a "D"
* Anything below a 65 should receive an "F"


**설명:** ①`grade_converter()` 함수를 다음 조건에 따라 동작 되게끔 지금가지 배운 **비교문**, **조건문** 등을 사용하여 작성하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Be careful with your indentation—grade_converter() is a function (which we'll get to in the next unit), and as you can see from the comment, function blocks are indented the same way if, elif, and else blocks are.

If you are having trouble creating the if and elif statements, here's the first one you can use as an example:
```python
if grade >= 90:
     return "A"
```     
This will compare the variable grade with the value 90 and if it is greater than or equal to 90 it will return the letter A.

**설명:** `if` grade`>=` 90: 은 변수 `grade` 값이 `90`보다 크거나 같다는 표현이다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    
```python
# Complete the if and elif statements!
def grade_converter(grade):
    if grade >= 90:
        return "A"
    elif grade >= 80:
        return "B"
    elif grade >= 70:
        return "C"
    elif grade >= 65:
        return "D"
    else:
        return "F"
      
# This should print an "A"      
print grade_converter(92)

# This should print a "C"
print grade_converter(70)

# This should print an "F"
print grade_converter(61)
```

**설명:** 각 `if`, `elif`, `else`를 사용한다. 
{: .notice--info}


**결과** 
``` 
A
C
F
```

<br>
<br>    
<br>    