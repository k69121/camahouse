# camahouse

##code
```
import turtle
import random

mypen = turtle.Turtle()
mypen.penup()
mypen.setposition(-300, 300)
mypen.pendown()
mypen.pensize(3)

for x in range(4):
    mypen.forward(600)
    mypen.right(90)

mypen.hideturtle()

t1 = turtle.Turtle()
t1.shape("turtle")
t1.color("red")
t1.up()

t2 = turtle.Turtle()
t2.shape("turtle")
t2.color("green")
t2.up()

t3 = turtle.Turtle()
t3.shape("turtle")
t3.up()

while True:
    for i in range(100):
        length = random.randint(1,100)
        t1.forward(length)
        t2.forward(length)
        t3.forward(length)

        if t1.xcor() > 300 or t1.xcor() < -300 or t1.ycor() > 300 or t1.ycor() < -300:
            t1.right(180)
            t1.forward(length)
        if t2.xcor() > 300 or t2.xcor() < -300 or t2.ycor() > 300 or t2.ycor() < -300:
            t2.right(180)
            t2.forward(length)
        if t3.xcor() > 300 or t3.xcor() < -300 or t3.ycor() > 300 or t3.ycor() < -300:
            t3.right(180)
            t3.forward(length)

        angle = random.randint(-180, 180)
        t1.right(angle)

        a = random.randint(-180, 180)
        if a != angle:
            t2.right(a)
        if a == angle:
            t2.right(180)

        b = random.randint(-180, 180)
        if b != angle or b != a:
            t3.right(b)
        if b == angle and b == a:
            t3.right(180)
```
*italics*
**bold**
