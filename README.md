# random.star


import turtle
import time
import random

t = turtle.Turtle()
s = turtle.Screen()
t.hideturtle()
s.title("Night Sky")
s.screensize(800, 500,  bg='black')
t.pencolor("Red")
time.sleep(1)

def start():
   for i in range(5):
       t.pendown()
       time.sleep(0)
       t.forward(10)
       t.right(145)


s.colormode(255)
while True:
    x = random.randint(-400, 250)
    y = random.randint(-400, 250)
    r = random.randint(0, 255)
    b = random.randint(0, 255)
    g = random.randint(0, 255)
    t.pencolor(r, b, g)
    t.penup()
    t.goto(x, y)
    start()


turtle.done()
