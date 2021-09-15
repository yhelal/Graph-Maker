import sys
import turtle
import math
import random
t=turtle.Turtle()

def build_axis(a,b,c): # a is x scale b is y scale and c is intervals
    t.penup()
    t.goto(-a,0)
    t.pendown()
    t.fd(a*2)
    t.goto(0,0)
    t.lt(90)
    t.fd(b)
    t.bk(b*2)
    t.penup()
    t.goto(-a,0)
    t.pendown()
    x=-a
    rx=int((a*2)/c)
    for _ in range (0,rx+1):
        t.goto(x,0)
        lines()
        axes_text(str(x))
        x+=c
    t.penup()
    t.goto(0,-b)
    t.rt(90)
    y=-b
    t.pendown()
    ry=int((b*2)/c)
    for _ in range (0,ry+1):
        t.goto(0,y)
        lines()
        axes_text(y)
        y+=c
        

def lines():
    t.fd(5)
    t.bk(10)
    t.fd(5)

    
def axes_text(x):
    if(x!=0):
        t.penup()
        t.bk(17)
        t.write(x,font=('Arial',8,'normal'))
        t.fd(17)
        t.pendown()
    

def axes_eq(x,n):
    t.penup()
    t.goto(-300,-((n*25)+100))
    t.write(x,font=('Arial',10,'normal'))

def plot_line(eq,n,end,a):
    t.penup()
    t.goto(-a,0)
    t.pendown()
    t.pencolor(random.uniform(0,1),random.uniform(0,1),random.uniform(0,1))
    for x in range (-a,a):
        if(x==-a):
            t.penup()
        else:
            t.pendown()
        y=eval(eq)
        t.goto(x,y)
    axes_eq(eq,n)
    if(n==end-1):
        turtle.done()
    
def input_formulae():
    f=turtle.textinput('Graph Creator', 'Please enter the desired formula in terms of x')
    return f
def input_scale():
    sx=turtle.textinput('Graph Creator', 'Please Enter the Desired Limit for the x-axis')
    sy=turtle.textinput('Graph Creator', 'Please Enter the Desired Limit for the y-axis')
    sintv=turtle.textinput('Graph Creator', 'Please Enter the Desired Interval for Scaling')
    return (sx,sy,sintv)
    
#build_axis(200,200,50)        
#plot_line('100*math.cos(x/100)',1,2,200)  

#f=input_formulae()
#plot_line(f,1,2,200)


