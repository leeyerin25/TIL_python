# TIL


---
---
**3/15**

TYPE, μ κ³± μ μ© 



```python
height = input("enter your height in m: ")
weight = input("enter your weight in kg: ")
```

#Write your code below this line π

```python
height_second=(float(height))
weight_second=(int(weight))
result=(weight_second/height_second**2)   
print(float(result))
print(int(result))
```

***2 λ 2μμ κ³±*

#it's teacher's code π
```python
bmi = weight_as_int / heiight_as_float **2
bmi_as_int = int(bmi)
print(bmi_as_int)
```
.

CONSOLE<br>
enter your height in m: 1.75 <br>
enter your weight in kg: 80<br>
26.122448979591837<br>
26

<br>

<br>
<br>
<br>
<br>


---
---

**3/16**

f-string ν¨μ μ μ©

```
age = input("What is your current age?")
```
#Write your code below this line π
```python
days=(365*90-int(age)*365)
weeks=(52*90-int(age)*52)
months=(12*90-int(age)*12)
print(f" You have {days} days, {weeks} weeks, and {months} months left.")
```

CONSOLE<br>
What is your current age?56
 You have 12410 days, 1768 weeks, and 408 months left.





fν¨μ+μ¬μΉμ°μ°ν¨μ+μμμ ν¨μ



 ```python
 #If the bill was $150.00, split between 5 people, with 12% tip. 

#Each person should pay (150.00 / 5) * 1.12 = 33.6
#Format the result to 2 decimal places = 33.60

#Tip: There are 2 ways to round a number. You might have to do some Googling to solve this.πͺ

#Write your code below this line π

print("Welcome to the tip calculator!")
bill=float(input("What was the total bill? $"))
tip=int(input("How much tip would you like to give? 10, 12, or 15? "))
people=int(input("How many people to split the bill?"))

tip_2=(tip/100*bill+bill) #ννΌμΌνΈ*μ΄κΈμ‘ = νκΈμ‘+μ΄κΈμ‘
pay=int(tip_2)/people
pay_final="{:.2f}".format(pay)  #f-string λ μμ£Όμ¬μ©
print(pay_final)
```

*.2f*



* CONSOLE

Welcome to the tip calculator!

What was the total bill? $150

How much tip would you like to give? 10, 12, or 15? 12

How many people to split the bill?5
33.600000
<br>
<br><br>
<br>
<br>

---
---




**3/17**

IF ELSE ν¨μ

 ```python
number = int(input("Which number do you want to check? "))

#Write your code below this line π
if number%2==0:
 print("This is an even number.")
else:
  print("This is an odd number.")
```

*if μ : κΉλ¨Ήμ§ μκΈ°* <br>
*%λ λλκ³  λ λλ¨Έμ§κ° λμΆ*
<br>
COLSOLE<br>
Which number do you want to check? 94<br>
This is an even number.
<br>
<br>

---
if,else,round μ μ©
```python
# π¨ Don't change the code below π
height = float(input("enter your height in m: "))
weight = float(input("enter your weight in kg: "))

#Write your code below this line π
bmi=round(weight/height**2)
.
if bmi<18.5:  
 print(f"Your BMI is {bmi}, you are underweight.") 
elif bmi<25:   # belowλ§ μκ°νκΈ°
 print(f"Your BMI is {bmi}, you are normal weight") 
elif bmi<30:
 print(f"Your BMI is {bmi}, you are slightly overweight") 
elif bmi<35:
 print(f"Your BMI is {bmi}, you are obese") 
else:    #λλ¨Έμ§λ else
 print(f"Your BMI is {bmi}, you are clinically obese")
 ```

 COLSOLE<br>
 Your BMI is 28, you are slightly overweight.
<br>
<br>

---
**if , else κ΅¬νκΈ° λ³΄μ€λ¬Έμ <br>**
**leap year : μ€λ : 4λλ§λ€ λλλλ ν΄λ₯Ό νμνλΌ**<br><br>
1.νλ¦ flow λ§λ€κΈ° (μ΄λ»κ² κ³μ°ν κ²μΈμ§)
<br>2.μκ°ννκΈ°<br><br>


*νλ¦°λ²μ 1*
 ```python
 year = int(input("Which year do you want to check? "))
# π¨ Don't change the code above π

#Write your code below this line π
#t=round(year/4,1)
if year%4==0:
  if year%100\=0:     #????
    if year%400==0:
     print("Leap year.")
else:
  print("Not leap year." )  #????

```

```PYTHON
# π¨ Don't change the code below π
year = int(input("Which year do you want to check? "))

#Write your code below this line π

if year%4==0: #4λ‘ λλ λλ¨Έμ§κ° 0μΌμ μ€λ μλ
 if year%100==0:  #μ¬κΈ°μ 100μΌλ‘ λλκ°μ λλ¨Έμ§κ° 0μΌμ μ€λμ
   if year%400==0: #κ·Όλ° μ¬κΈ°κΉμ§ 
    print("Leap year.") 
   else:
    print("Not Leap year." ) # %400 ->0 
 else:
  print("Leap year." ) # %100->0 
else:
 print("Not leap year." ) # %4 

#4λ‘λλ΄μλ 0 -> μ€λμλ
#4λ‘λλ³μλ 0, 100μΌλ‘λλ³μλ0 -> μ€λ
#4λ‘λλ³μλ 0, 100μΌλ‘λλ³μλ0, 400μΌλ‘ λλ΄μλκ° 0 -> μ€λ

 ```
<br>
<br>
<br>

---
---

 3/19<BR>
IFν¨μ
 ```PYTHON
 # π¨ Don't change the code below π
print("Welcome to Python Pizza Deliveries!")
size = input("What size pizza do you want? S, M, or L ")
add_pepperoni = input("Do you want pepperoni? Y or N ")
extra_cheese = input("Do you want extra cheese? Y or N ")


#Write your code below this line π

if size=='L':
 bill = 25
 if add_pepperoni=='Y':
  bill = bill+3
 if size=='M':
  bill = 20
  if add_pepperoni=='Y':
   bill = bill+3
  if size=='S':
   bill = 15
   if add_pepperoni=='Y':
    bill = bill+1

if extra_cheese=='Y':
 bill = bill+1
 ```

 CONSOLE
<BR> 28

 ```python
 # π¨ Don't change the code below π
print("Welcome to the Love Calculator!")
name1 = input("What is your name? \n")
name2 = input("What is their name? \n")

#Write your code below this line π

name1 = name1.lower() #.lower()
name2 = name2.lower()
name3 = f'{name1}{name2}' #fμ€νΈλ§μ κ°λ‘ νμμμ

a=name3.count('t')+name3.count('r')+name3.count('u')+name3.count('e')
b=name3.count('l')+name3.count('o')+name3.count('v')+name3.count('e')

ab=int(f'{a}{b}')

if ab<10 or ab>90:
 print(f'Your score is {ab}, you go together like coke and mentos.')
elif 40<ab<50:
 print(f'Your score is {ab}, you are alright together.')
else:
 print(f'Your score is {ab}.')	   
```

CONSOLE<BR>
Welcome to the Love Calculator!
What is your name? 
Kanye West
What is their name? 
Kim Kardashian
Your score is 42, you are alright together.
<br>
<br>
<br>

---
---
3/20<br>
νλ¦°λ²μ 1
```python
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 

#Write your code below this line π
leftright=input("Youre at a crossroad. Where do you want to go? Type 'left' or 'right'")
waitswim=input("Youve come to a lake. There is an island in the middle of the lake. Type wait to wait for a boat. Type swim to swim across.")
dore=input("You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose?")

print(leftright)
if leftright=='left':
	print(waitswim)
	if waitswim=='wait':  #μ¬κΈ°μ λ£λκ² μλλΌ μ¬κΈ°μ λ°λ‘ inputμν΄μ μ§λ¬Έμ μ΄μ΄κ°μΌν¨. κ·Έλ¦¬κ³  κ·Έ inputμ μ λͺ©μ λΆνμ€μ λμ€μ μ΄μ©ν  μ μκ² ν΄μΌν¨
		print("You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose?")
	else:
		print("You fell into a hole. Game Over.")
elif leftright=='right':
	print("fall in a hole. game over.")
  ```

  μ λ΅
  ```python
  print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 

#Write your code below this line π
leftright=input('Youre at a crossroad. Where do you want to go? Type "left" or "right".') #1λ²μ§Έ μ§λ¬Έμ INPUT μ¬μ©ν΄μ μμ±

if leftright=="left": 
	waitswim=input('You\'ve come to a lake. There is an island in the middle of the lake. Type "wait" to wait for a boat. Type "swim" to swim across.')
	if waitswim=="wait":
		door=input("You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose?")
		if door=='yellow':
			print("You found the treasure! You Win!")
		else:
			print("You chose a door that doesn't exist. Game Over.")	
	else:
		print("You fell into a hole. Game Over.")
elif leftright=='right':
	print("fall in a hole. game over.")
  ```

CONSOLE<br>
Welcome to Treasure Island.<br>
Your mission is to find the treasure.<br>
Youre at a crossroad. Where do you want to go? Type "left" or "right".left<br>
You've come to a lake. There is an island in the middle of the lake. Type "wait" to wait for a boat. Type "swim" to swim across.wait<br>
You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose?red<br>
You chose a door that doesn't exist. Game Over.

---

RANDOMν¨μ<br>
ν¨μλ3μ’λ₯ λ΄μ₯ν / λͺ¨λ / λ€μ΄λ°μμΌλλκ±°
```PYTHON 
import random # import  + random.radnint
ramdom2=random.randint(1,6) #1~6μ¬μ΄ μ«μ λ¬΄μμμΆμΆ

print(ramdom2)

random3=random.random() #0~1μ¬μ΄ λ¬΄μμ μΆμΆ
print(random3)
```
CONSOLE
<BR> 3<BR>0.25445<br><br>

---

λλ€μΌλ‘ μ«μ λ½κ³  1μ΄λ©΄ headλ₯Ό νμ, 0μ΄λ©΄ tailsλ₯Ό νμνλΌ

```python
import random
random2 =random.randint(0,1)

if random2==1:
	print("Head")
else:
	print("Tails")
```

---
random,splitν¨μ<BR>
νλ¦°λ²μ 
```python
import random #import random μ λ³΄ν΅ λ§¨μμ€μ
# Split string method
names_string = input("Give me everybody's names, separated by a comma. ")
names = names_string.split(", ")  
# π¨ Don't change the code above π

#Write your code below this line π
len=len(names)
random1 = random.randint(0,len-1) #λ½μ λ²μμλ₯Ό μ ν¨

print(f'{random1} is going to buy the meal today!')
```
<br>
μ λ΅λ²μ <br>

```python
import random #import random μ΄λΌλ λͺ¨λμ μ¨μΌ κ·Έμ λΈλ €μ€λ choice,sample λ±μ ν¨μλ₯Ό λΆλ¬μ¬μμλ€. 
# Split string method
names_string = input("Give me everybody's names, separated by a comma. ")
names = names_string.split(", ") #kim, lee[, ]park
# π¨ Don't change the code above π

#Write your code below this line π
len=len(names)
random1 = random.randint(0,len-1) # λ€μ΄μ€λ μ΄λ¦μμ μλ¬΄κ±°λ λ½μμ£Όλκ²λ¨
person=names[random1]  #λ¦¬μ€νΈμμ μ«μλ‘ μΆμΆνλκ±°
print(f'{person} is going to buy the meal today!')
```
<br><br>
---
---
3/21<br>listν¨μ
```python
# π¨ Don't change the code below π
row1 = ["β¬οΈ","β¬οΈ","β¬οΈ"]
row2 = ["β¬οΈ","β¬οΈ","β¬οΈ"]
row3 = ["β¬οΈ","β¬οΈ","β¬"]
map = [row1, row2, row3]
print(f"{row1}\n{row2}\n{row3}")
position = input("Where do you want to put the treasure? ")
# π¨ Don't change the code above π

#Write your code below this row π

hori=int(position[0]) #2
verti=int(position[1]) #3

selected_row=map[verti-1] #λ§΅μμ row1,row2,row3μ΄λ λͺλ²μ§Έ μ€μΈκ°λ₯Ό κ³¨λΌμ€ + μ€μ μ νλκ² μ°μ μμ
selected_row[hori-1] = "x" #κ·Έμ€μμ λͺλ²μ§Έ λ°μ€μΈκ°λ₯Ό κ³¨λΌμ€

#Write your code above this row π

# π¨ Don't change the code below π
print(f"{row1}\n{row2}\n{row3}")
```
CONSOLE
```PYTHON
['β¬οΈ', 'β¬οΈ', 'β¬οΈ']
['β¬οΈ', 'β¬οΈ', 'β¬οΈ']
['β¬οΈ', 'β¬οΈ', 'β¬']
Where do you want to put the treasure? 23
['β¬οΈ', 'β¬οΈ', 'β¬οΈ']
['β¬οΈ', 'β¬οΈ', 'β¬οΈ']
['β¬οΈ', 'x', 'β¬']  #23μ λ£μμλ 
#3μ νμ λ¨Όμ  μ°Ύκ³ , 2λΌλμ΄μ μμΉλ₯Ό μ°Ύλλ€.
```
---
list,if,random,input ν¨μ "κ°μλ°μλ³΄κ²μ"<BR>
1μ°¨λ²μ 
```python
list=[rock,paper,scissors]
choice=int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.\n"))
if choice==0: #0μ λ½κΈ°μν΄μ  μΈνμ intλ‘ μ μ©μμΌμΌν¨
	print(rock)
	if choice==1:
		print(paper)
		if choice==2:
			print(scissors) #λ κΈΈμ΄

radom= random.randint(0,2)
print("Computer choose" + list[radom])
```
μ λ΅
```python
list=[rock,paper,scissors]
choice=int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.\n"))
print(list[choice]) #if 3μ€μ νμ€λ‘ μ€μ΄λ λ°©λ²

radom= random.randint(0,2)
print("Computer choose" + list[radom])

if choice==0 and radom==0:
	print("it's draw")
if choice==0 and radom==2:
	print("you win") .....
  ```
  CONSOLE
  ```
  What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.
0

    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)

Computer choose #RANDOM
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)

it's draw
```
---
for in λ°λ³΅λ¬Έ (INμ μν κ° μλ§νΌ λ°λ³΅μ΄ λμμΌ λλ¨)
```python
student_heights = input("Input a list of student heights ").split()
for n in range(0, len(student_heights)):
  student_heights[n] = int(student_heights[n]) 
# π¨ Don't change the code above π

height_total = 0
for height in student_heights: 
 height_total = height_total + height #+heightλ₯Ό ν΅ν΄μ ex)140+160+180 μ΄λ κ² λ°λ³΅λμ΄ λν΄μ§
print(height_total)

number=0
for student in student_heights:
 number = number + 1 # +1μ ν΅ν΄μ 140+160+180μ μ«μλ§νΌ 1μ©λ§ λν΄μ§λ€. (inputκ°κ³Ό μκ΄μμ΄)

 print(round(height_total/number))

```
CONSOLE<BR>
Input a list of student heights<BR> 100 200 300 100<BR>
700<BR>
4<BR>S
175

---
```python
# π¨ Don't change the code below π
student_scores = input("Input a list of student scores ").split()  #λ¦¬μ€νΈλ‘λ§λ¬ ["37","90","100"]
for n in range(0, len(student_scores)):
  student_scores[n] = int(student_scores[n]) #μ«μλ‘λ°κΎΈλμμ
print(student_scores) # [37, 90, 100]

#Write your code below this row π
scoretotal =0
for score in student_scores:
	if score > scoretotal: # >λ₯Ό ν΅ν΄ κ°μ μ­ λΉκ΅νκ³ 
		scoretotal = score # =λ₯Ό ν΅ν΄ score > scoretotal μ΄ μ±λ¦½ν μ κ°μ λ°κΏμ€λ€
print(f"the score is :{scoretotal} .") #κΆκΈνμ  PRINTλ₯Ό μμλΆνλκ²κ³Ό λμ΄μ°κΈ°ν΄μ λμ¨κ°μ΄ λ€λ₯΄λλ° μκ·Έλ°κ²μΈκ°?? forλ¬Έ νλ¦°νΈκ° λμ λ°λ³΅μ΄ λκ²μ.
```
CONSOLE<BR>
Input a list of student scores 140 150 187 100 195<BR>
[140, 150, 187, 100, 195]<BR>
the score is :195 .<BR>
<BR><BR><BR>

---
for in range μ¬μ©ν΄μ κ° μ μ²΄λνκΈ° (μ§μλ§)
```
total = 0
for number in range(2,101,2): #2μ© μ»€μ§κ²
	total = total+number
print(total)
```
``` 
total = 0
for number in range(2,101,2): 
	if number %2 == 0:  #λλ¨Έμ§=0 μΈ κ°μ μ°ΎκΈ°=μ§μ
  total += number
print(total)
```
CONSOLE<BR>
2550
<BR><BR>

---
FOR IN RANGE + IF ν¨μ <BR>
μ€λ΅
```
#Write your code below this row π
for number in range(1,101):
	if number %3==0 :
		print("Fizz")
	elif number % 5 == 0:
		print("buzz")
	elif number %3==0 and number %5==0 :
		print("fizzbuzz")
print(number)		#λ€μ΄μ°κΈ° νλ¦Ό
```
```python
for number in range(1,101):
	if (number %3==0) and number %5==0 : #μ‘°κ±΄μ΄ λ§μκ±Έ λ¨Όμ μ°λκ±΄κ°? λ§μκ±Έ λ¨Όμ  μ¨μ€μΌ λ°μμ μκ±Έλ¦Ό μμλ‘ %5==0: λ₯Ό λ¨Όμ μ°λ©΄ 15 κ° νλ°ν΄ λλ 5μμ κ±Έλ¦¬κ³  %3κ³Ό %5 μμ κ±Έλ¦¬μ§ λͺ»ν¨.
		print("fizzbuzz")
	elif number % 5 == 0:
		print("buzz")
	elif number %3==0 :
		print("fizz")
	else:
		print(number) #μ μ©ν κ² μμλ κ·Έλλ‘ μ¨μ£ΌκΈ°


CONSOLE<BR>
1
2
fizz
4
buzz
fizz
7
8
fizz
buzz
11
fizz
13
14
fizzbuzz
16
17 ....
```

```python
#Password Generator Project
import random
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

print("Welcome to the PyPassword Generator!")
nr_letters= int(input("How many letters would you like in your password?\n")) 
nr_symbols = int(input(f"How many symbols would you like?\n"))
nr_numbers = int(input(f"How many numbers would you like?\n"))
```
μ€λ΅ easy case
```
#Eazy Level - Order not randomised:
#e.g. 4 letter, 2 symbol, 2 number = JduE&!91
password = ""

random2 = random.randint(0,2)   #λλ€λ§ μ¨μ  λͺ»νλ??
print(letters[random2] + "is gppd.")
```
μ λ΅ easy case
```py
password = "" #λ¬Έμ₯λ§λ€κΈ°μν΄ κ³΅λμΌλ‘

for char in range (0,nr_letters):  #nr_letters INPUT λ£μνμλ§νΌ λκ²λ¨ -> μνλ μλ¦Ώμκ° μλ€λ©΄ for in rangeλ‘ λμ¬ μλ¦Ώμλ₯Ό μ ν΄μ€μΌν¨ 
#κΆκΈνκ±΄ char μ κ·Έλ₯μ΄λ¦, μ¬κΈ°μ  λ³μκ° μμ°μ΄κ³  λ°λ³΅λ§μ°μ
	password = password + random.choice(letters)
	
for char in range (0,nr_symbols): 
	password = password + random.choice(symbols)
	
for char in range (0,nr_numbers): 
	password = password + random.choice(numbers)

 print(password)

 ---
CONSOLE
Welcome to the PyPassword Generator!
How many letters would you like in your password?
3
How many symbols would you like?
3
How many numbers would you like?
3
dAw%!!592
```
μ€λ΅ hard case
```py
password_list = []

for char in range(0,nr_letters): 
	password_list.append(random.choice(letters))
	
for char in range(0,nr_symbols): 
	password_list = password_list + random.choice(symbols)
	# list + str => μλ¬κ° λ¨ κ·Έλ₯ λ€ appendλ‘ μ¨μ€μΌ λ¦¬μ€νΈλ‘ λ£μ΄μ§
for char in range(0,nr_numbers): 
	password_list = password_list + random.choice(numbers)

print(password_list)
random.shuffle(password_list)
print(password_list)

```
```
for _ char in enumerate(xxx)
1 a
2 b
3 c
4 d
```


3/22<br>
ν¨μκ°μ΄λ = pep8<br>

```
1.λ¦¬νν°λ§(ν¨μλ₯Ό κ°λ¨ν λ€μ λ§λλκ±°)
ν¨μ κΈ°μ‘΄μκ±Έ μ΄μ©ν΄μ μλ‘λ§λ€κΈ°
def ν¨μμ΄λ¦():
	ν©μΉ ν¨μ()
	ν©μΉ ν¨μ()

ν¨μμ΄λ¦ #μνλ¨

2. νλΌλ―Έν°	
def ν¨μμ΄λ¦(λ³μμ΄λ¦):
	print("μ°κ³ μΆμλ§ {λ³μμ΄λ¦}" ) #λ³΄μ¬μ£Όλμ©λλΌμ μ΄μ©μλ¨
	return #μ€μ λ΄λ³΄λ΄λμ©λ

print(ν¨μμ΄λ¦)

ν¨μμ΄λ¦{λ£κ³ μΆμκ±°}

μΆλ ₯: μ°κ³ μΆμλ§ + λ£κ³ μΆμκ±°
```
<br><br>

---

https://reeborg.ca/reeborg.html<br>
νλ€κ²μ λμ΄λ1 νμ΄
```py
def turn_right(): #def λ€μμ€μ λ¬΄μ‘°κ±΄ λμ΄μ°κΈ°
    turn_left()
    turn_left()
    turn_left()

 #μνμμλ λμ λΆνμ ν¨μμ΄λ¦μ¨μ νΈμΆ

def one():
    move()
    turn_left()
    move()
    turn_right() #ν¨μμμ ν¨μ
    move()
    turn_right()
    move()
    turn_left()

def μμ():
    a = 3
    if a > 2:
      print("aκ°2λ³΄λ€ ν΄κ²½μ° νλ¦°νΈν΄μΌν¨") #νλ¦°νΈλ ν¨μμ κΈ°λ₯μ΄κΈ°λλ¬Έμ μ if μ€λ³΄λ€ λ μμͺ½μΌλ‘ μμ±νλ€.
console
def()
:aκ°2λ³΄λ€ ν΄κ²½μ° νλ¦°νΈν΄μΌν¨





i = 0    
while i < 6: # 5κΉμ§ 5λ² λ°λ³΅
    one()
    i += 1  # μ one μ΄λΌλ ν¨μλ₯Ό 5λ² λ°λ³΅μν΄

while True: # λ¬΄νλ°λ³΅

```
<br>
νλ€κ²μ λμ΄λ3 νμ΄

```python
def turn_right():
    turn_left()
    turn_left()
    turn_left()
    
while not at_goal():

    #μΌλ¨ κ° (μμ΄ λ«λ €μμΌλ©΄) λ§νμμΌλ©΄ κ°μ§λ§κ³ ..
    if front_is_clear():
        move()


    # λ²½μ λ§λ¬λλ° μ€λ₯Έμͺ½μ΄ λ§νμμκ²½μ° turn_left
    if (not front_is_clear()) and wall_on_right():
        turn_left() #ifλ₯Ό κ°μ μ΄ μμΉμ λλ²μΈκ²½μ° : λ ifμ λΆ μ€νμν΄


    # μμ΄ λ«λ €μκ³ , μ€λ₯Έμͺ½μ΄ λ§νμμ.
    elif front_is_clear() and (not wall_on_right()):
        turn_right() #if μ΄ μμΉμ elif λ₯Ό μΈκ²½μ° : μμ if κ° ν΄λΉνμ§ μμλ elif λ‘ λ΄λ €μ΄ => μ‘°κ±΄μ μ€μλλ₯Ό λΆμ¬ν΄μ μ°¨λ‘λ‘ μ°λκ² μ€μν¨

    # μμ΄ λ§νμκ³ , μ€λ₯Έμͺ½μ ~~~
    elif (not front_is_clear()) and (not wall_on_right()):
        turn_right()
	```

  <br>
νλ€κ²μ λμ΄λ4 νμ΄

```python
def turn_right():
    turn_left()
    turn_left()
    turn_left()

def jump():
    turn left()       #μΌμͺ½μΌλ‘λμμ
    while wall_on_right(): #μ€λ₯Έμͺ½μ λ²½μ΄ μλλμμλ
        move()        #κ³μκ°λΌ 
    turn_right()   #μ€λ₯Έμͺ½μ λ΄λΌ (λ²½μ΄μλμκ°μ΄ μμΌ μ΄ νμ ν¨μκ° μ€νλ¨ λ§λμ©??)
    move()          #νμΉΈμ 
    turn_right()    #λ€μ μ€λ₯Έμͺ½
    while front_is_clear(): #μμ΄ λΉμ΄μλλμμλ
          move()            #μ§μ§
    turn left()    #μΌμͺ½μ λ΄λΌ(μμ΄ λ§νμμΌλ©΄ μ΄ν¨μκ° μ€νλ¨ . ?)
    
    #λ€μ μλ‘ λ°λ³΅νλ©΄ μ΄λ ν νλ€λ λ€ λ°μ΄λμμμλ ν¨μκ° λ¨
    
while not at_goal(): 
    if wall_in_front():
        jump()
    else:
        move()

**λμ€μ day6 μμ€μΌμ΄νλ λ©μ΄μ¦ νμ νκΈ°!!
```



<br><br> HANGMAN GAME<br>
3/23-day7<Br>κ΅¬μνμν€κΈ°

step1 

```py
word_list = ["aardvark", "baboon", "camel"]

#TODO-1 - Randomly choose a word from the word_list and assign it to a variable called chosen_word.

import random
choose = random.choice(word_list)


#TODO-2 - Ask the user to guess a letter and assign their answer to a variable called guess. Make guess lowercase.

guess = input("gets a letter: ").lower()

#TODO-3 - Check if the letter the user guessed (guess) is one of the letters in the chosen_word.

for a in choose : #chooseλ‘ λλ€μ νλ λ¨μ΄λ€μ΄ μͺΌκ°μ Έμ aλ‘ λ€μ΄κ°λκ² μ κΈ°ν¨ -> str μ΄ λ€μ΄κ°λ©΄ νλνλ λ€μ΄κ°μ§λκ²μΈκ°μ©??
	if a == guess :
		print("right")
	else:
		print("worng")
		
```
step 2
```py

import random
word_list = ["aardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#TODO-1: - Create an empty List called display.
#For each letter in the chosen_word, add a "_" to 'display'.
#So if the chosen_word was "apple", display should be ["_", "_", "_", "_", "_"] with 5 "_" representing each letter to guess.

display = []  
length = len(chosen_word)
for _ in range(length):
	display += "_" #display λΌλ λ¦¬μ€νΈ [] μμ "_"λ₯Ό μΆκ°ν΄μ£Όλ λ¨κ³ ????
print(display)

#list comprehension λ¦¬μ€νΈμ νλμ© μΆκ°

guess = input("Guess a letter: ").lower()


#TODO-2: - Loop through each position in the chosen_word;
#If the letter at that position matches 'guess' then reveal that letter in the display at that position.
#e.g. If the user guessed "p" and the chosen word was "apple", then display should be ["_", "p", "p", "_", "_"].

for position in range(length): 
	letter = chosen_word[position] #chose_word λ¨μ΄μ μ²«λ²μ§Έ μνλ²³μ΄ letter μ΄ λλ€
	if letter == guess: #letterμνλ²³κ³Ό guessμλ£μ μνλ²³νλκ° κ°λ€λ©΄! μκΉ κ·Έ display "-""-" μ΄ μλ¦¬λ₯Ό letter μνλ²³μΌλ‘ λ°κΏμΉκ³  μλλ©΄ λ§μλΌ
		display[position] = letter

#TODO-3: - Print 'display' and you should see the guessed letter in the correct position and every other letter replace with "_".
#Hint - Don't worry about getting the user to guess the next letter. We'll tackle that in step 3.

print(display)

```
step3
```py
#Step 3

import random
word_list = ["aardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)
word_length = len(chosen_word)

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#Create blanks
display = []
for _ in range(word_length):
    display += "_"

#TODO-1: - Use a while loop to let the user guess again. The loop should only stop once the user has guessed all the letters in the chosen_word and 'display' has no more blanks ("_"). Then you can tell the user they've won.
end_of_game = False

while not end_of_game:
    guess = input("Guess a letter: ").lower()

    #Check guessed letter
    for position in range(word_length):
        letter = chosen_word[position]
        #print(f"Current position: {position}\n Current letter: {letter}\n Guessed letter: {guess}")
        if letter == guess:
            display[position] = letter

    print(display)

    #Check if there are no more "_" left in 'display'. Then all letters have been guessed.
    if "_" not in display:
        end_of_game = True
        print("You win.")
```

step4
``` py
#Step 4

import random

stages = ['''
  +---+
  |   |
  O   |
 /|\  |
 / \  |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
 /    |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|   |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
  |   |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
      |
      |
      |
=========
''', '''
  +---+
  |   |
      |
      |
      |
      |
=========
''']

end_of_game = False
word_list = ["ardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)
word_length = len(chosen_word)

#TODO-1: - Create a variable called 'lives' to keep track of the number of lives left. 
#Set 'lives' to equal 6.
lives = 6

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#Create blanks
display = []
for _ in range(word_length):
    display += "_"

while not end_of_game:
    guess = input("Guess a letter: ").lower()

    #Check guessed letter
    for position in range(word_length):
        letter = chosen_word[position]
       # print(f"Current position: {position}\n Current letter: {letter}\n Guessed letter: {guess}")
        if letter == guess:
            display[position] = letter

    #TODO-2: - If guess is not a letter in the chosen_word,
    #Then reduce 'lives' by 1. 
    #If lives goes down to 0 then the game should stop and it should print "You lose."
    if guess not in chosen_word: #λκ° inputν μνλ²³μΈ guessκ° chosen wordμ ν¬ν¨λμ§ μμΌλ©΄  μλͺμ΄ νλ κΉμ. κ·Όλ° ν¬ν¨λλ©΄ λ°μ joinμ΄ νλ¦°νΈλ¨
        lives -= 1 
        if lives == 0:
            end_of_game = True
            print("You lose.")

    #Join all the elements in the list and turn it into a String.
    print(f"{' '.join(display)}") #joinμ λ¦¬μ€νΈμμ νλ¨μ΄μ©μ ''λΆλΆμ΄ λ±λΆμ΄μ λμ΄ 
    #fμ€νΈλ§{} μμ display λ₯Ό μ‘°μΈν΄μ£ΌκΈ°μν΄μ ()κ°λ‘λ₯Ό μ

my_set = {"kim","park"} μ(μ§ν©)μ μμκ°μμ
print(" ".join(my_set)) -> λ¬΄μμλ‘ μ‘°μΈλ¨, μ‘°μΈμ κ²°κ³Όλ¬Ό : kim park

    #Check if user has got all letters.
    if "_" not in display:
        end_of_game = True
        print("You win.")

    #TODO-3: - print the ASCII art from 'stages' that corresponds to the current number of 'lives' the user has remaining.
    print(stages[lives])
```

while κ²μμ΄ λλ λκΉμ§:<br>
 if<br>if<br>
 (κ²μμ΄ λλ λλ₯Ό μ μν΄μ€μΌν¨)<br>
 κ²μ μ‘°κ±΄ μμλ₯Ό κ΅¬μνμν€λκ² μ€μνλ€

*λ°λ³΅λ¬Έ λͺλ Ήμ΄*<br>
 continue : ν΄λΉ λΆλΆ λ€μ loopμ κ³μ μ§ν<br>
 pass : κ·Έλ₯ μ­ μ§ν <br>
 break : λ©μΆ°μ€ <br>

 ---
 <br><br><br>
 3/26<br>
 1.def μ¬μ©λ²<br>
 ```py
def add(a, b):
    return a + b  # add λΌλ ν¨μλ₯Ό λ μ΄μ©ν΄μ μ°κ³ μΆμΌλ©΄ returnκ°μΌλ‘ μ μν΄μ£ΌκΈ°.

num1 = 1
num2 = 2

c = add(num1, num2)
c+1
 ```
2.def μμ©λ² (def μμ for, if, enumerate, index)
```py
#defλ λ΄κ° μνλ μ‘°κ±΄μ λ£μ΄ λ§λλ ν¨μ, μ¬κΈ°μλ 3κ°μ νλΌλ―Έν°λ₯Ό λ§λ€κ³ , ν΄λΉλλ κ°κ° μ‘°κ±΄μ λ§λ€μ΄, λλ§μ ν¨μλ₯Ό λ§λ€μλ€. : λͺ©μ : μνλ²³ μμ μνλλ§νΌ λ°κΈ°

n_list=["a","b","c","d","e","f"]

# cbd -> edf
# 2

def number(text, n, what): #textλ λ³ννλ €λ μνλ²³μ΄κ³ , nμ μμ§μ΄κ³ μΆμ μ«μμ΄λ©°, whatμ μμΌλ‘κ°μ§ λ€λ‘κ°μ§ μ νλκ²μΌλ‘ νκ³ μΆλ€. μ΄μ  ν¨μλ₯Ό λ§λ€μ΄λ³΄μ~


step1
    index_list = [] #λ¨Όμ  λ¦¬μ€νΈλ₯Ό μμ±νμ
    for alphabet in text: #μ¬λμΌλ‘λΆν° λ°μ textλ₯Ό alphabetμ λ£κ³ . 
        index_list.append(n_list.index(alphabet))
    #λ°λ³΅λ¬Έμ μ΄μ©ν΄ κ·Έ alphabetμ΄ n_listμ μλ λͺ¨λ μμλ₯Ό λ½μ (μ«μλ -> indexμ΄μ©ν΄μ μΆμΆ)
    #ex) cλ©΄ n_list μμ 2λ²μ§Έ, bλ©΄ 1λ²μ§Έ μ΄λ κ² λ½κ³  appendλ₯Ό μ΄μ©ν΄ index_listμ λ€λ‘ λΆνκ³ ,  forλ¬Έμ΄ λ°λ³΅λλ©΄μ νλμ© μ±μμ§λ€ 
    print(index_list) #νλ¦°νΈλ κ²°κ³Όλ [2,1,3]

    #μ΄λ κ² 1λ²μ§Έ νΌλΌλ―Έν°μΈ text μ λν΄ μ‘°κ±΄μ κ±Έμλ€. textμ λ£λ μνλ²³μ μ«μλ‘ λ³νμν€κΈ°.
step2
    for index, i in enumerate(index_list): #κ·Έ index_listλ₯Ό enumerateλ₯Ό ν΅ν΄ μ«μ(index)μ i λ‘ λ³κ²½νλ€.
        if what == "e": #μ¬κΈ°μ νλΌλ―Έν°3λ²μ§Έ μ‘°κ±΄ whatμ μμ±νλ€. e κ°μ λ£μκ²½μ° λ°λ‘ μλ ν¨μκ° μ€νλλ€.
            index_list[index] = i + n  
        else:
            index_list[index] = i - n #κ·Όλ° λ dλ₯Ό λ£μ΄μ μ΄κ² μ€νλ¨. 
            #ex) [2,1,3] μ[0]λ²μ§Έ = 2 - 1 = 1
            #ex) [2,1,3] μ[1]λ²μ§Έ = 1 - 1 = 0 ....

    print(index_list) #[1, 0, 2]
  #λ°κΎΈλ μ΄μ λ? μμ§μ΄κ³  μΆμ μλ¦¬μ μνλ²³μ κ΅¬νλ €λ©΄ μλ¦¬μλ₯Ό λ¨Όμ  μμμΌνλκΉ.

step3   
    decode_text = "" #μνλ²³μΌλ‘ λ§λ€κ±΄λ° μΌλ¨ κ³΅λμ λ§λ€μ΄μ€
    for i in index_list: #λ§μ§λ§μΌλ‘ μμ±λ index_list [1, 0, 2] λ μ°¨λ‘λ‘ iλ‘ λ€μ΄κ°λ€
        decode_text += n_list[i] #κ·Έ iμ μ«μλ μκΉ μ΄κΈ°μ n_listμ ν΄λΉλμ΄ μ€μ  μνλ²³μΌλ‘ λ€μ λ³νμ΄λλ€
    print(decode_text) #νλ¦°νΈνλ©΄ μμ±


#μ€μ  μ¬μ©μκ° λ£λ μ‘°κ±΄ : cbd λ₯Ό 1μΉΈμ© λ€λ‘ μ?κ²¨μ£ΌμΈμ!  
number(text="cbd", n=1, what="d")
```
```
console

[2, 1, 3]
[1, 0, 2]
bac
```
<br><br><br>
3.+ index κ°λ
```py
my_list = ["a","b","c","d"]

my_list.index("a")
```
<br>console<br>
0<br><br><br>
4. defμμ©λ²2 (def μμ while λ£κΈ°)<br>
```py
alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z','a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

# κ²μμ λμ μ νκΈ° μν΄ while λ£μ΄ go,stopμ κ²°μ ν©λλ€.

def caesar(start_text, shift_amount, cipher_direction):
    end_text = ""
    for letter in start_text:
        position = alphabet.index(letter) #λ½μ μνλ²³μ μ«μλ‘λ³νν΄μ positionμ λ΄μ
        if cipher_direction == "decode":
            shift_amount = shift_amount * -1 #μ€λ₯λΆλΆμ΄μμ
        new_position = position + shift_amount
        end_text += alphabet[new_position]
    print(f"here's the {cipher_direction}d result: {end_text}")



while True:
    ed = input("encode?decode:")
    test = input("input text:")
    shift = int(input("input shift:"))
    caesar(test, shift, ed)
    
    user_input = input("νλ²λ?")
    if user_input == "yes":
        pass
    elif user_input == "no":
        break
```

---
<br><br><br>
3/29 day9
<Br>
```py
student_scores = {
  "Harry": 81,  #νν€μλ νλμ value λ§!
  "Ron": 78,
  "Hermione": 99, 
  "Draco": 74,
  "Neville": 62,
}
# π¨ Don't change the code above π

#TODO-1: Create an empty dictionary called student_grades.

student_grades={}

#TODO-2: Write your code below to add the grades to student_grades.π

for student in student_scores : #student_scoresμ keyλΆλΆμΈ μ΄λ¦μ΄ λ½ν
	score = student_scores[student] #81=student_scores[harry] 
	if score > 90:
		student_grades[student] = "Outstanding"
	elif score > 80:
		student_grades[student] = "exptable"
	elif score > 70:
		student_grades[student] = "acceptable"
	elif score :
		student_grades[student] = "fail"

print(student_grades)

```
```
console
{'Harry': 'exptable', 'Ron': 'acceptable', 'Hermione': 'Outstanding', 'Draco': 'acceptable', 'Neville': 'fail'}
```
<br>
<br><br>

```py
travel_log = [
{
  "country": "France",
  "visits": 12,
  "cities": ["Paris", "Lille", "Dijon"]
},
{
  "country": "Germany",
  "visits": 5,
  "cities": ["Berlin", "Hamburg", "Stuttgart"]
},
]
#π¨ Do NOT change the code above

#TODO: Write the function that will allow new countries
#to be added to the travel_log. π

def add_new_country(country_visited, times_visited, cities_visited):
	new_country = {}
	new_country["country"] = country_visited 
    #"country":"russia"
	new_country["visits"] = times_visited
    #"visits" : 2
	new_country["cities"] = cities_visited
	travel_log.append(new_country) 
    #μμ λ½ν "country":"russia" μ "visits" : 2 κ° travel.log λ€μ νλμ© λΆνμ§
	

def λ‘ ν¨μλ₯Ό λ§λ κ±΄
μλμ²λΌ μ§μ μ¨μ£Όκ±°λ 

or

return κ°μ μ¨μ μ΄μ©
ex) print(defμ΄λ¦(input(a,b)))


#π¨ Do not change the code below
add_new_country("Russia", 2, ["Moscow", "Saint Petersburg"])
print(travel_log)


```
```
console 

[{'country': 'France', 'visits': 12, 'cities': ['Paris', 'Lille', 'Dijon']}, {'country': 'Germany', 'visits': 5, 'cities': ['Berlin', 'Hamburg', 'Stuttgart']}, {'country': 'Russia', 'visits': 2, 'cities': ['Moscow', 'Saint Petersburg']}] 
```
<br><br><br>

*λμλλ¦¬ ν΄μ¦* <br>

```
1. addνλλ² μ λ¦¬
λ¦¬μ€νΈ["c"]=λ΄μ© 
= = = x  
.append()  λ λμλλ¦¬μμ μ¬μ© λΆκ°λ₯. λ¦¬μ€νΈλ§ κ°λ₯


2. μ€λ₯ μ λ¦¬<br>

dict = {"a" : 1
"b" : 2
"c" : 3
}
for key in dict:
    dict[key] +=1

console : a:2   b:3   c:4

3. μνλκ±° μΆλ ₯νλ λ°©λ²
```

```py
Which line of code will print "Steak"?

order = {
    "starter": {1: "Salad", 2: "Soup"},
    "main": {1: ["Burger", "Fries"], 2: ["Steak"]},
    "dessert": {1: ["Ice Cream"], 2: []},

λ°©λ² : print(order["main"][2][0])
# [2]λ key μ΄λ¦ , [0]μ λΆλ¬μ¬ λ΄μ©μ μμ
```


AUCTION PROGRAM
```py

from replit import clear #???????
#HINT: You can call clear() to clear the output in the console.

from art import logo
print(logo)


def bid(name, price)
    bids = {} 
	bids["μ΄λ¦"] = name
	bids["λ"] = price
    bids.append(bid)


while True:
    name = input("what is your name?")
    price = input("what is your bids?")
    continu = input("wanna go? yes or no")
    bid(name, price)
    

    if ucontinu == "yes":
        pass
    elif continu == "no":
        #μ¬κΈ°μ μ μΌλμ nameκ³Ό price μ κ°κ²©μ μΆμΆν μμλ μ‘°κ±΄μ κ±Έλ©΄ λ¨.
        break

```

```py
*λμλλ¦¬μ μ€μν κ·μΉ*

1. μ½€λ§λ‘ κ΅¬λΆνλ€

my_dict = {
    "key" : value, #μ½€λ§λ‘ κ΅¬λΆ
    "key2": value,
        ...
}


2. forλ¬Έμ κ·Έλ₯ λλ¦¬λ©΄ ν€λ§ λμ¨λ€.

for key in my_dict : 
    print(key)

console : "key" , "key2"




3. itemsλ₯Ό μ°κ³  forλ¬Έμ λλ¦¬λ©΄ ν€,valueκ° κ°μ΄ λμ¨λ€.

for key,value in my_dict.items(): # .items() μ°λ©΄ keyκ°κ³Ό valueκ°μ΄ κ°μ΄ λμ΄
    print(key, value)

console : "key" : value, "key2": value,



4. λμλλ¦¬μμ μνλκ±Έ μΆμΆνλ λ°©λ²

order = {
    "starter": {1: "Salad", 2: "Soup"},
    "main": {1: ["Burger", "Fries"], 2: ["Steak"]},
    "dessert": {1: ["Ice Cream"], 2: []},
}

Steak μΆμΆνλλ²μ
order["main"][2][0] #λ©μΈλ¦¬μ€νΈμμ 2λ²μ§Έλ¦¬μ€νΈμ 0λ²μ§Έλ¨μ΄λ₯Ό μΆμΆν¨

```   

<br><br><br>
3/30 day10<br>
def μμ if,return λ£κΈ°

```py
def format_name(f_name, l_name):
  if f_name == "" or l_name == "":
    return "You didn't provide valid inputs."
  formated_f_name = f_name.title()  #titleμ Yerin μ²λΌ μμλ¦¬λ§ λλ¬Έμλ‘ λ°κΏμ€
  formated_l_name = l_name.title()
  f"Result: {formated_f_name} {formated_l_name}"

#Storing output in a variable
formatted_name = format_name(input("Your first name: "), input("Your last name: "))
print(formatted_name)
```

```py
def is_leap(year):
  if year % 4 == 0:
    if year % 100 == 0:
      if year % 400 == 0:
        return True
      else:
        return False
    else:
      return True
  else:
    return False

month_days = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]

def days_in_month(year, month):
	if is_leap(year) and month == 2:   #is_leap(year)μ΄ true , month=2 true μΌκ²½μ°μλ§ 29λ₯Ό λ¦¬ν΄ν΄μ€.
		return 29
	return month_days [month - 1]
  
#π¨ Do NOT change any of the code below 
year = int(input("Enter a year: "))
month = int(input("Enter a month: "))
days = days_in_month(year, month)
print(days)
```
```
console
Enter a year: 2020
Enter a month: 2
29
```
<br><br>

**ν΄μ¦**

```py
1.What would you predict to be the result of running the following code?

def outer_function(a, b):
    def inner_function(c, d): #2. κ·Έλ¦¬κ³  λ°μ  inner_function μ returnμ ν΄μ λ°λ‘ μ΄ λκ°μ ν¨μκ° μνμ΄ λλλ― ???
        return c + d
    return inner_function(a, b) #1. outer_function(a, b)μ λν returnκ°μΈ μ΄μ€μ΄ λ°λ‘ μ€νλλλ― ???
 
result = outer_function(5, 10)
print(result)

console=15




2.What will be printed in the console after running the following code?

def my_function(a):
    if a < 40:
        return   #return λ€μμ λ°λ‘ μμ΄μΌλλλ° μμ΄μ noneκ°!!
        print("Terrible")
    if a < 80:
        return "Pass"
    else:
        return "Great"
print(my_function(25))

console=none

```

κ³μ°κΈ°λ¬Έμ 
```py
def add(n1,n2):
	return n1 + n2

def sub(n1,n2):
	return n1-n2

def mul(n1,n2):
	return n1*n2

def div(n1,n2):
	return n1/n2

# if choose == '+' :
# 	add(add_1,add_2)
#λμλλ¦¬ λ§λ€κΈ°!!
calculate={
	"+":add,
	"-":sub,
	"*":mul,
	"/":div
}

num1=int(input("what 1?"))  #inputμ str μΌλ‘ λ°μμ Έμ μ€λ₯λ¨ int λ£κΈ°!!
num2=int(input("what 2?"))

choose=input("what do u want?")
#for symbol in calculate:
symbol = calculate[choose] 
print(symbol)   
result = symbol(num1, num2)
print(result)
```

<br><br>
κ³μ°κΈ°λ¬Έμ  μμ±λ³Έ
```py
from replit import clear

def add(n1, n2):
  return n1 + n2

def subtract(n1, n2):
  return n1 - n2

def multiply(n1, n2):
  return n1 * n2

def divide(n1, n2):
  return n1 / n2

operations = {
  "+": add,
  "-": subtract,
  "*": multiply,
  "/": divide
}

def calculator(): #def calculator μμ for λ¬Έκ³Ό while λ¬Έμ λ£μ, λ³΄λ©΄ λ°μ calculator()λ₯Ό λ°λ‘ μ¨μ€μΌ μ΄ ν¨μκ° μνλ¨
  

  num1 = float(input("What's the first number?: ")) #num1 λ§ λ°λ‘ λΉΌλμ
  for symbol in operations:
    print(symbol)
  should_continue = True  #trueλ‘ κ°μ ν¨μΌλ‘μ¨ whileλ¬Έμ΄ μνλκ±΄κ°? γγ
#forλ¬ΈμΌλ‘ κΌ­ λλ¦¬μ§ μμλ while λ°λ³΅μ μν΄μ  true λΌλ κ°μ μ΄ νμνκ±°. κ·Έλ¬λκΉ calculaator()μ΄ ν¨μμ ture λ μ€μμΉλ₯Ό λ°λ‘ λ£μ΄λλ¨
 
  while should_continue: #μ΄μνλ true
    operation_symbol = input("Pick an operation: ")
    num2 = float(input("What's the next number?: "))
    calculation_function = operations[operation_symbol]
    answer = calculation_function(num1, num2)
    print(f"{num1} {operation_symbol} {num2} = {answer}")

    if input(f"Type 'y' to continue calculating with {answer}, or type 'n' to start a new calculation: ") == 'y': #λ°μκ² false λκΉ μλμΌλ‘ μ΄ yλ trueκ° λ¨
      num1 = answer
    else:
      should_continue = False
      clear()
      calculator()

calculator()
```
<br><br>
νΌμ λ§λ€μ΄λ΄
```py


def add(n1, n2):
  return n1 + n2

def subtract(n1, n2):
  return n1 - n2

def multiply(n1, n2):
  return n1 * n2

def divide(n1, n2):
  return n1 / n2

operations = {
  "+": add,
  "-": subtract,
  "*": multiply,
  "/": divide
}

#num1 , num2 , μ¬λμ΄ μνλ©΄ κ³μ°λκ±°μμ μκ³Ό num2λ§ λ°κΏμ μ­ μ§νμν€κ³ ν

def calculator():
	num1 = float(input("what is yout first number??"))
	go = True # =λμ  : μ¨μ νλ¦Ό
	
	while go:
		symbol = input("what symbol?") #μμΌλ¬Έμμ λμ΄μ°κΈ°μν΄μ νλ¦Ό
		oper_2 = operations[symbol]
		num2 = float(input("what is yout second number??")) #float μμ¨μνλ¦Ό
		result = oper_2(num1,num2)
		print(f"{num1} {symbol} {num2} = {result}")
		if input("you want keep y or n") == 'y' :  # y ''λ‘ μκ°μΈμ νλ¦Ό
			num1 = result
		else :
			go : False
	
calculator()

```
<br><br><br>
4/1 blackjak game
```py

############### Our Blackjack House Rules #####################

## The deck is unlimited in size. 
## There are no jokers. 
## The Jack/Queen/King all count as 10.
## The the Ace can count as 11 or 1.
## Use the following list as the deck of cards:
## cards = [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
## The cards in the list have equal probability of being drawn.
## Cards are not removed from the deck as they are drawn.
## The computer is the dealer.

##################### Hints #####################

import random



def deal_card():
	cards = [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
	card = random.choice(cards)
	return card



#μμΉνλ Έμ  score μμμ μμ΄μΌ λ°μ μ μλ₯Ό κ°μ§κ³  ν¨μκ° μ¬μ©μ΄ λλ€ 
def compare(computer_score,user_score):  #μλ¬λΈ -> μμ νλΌλ―Έν° λΉ μ§
	if computer_score == user_score :     #νλΌλ―Έν°μ΄λ¦μ ν¨μμμμ λμΌν¨, λ°μμ€λ νλΌλ―Έν°μ μ΄λ¦μ λ¬λΌλ μκ΄μμ ex. compare(a,b)
		return "draw" #return λΉΌλ¨Ήμ
	elif computer_score == 0 :	
		return "lose, opponent has blacjak"
	elif  user_score == 0 :	
		return "win, has blacjak"
	elif  user_score > 21 :	
		return "loose"
	elif  computer_score > 21 :	
		return "you win"
	elif computer_score < user_score :
		return "you win"
	else:
		return "you loose"

def calculate_score(cards):
	#user_card μ΄κ±΄ κ·Έλ₯ (cards) μλ¦¬μ λλ©΄ λλκ±°!!
	if sum(cards) == 21 and len(cards) == 2:
		return 0	
	if 11 in cards and sum(cards) > 21 : #11 in cards andμ΄κ±° λΉΌλ¨Ήμ
		cards.remove(11)	#return 1μ΄λΌκ³  νλ¦Ό
		cards.append(1)

	return sum(cards) 

def play_game():
	user_cards = []
	computer_cards = []
	is_game_over = False 
	
	#κ²μ end λ μ€μμΉλ‘ forλ¬Έ λ°μ λ£λλ€
	
	for _ in range(2): #λ°λ³΅ν΄μ λ¦¬μ€νΈμ μΆκ°λ§ ν  μ©λ
		pick = deal_card()	#μ¬κΈ°νλ¦Ό
		user_cards.append(pick)  # += μ λ¦¬μ€νΈλ§ κ°λ₯, pickκ³Ό κ°μ΄ νλμ μλ appendλ₯Ό μ΄μ©!
		computer_cards.append(deal_card()) #μ΄λ κ² μΆμ½λ¬Έλ κ°λ₯
	
	while not is_game_over :	#is_game_over μ΄ true κ° λ  λ λ°λ³΅μ λ©μΆλ€.	
		user_score = calculate_score(user_cards)
		computer_score = calculate_score(computer_cards)
		print(f" your cards : {user_cards} , score is {user_score}")
		print(f" computer first cards : {computer_cards[0]} ")
		
		
		if user_score == 0 or computer_score ==0 or user_score > 21 : #μ΄κ±° λ§λ€κ³  ν΄λ¬Έ μμ true false μ€μμΉ ν€ λ§λ€κΈ°
			is_game_over = True #trueλ©΄ κ²μ μ€λ²λλκ². μμκ° false μΈκ²λ§μΌλ‘λ κ²μμ΄ λλ μκ°μλ?γ΄γ΄ whileλ¬Έμ λ£κΈ°! ??
		else:
			y = input("'y' to get another card, 'n' to pass ")
			if y == 'y' :
				pick = deal_card()	
				user_cards.append(pick)  # λ λ¦¬μ€νΈ λ€μ νμ₯ μΆκ°
			else :
				is_game_over : True #λΉΌλ¨Ήμ
	
	while computer_score != 0 and computer_score < 17 : #stopμ 17λ³΄λ€ ν΄λ ?
		computer_cards.append(deal_card())  #17λ³΄λ€ μμΌλ©΄ νμ₯ λ λ½λκ±΄κ°?
		computer_score = calculate_score(computer_cards)  
				b
	print(compare(computer_score, user_score))
		
#λ°λ³΅νκ³ μΆμλλ μ§κΈκΉμ§ ν λͺ¨λ  ν¨μλ€μ λ λ°λ³΅μν€λ ν¨μμ μ§μ΄λ£μΌλ©΄λ¨. ex play_game()

while input("you waana paly? 'y' is connet ") == "y" :  #ifλ‘ μλͺ»μ&μμλΆλΆμ΄λΌ μμλΆνκΈ°
	play_game()
```
<br><br><br>
4/2 local , global scope κ°λ ν΄μ¦
```py
1.def a_function(a_parameter):
    a_variable = 15
    return a_parameter
 
a_function(10)
print(a_variable)

λ΅: name error

```


```py
def mutate(a_list):
  b_list = []
  for item in a_list:
    new_item = item * 2
    b_list.append(new_item)
  print(b_list) #def μμλ§ μλ μν

mutate([1,2,3,5,8,13])
```
```
console
[2, 4, 6, 10, 16, 26]
```
<br><br>
4/4 μ«μλ§μΆκΈ°κ²μ
```py
import random


type = input("welcome , choose type 'easy' or 'hard'.")

random2=int(random.randint(1,101))
print(random2)
number = int(input("make a guess."))

if type == 'easy':
	attempts = 5
if type == 'hard':   #μ ifλ¬Έμ μνκ² λλ©΄ typeμΌλ‘ hardλ₯Ό λ£μμκ²½μ° easyλ§ μ½κ³  λμ΄κ°μ attemptsλ μλκ² λ¨
	attempts = 10

for _ in range(0,int(attempts)):
	attempts = attempts-1
	if random2>number : 
		print(f"too low.  you have {attempts} attempts.")
	elif random2<number :
		print(f"too higt. you have {attempts} attempts.")
	elif random2==number :    #elif*
		print("good.")
		break   
	number = int(input("make a guess."))

print("You've run out of guesses, you lose.") #λΉΌλ¨Ήμ

  ```
```
console

welcome , choose type 'easy' or 'hard'.easy
98
make a guess.99
too higt. you have 4 attempts.
make a guess.97
too low.  you have 3 attempts.
make a guess.98
good.
```

<br><br>
μ μλλ²μ 
```py
from random import randint

EASY_LEVEL_TURNS = 10
HARD_LEVEL_TURNS = 5

#Function to check user's guess against actual answer.
def check_answer(guess, answer, turns): 
  """checks answer against guess. Returns the number of turns remaining."""
  if guess > answer:
    print("Too high.")
    return turns - 1
  elif guess < answer:
    print("Too low.")
    return turns - 1
  else:
    print(f"You got it! The answer was {answer}.")

#Make function to set difficulty.
def set_difficulty():
  level = input("Choose a difficulty. Type 'easy' or 'hard': ")
  if level == "easy":
    return EASY_LEVEL_TURNS
  else:
    return HARD_LEVEL_TURNS

def game():
  print("Welcome to the Number Guessing Game!")
  print("I'm thinking of a number between 1 and 100.")
  answer = randint(1, 100)
  print(f"Pssst, the correct answer is {answer}") 

  turns = set_difficulty()

  guess = 0
  while guess != answer: #λκ°κ° λ€λ₯Έν true λκΉ κ³μ λ°λ³΅
    print(f"You have {turns} attempts remaining to guess the number.")
    guess = int(input("Make a guess: "))
    turns = check_answer(guess, answer, turns)  #turns μ λ£μ printκ°μ΄ λμ¬κ².
    if turns == 0:
      print("You've run out of guesses, you lose.")
      return
    elif guess != answer:
      print("Guess again.")


game()

```


<br><br>
4/7 μ»€νΌλ¨Έμ 
```py

MENU = {
    "espresso": {
        "ingredients": {
            "water": 50,
            "coffee": 18,
        },
        "cost": 1.5,
    },
    "latte": {
        "ingredients": {
            "water": 200,
            "milk": 150,
            "coffee": 24,
        },
        "cost": 2.5,
    },
    "cappuccino": {
        "ingredients": {
            "water": 250,
            "milk": 100,
            "coffee": 24,
        },
        "cost": 3.0,
    }
}
money = 0
resources = {
    "water": 300,
    "milk": 200,
    "coffee": 100,
}


def resources_sufficient(drink):
    for item in drink:  # drink μ ν€κ°μ΄ λμ΄. λμ€μ νλΌλ¨ΌνΈμλ€κ° λ κΉν μ§μ΄λ£μΌλ©΄ μ«μλ‘ λ΄λ³΄λ΄μ§μμμ΄
        if resources[item] < drink[item]: #resoureces = {water:300, milk;200, coffe:100} item 1λ²μ§Έ[water]
            print("Sorry there is not enough resources.")
            return False
        return True


def process_coins():
    quarters = int(input("how many quarters?")) * 0.25
    dimes = int(input("how many dimes?")) * 0.10
    nickles = int(input("how many nickles?")) * 0.05
    pennies = int(input("how many pennies?")) * 0.01
    total = quarters + dimes + nickles + pennies
    return total


def transaction_successful(menu_cost, inserted_coin):
    global money
    if menu_cost <= inserted_coin:
        change = round(inserted_coin - menu_cost, 2)
        money += round(inserted_coin-change, 2)
        print(f"Here is ${change} dollars in change.")
        return True
    else:
        print("Sorry that's not enough money. Money refunded.")
        return False

def report():
    print(f"water: {resources['water']}")  # fμ€νΈλ§κ³Ό λμλλ¦¬ ν¨κ» μ°λλ² **
    print(f"milk: {resources['milk']} ")
    print(f"coffee: {resources['coffee']} ")
    print(f"money : {money}")


def make_coffee(drink_name, order_ingredients):
    """Deduct the required ingredients from the resources."""
    for item in order_ingredients:  # water milk μ°¨λ‘λλ‘ λ€μ΄κ°κ² λ§λ¬
        resources[item] -= order_ingredients[item]
    print(f"Here is your {drink_name} βοΈ. Enjoy!")


is_going = True
while is_going:  # λ¬΄νλ°λ³΅
    answer = input("What would you like? (espresso / latte / cappuccino) : ")
    if answer == "off":  # μ²«λ²μ§Έ μ€μ
        is_going = False
    elif answer == "report":
        print(f"water: {resources['water']}")  # fμ€νΈλ§κ³Ό λμλλ¦¬ ν¨κ» μ°λλ² **
        print(f"milk: {resources['milk']} ")
        print(f"coffee: {resources['coffee']} ")
        print(f"money : ${money}")
    else:
        drink = MENU[answer] #MENU[latte] -> "ingredients":"water": 200 ..."cost": ...
        if resources_sufficient(drink["ingredients"]):   #latte["ingredients"] -> water:x , milk:y ...
            pay = process_coins()
            if transaction_successful(drink["cost"], pay):
                make_coffee(answer, drink["ingredients"])

*λμλλ¦¬λ λΆλ¬μ¬λ μ§μ νλ©΄ ex)whileλ¬Έ μμ drink=MENU[ansewr]  λμ ν¨μλ₯Ό λ§λ€λλ μλ¦Ώμλ₯Ό μκ΄ν νμκ° μλκ±°κ°λ€.

```
CONSOLE
```
What would you like? (espresso / latte / cappuccino) : latte
how many quarters?9
how many dimes?9
how many nickles?9
how many pennies?9
Here is $1.19 dollars in change.
Here is your latte βοΈ. Enjoy!
What would you like? (espresso / latte / cappuccino) : report
water: 100
milk: 50 
coffee: 76 
money : $2.5
What would you like? (espresso / latte / cappuccino) : off
```

<br><br>
**κ·ΈμΈ λ¬Έλ² μ λ¦¬**
```py
1.with
: λ€λ₯Έ νμΌμ κ°μ Έμ€κ±°λ μμ±λ κ°λ₯

ex) 50μ£Όμ°¨μ λ³΄κ³ μ νμΌμ λ§λλ νλ‘κ·Έλ¨μ μμ±νλΌ(μ΄50κ°μ νμΌμ μμ±)
for i in range(1, 51)
  with open(srt(i) + "μ£Όμ°¨", "w", encoding="uft8")as report_file:
# (μ λͺ©/"w"=μμ±νλ€λμλ―Έ / "utf8"=νκΈμ¬μ©/ "as"=λ³μμ΄λ¦μ§μ 
  report_file.write("νμ΄μ¬κ³΅λΆμ€μ΄μμ")

console
νμ΄μ¬κ³΅λΆμ€μ΄μμ λΌλ λ΄μ©μ 50κ° λ¬Έμκ° μκΉ
	
	
	
	
1-1. μλλ° μ λνμΌμ μ΄μ©νμ¬ λ©μΌλ¨Έμ§νλ‘μ νΈμμ±

# 1. μμλ¬Έμ λ³κ²½λ  λ§€μ²΄ [name] λ₯Ό μ μνλ€. λ¦¬μ€νΈλ μΆνμ μ¬μ©λ  replace λΌλ ν¨μμ μ¬μ©μ΄ μλκΈ°λλ¬Έ.
PLACEHOLDER = "[name]"

	
	#2.μ λκ²½λ‘λ₯Ό μ΄μ©ν΄ μ΄μ©ν  μ΄λ¦ λ¦¬μ€νΈλ₯Ό κ°μ Έμ΄
with open("./Input/Names/invited_names.txt") as names_file:
	#3.readlines() λΌλ ν¨μλ₯Ό μ΄μ©ν΄ λ¦¬μ€νΈλ‘ μλ₯Έλ€.
    names = names_file.readlines()

	#4.μμλ¬Έ txt λ₯Ό κ°μ Έμ¨λ€
with open("./Input/Letters/starting_letter.txt") as letters_file:
    letters = letters_file.read()
	#5.μκΉ λλ λ¦¬μ€νΈλ₯Ό for μ μ΄μ©ν΄ νλνλ μ΄μ©νλ€.
    for name in names:
        stripped_name = name.strip()  #strip μ΄λΌλ ν¨μλ λ¦¬μ€νΈμλ λΆκ°λ₯. μ¬λ¬κ°λ for λ¬Έ μ΄μ© νμ
        new_letter = letters.replace(PLACEHOLDER,stripped_name) #λ¦¬μ€νΈλ replace κ° λΆκ°λ₯μ΄λΌ μμ μλ‘ μ μλ₯Ό ν΄μ£Όμλ€.
	#6.μ΄λ νμΌμ open νλλ° "w" λͺ¨λλ‘ μλ‘­κ² μ€νμν¨λ€. κ·Έλ μμ replace λ‘ μ΄λ¦μ λ£μ μλ²½ν νΈμ§ μ μνκ±Έ write λ΄μ©μ λ£μ΄μ€λ€.
	#7.κΈ°μμ΄λ©΄ open μμ μ΄λ¦μ fμ€νΈλ§μ μ¬μ©ν΄ μ λͺ©μ λΆλ₯ν΄μ£Όλ©΄ μ’λ€.
        with open(f"./Output/ReadyToSend/letter_for_{stripped_name}.txt", mode="w") as completed_letters:
            completed_letters.write(new_letter)


2.ν΄λμ€ (νμν μ΄μ :   )
μμ ν¨μλ₯Ό λ©μλλΌ λΆλ¦
class Unit:  #(class μμ μ΄λ¦)
    def __init__(self, name, hp, damage):
        self.name = name
        self.hp = hp
        self.damage = damage
        print("{0} μ λμ΄ μμ±λμλ€".format(self.name)
        print("μ²΄λ ₯: {0}, κ³΅κ²©λ ₯: {1}".format(self.hp, self.damage))

2-1 μ¬μ©λ²:  
marine1 = Unit("λ§λ¦°",40,5) #κ°μ²΄λΌ ν¨
tank = Unit("ν±ν¬",150,35) 

2-2 init μ΄λ?
μμ±μ : init ν¨μμ μ§μ λ μκ·λ¨ΌνΈ λ§νΌ λ£μ΄μ€μΌν¨ 3κ°

2-3 λ©€λ²λ³μλ?
ν΄λμ€μμ μ§μ λ κ²λ€
ex) self.name = name 

#μμ 1 ! μΈλΆμμ νλ μλ μ΄λκ±Έ λ§λ€μ΄λ΄μλ€
wraith = Unit("λ μ΄μ€",80,5)
print("μ λμ΄λ¦:{0},κ³΅κ²©λ ₯:{1}".format(wraith.name, wraith.damage))
#μ΄λ κ² κΈ°μ‘΄μ μ€μ λ λ³μμ μλ‘μ΄ λ³μλ₯Ό λ£μ΄ μμ©μ΄ κ°λ₯ν¨

console : 
λ μ΄μ€ μ λμ΄ μμ±λμλ€. #-> def init λ΄λΆν¨μκ°
μ²΄λ ₯: 80, κ³΅κ²©λ ₯: 5     #-> def init λ΄λΆν¨μκ°
μ λμ΄λ¦:λ μ΄μ€, κ³΅κ²©λ ₯:5 #-> def initμ μμ©ν μΈλΆ ν¨μκ°

#μμ 2!
wraith2 = Unit("λΉΌμμ λ μ΄μ€",80,5) #1. Unit μ΄μ©
wraith2.clocking = True #μ΄μ©λ ν¨μμ .clocking μ΄λΌλ λ³μλ₯Ό μΆκ°ν΄μ€

if wraith2.clocking == True:
print("{}λ ν΄λ‘νΉμ΄λ€".format(wraith2.name))


2-4 λ©μλλ?
class AttackUnit: 
    def __init__(self, name, hp, damage):
        self.name = name
        self.hp = hp
        self.damage = damage
        

    def attack(self, location):
        print("{0}:{1} λ°©ν₯μΌλ‘ κ³΅κ²©. κ³΅κ²©λ ₯:{2}".format(self.name, location, self.damage)) #def λ€λ₯Έλ° μ¬κΈ°μ λΆλ¬μμ§λ {0}:self.nameμ μμμ μ μλμ λ‘ λΆλ¬μμ§λ€!!
        #location μ μ΄νν¨μμμ λ°μ μ λ‘ λΆλ¬μμ§

    def damaged(self, damage):
        print("{0}:{1} λ°λ―Έμ§μμ.".format(self.name, damage)) 
        self.hp -= damage
        print("νμ¬μ²΄λ ₯{0}".format(self.hp))
        if self.hp <= 0:
          print("{0} νκ΄΄λ¨".format(self.name))


#μ μ©ν΄λ³΄μ
#1λ²μ§Έλ‘ ν κ²: AttackUnit ν΄λμ€ μ μ©νκΈ° /
firevat1 = AttackUnit("νμ΄μ΄λ±",50,16) #νλ¦°νΈλ°λ‘ μλ¨ (μμ±μλΌμ μ§μ λ§ν΄μ€) / μμμ init ν¨μ νκ·λ¨ΌνΈ!!

#κΈ°λ³Έ ν΄λμ€κ° μ μ©λ μνμμ λ΄λΆν¨μλ₯Ό μ μ©
firevat1.attack("5μ")
firevat1.damaged(25)
firevat1.damaged(25)

console
νμ΄μ΄λ±:5μ λ°©ν₯μΌλ‘ κ³΅κ²©. κ³΅κ²©λ ₯:16
νμ΄μ΄λ±:25 λ°λ―Έμ§μμ.
νμ¬μ²΄λ ₯25
νμ΄μ΄λ±:25 λ°λ―Έμ§μμ.
νμ¬μ²΄λ ₯0
νμ΄μ΄λ± νκ΄΄λ¨


2-5 μμμ΄λ?
κΈ°λ³Έν΄λμ€μ λλ€λ₯Έν΄λμ€μ κ²ΉμΉλ λΆλΆμ΄ μλ€λ©΄ μμμ ν΅ν΄ μ²λ¦¬νλ€.

#κΈ°λ³Έμ λ
class Unit: 
    def __init__(self, name, hp):
        self.name = name
        self.hp = hp

#μ΄νμ λ
class AttackUnit(Unit): #1λ². nameκ³Ό hpκ° κ²ΉμΉλ μμμ΄ νμ --> μ λμ ()μμ μμλ°μ κΈ°λ³Έν΄λμ€λͺ λ£κΈ°
    def __init__(self, name, hp, damage):
        #self.name = name #2λ². κ²ΉμΉλλΆλΆμ­μ 
        #self.hp = hp
        Unit.__init__(self, name, hp)#3λ². κΈ°λ³Έ ν΄λμ€ νΈμΆ
        self.damage = damage #4λ².(μμ©): κΈ°λ³Έν΄λμ€μ μλ λ€λ₯Έλ³μλ₯Ό μΆκ°ν¨
        

    def attack(self, location):
        print("{0}:{1} λ°©ν₯μΌλ‘ κ³΅κ²©. κ³΅κ²©λ ₯:{2}".format(self.name, location, self.damage))
        
    def damaged(self, damage):
        print("{0}:{1} λ°λ―Έμ§μμ.".format(self.name, damage)) 
        self.hp -= damage
        print("νμ¬μ²΄λ ₯{0}".format(self.hp))
        if self.hp <= 0:
          print("{0} νκ΄΄λ¨".format(self.name))

#μ μ©ν΄λ³΄μ
#firbat = Unit("νμ΄μ΄λ±",50) νλ¦Ό Unitμ AttackUnitμ μμνμΌλ μΈ νμ μμ!!
firbat = AttackUnit("νμ΄μ΄λ±",50,16)
firbat.damaged(25)
firbat.damaged(25)

console
νμ΄μ΄λ±:25 λ°λ―Έμ§μμ.
νμ¬μ²΄λ ₯25
νμ΄μ΄λ±:25 λ°λ―Έμ§μμ.
νμ¬μ²΄λ ₯0
νμ΄μ΄λ± νκ΄΄λ¨

2-6 λ€μ€μμμ΄λ?
μμλ°λκ² λκ° μ΄μμΈκ²

class Unit: 
    def __init__(self, name, hp):
        self.name = name
        self.hp = hp

#μ΄νμ λ
class AttackUnit(Unit): #1λ². nameκ³Ό hpκ° κ²ΉμΉλ μμμ΄ νμ --> μ λμ ()μμ μμλ°μ κΈ°λ³Έν΄λμ€λͺ λ£κΈ°
    def __init__(self, name, hp, damage):
        #self.name = name #2λ². κ²ΉμΉλλΆλΆμ­μ 
        #self.hp = hp
        Unit.__init__(self, name, hp)#3λ². ν΄λμ€ νΈμΆ
        self.damage = damage #4λ².(μμ©): κΈ°λ³Έν΄λμ€μ μλ λ€λ₯Έλ³μλ₯Ό μΆκ°ν¨
        
    def attack(self, location):
        print("{0}:{1} λ°©ν₯μΌλ‘ κ³΅κ²©. κ³΅κ²©λ ₯:{2}".format(self.name, location, self.damage))
        
    def damaged(self, damage):
        print("{0}:{1} λ°λ―Έμ§μμ.".format(self.name, damage)) 
        self.hp -= damage
        print("νμ¬μ²΄λ ₯{0}".format(self.hp))
        if self.hp <= 0:
          print("{0} νκ΄΄λ¨".format(self.name))

#ν΄λμ€ νλ λ μΆκ° : λ μμλ κΈ°λ₯ μΆκ°
class Flyable:
    def __init__(self, flying_speed):
      self.flying_speed = flying_speed #λ©€λ²λ³μ μ΄κΈ°ν = λ€λ₯Έλ°μλ μΈμμκ²ν΄μ£Όλ μμ???

    def fly(self, name, location):
      print("{0} : {1} λ°©ν₯μΌλ‘ λ μκ°. μλλ{2}".format(name,location,self.flying_speed)) #name,location μ μλ‘λ°μμΌνλ, flying_speedλ μμ init ν¨μλ₯Ό ν΅ν΄ μ¬μ©μ΄ λ¨.


#κ³΅κ²©κ³Ό λ μμλ μ λ ν΄λμ€ λ§λ€κΈ°(λ€μ€μμ)
class Flyable_Attack(AttackUnit, Flyable):
    def __init__(self, name, hp, damage, flying_speed):
  #1λ². μ€λ³΅λ name,hp,damage λ μ΄νν΄λμ€μ μ μλμμ.
      AttackUnit.__init__(self, name, hp, damage)
  #flyingspeedλ νλΌμ΄μ΄λΈμ μ μλ¨
      Flyable.__init__(self, flying_speed)

valkyrie = Flyable_Attack("λ°ν€λ¦¬",200,6,5)
valkyrie.fly("λ°ν€λ¦¬","3μ")

console
λ°ν€λ¦¬ : 3μ λ°©ν₯μΌλ‘ λ μκ°. μλλ5

```

list = 
dict[1] = 4 μ΄κ±΄μΆκ°νλκ±°μ

```python
#list comprehension

[ μΆλ ₯λ¬Ό for num in list ]		       
list λ₯Ό νλμ© num μΌλ‘ κ°μ Έκ°κ³  μ΅μ’ μΆλ ₯μ μΆλ ₯λ¬Όλ‘ κ°μ Έμ¨λ€. μΆλ ₯λ¬Όμ μ¬λ¬ μμμ κ±Έμκ° μμ 
		       
1.κΈ°μ‘΄ μ«μ λ¦¬μ€νΈμ 1μ© μΆκ°νκΈ°
number=[1,2,3]
new_numbers = [item+1 for item in number]

2.string λΆν΄νκΈ°
name="Angela"
list=[letter for letter in name]

3.κ° μ«μ 2μ© κ³±νκΈ°
numm =[num*2 for num in range(1,5)]

4.μ‘°κ±΄ κ±ΈκΈ°
names =["Alex","Beth","Caroline","Dave","Elanor","Freddie"]
short_name=[name for name in names if len(name) < 5]
long_name=[name.upper() for name in names if len(name) > 5]
	
5.μ‘°κ±΄ κ±ΈκΈ° - λκ°μ txt μ€λ³΅ μ²΄ν¬νκΈ°
with open("file1.txt") as names_file:
    file1 = names_file.readlines()
with open("file2.txt") as names_file:
    file2 = names_file.readlines()

result = [int(text.strip()) for text in file1 if text in file2 ]
print(result)
```
	
```python

with open("../pythonProject2/weather_data.csv") as names_file:
	#3.readlines() λΌλ ν¨μλ₯Ό μ΄μ©ν΄ λ¦¬μ€νΈλ‘ μλ₯Έλ€.
    names = names_file.readlines()

print(names)

import csv

# with open("weather_data.csv") as data_file:
#     data = csv.reader(data_file)
#     temperature = []
#     for row in data:
#         if row[1] != "temp":
#             temp = row[1]
#             temperature.append(int(temp))
#     print(temperature)

# μμ κΈ΄ μ½λλ₯Ό pandasλ₯Ό μ΄μ©ν΄ μ½κ² μ²λ¦¬ κ°λ₯

import pandas
data = pandas.read_csv("weather_data.csv")
#1 μ΄μ μ΄λ¦μΌλ‘ μ°Ύμμ μμ

print(data["temp"])

#2 λ°μ΄ν°λ₯Ό λμλλ¦¬λ‘ λ°κΎΈλ λ²
data_dic = data.to_dict()

#3 λ°μ΄ν° temp μ΄μ λ¦¬μ€νΈλ‘ λ°κΎΈλ λ²
data_lis = data["temp"].to_list()

avg = (sum(data_lis) / len(data_lis))
# print(data_lis.mean())
# print(data["temp"].max())


#4 νΉμ  νμ μ°Ύλλ²
print(data[data.day == "Monday"])

#5 κ°μ₯λμ μ¨λκ° μλ νμ μ°ΎμλΌ
print(data[data.temp == data["temp"].max()])  #data[~~~] μ΄κ² data κ°μ²΄λ₯Ό μ μ©μν€λκ²

#5-2 μμμΌμ μ¨λλ₯Ό μ°ΎμλΌ
 monday = data[data.day == "Monday"]
 print(monday.temp)

#6 λ°μ΄ν°νλ μλ§λ€κΈ°
data_dic_2 = {
    "students" : ["amy" , "jame", "jin"],
    "score": [70,50,80]
}
# μμ λμλλ¦¬λ₯Ό μ΄μ©ν΄ νλ§λ€κΈ°
print(pandas.DataFrame(data_dic_2))


#νλ©΄μ μ°μμλ μ’ν μ»λλ²
 def get_mouse_click_coor(x,y):
    print(x,y)
turtle.onscreenclick(get_mouse_click_coor)
screen.mainloop()





--------------

pandasλ₯Ό μ΄μ©ν΄ κ²μμμ± (csv κ°μ Έμ€κ³ , λΉκ΅νκ³  μμ±νκΈ°)

import turtle
import pandas

screen = turtle.Screen()
screen.title("US stage game")
image = "blank_states_img.gif"
screen.addshape(image)
turtle.shape(image)

data = pandas.read_csv("50_states.csv")
state_datas = data["state"]
data_state = state_datas.to_list()

#all_states = data.state.to_list() μμκ±° νμ€λ‘ λ§λ€κΈ° data μ state μ΄μ to_list μ΄μ©ν΄ λ¦¬μ€νΈλ‘ λ³ν
#guessed_states = []



states_list = []
while len(states_list) < 50:
    # νλ©΄μ μλ ₯μ°½ λμ°λλ²
    answer_state = screen.textinput(title=f"{len(states_list)}/50 state", prompt="what is another state name?")
    answer_state = answer_state.title() #titleν¨μλ μ²«μλλ¬Έμ λλ¨Έμ§ μλ¬Έμλ‘ λ³ν
    if answer_state == "Exit":
        #μ μ κ° λκ°λ λͺ»μ°Ύμ λλ¨Έμ§ λ¦¬μ€νΈ csv νμΌμ μ μ₯νκΈ°
        missing_state = []
        for state in data_state: 
            if state not in states_list: #λ΅μ§μ μ£Όκ° μ μ κ° μμ±ν states_list μ μλ€λ©΄.
                missing_state.append(state)
	# μμ 4μ€ λ¦¬μ€νΈμ»΄νλ¦¬ν¨μμ¬μ©ν΄μ
	# νμ€λ‘ κ°λ₯ missing_states = [state for state in all_states if state not in guessed_states]
        new_data = pandas.DataFrame(missing_state) #κ·Έ λ―Έμ± λ¦¬μ€νΈλ₯Ό df λ‘ λ³κ²½
        new_data.to_csv("states_to_learn.csv") #csvλ‘ λ³κ²½ν¨
        break
    if answer_state in data_state :
	# μ μ κ° μμ±ν answer state κ° data state μ μμΌλ©΄ κ·Έμλ¦¬μκ°μ write μ°κΈ°		    
        states_list.append(answer_state)
        t = turtle.Turtle()
        t.hideturtle()
        t.penup()
        position = data[data.state == answer_state]   # answer_state μ date μ state μ΄μ κ°μ΄ κ°μ -> position μΌλ‘ μ§μ 
        t.goto(int(position.x), int(position.y)) # position μ x μ΄ yμ΄λ‘ κ°μ
        t.write(answer_state) #wirte λ₯Ό 




```
