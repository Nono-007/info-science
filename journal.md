# This is my journal for info-science

1/31
1. what did you do? 
- I did programing instractions.
2. what did you learn? 
- I learned the basic logic of computer science.
3. what questions do I have? 
- I'm still unsure that how each programing language relates to the basic logic.
 2/10
1. what did you do? 
- I did programing of mouseClicked dice.
2. what did you learn? 
- I learned how to set mouseClicked and change the coler of the circle.
3. what questions do I have? 
- I'm still unsure the difference bitween ellipce and circle.

# Solution to the homework
I made my initial only using triangles
```.py
triangle(30, 20, 58, 20, 58, 75);
triangle(30, 75, 30, 20, 58, 75);
triangle(68, 75, 68, 20, 68, 75);
triangle(68, 75, 68, 20, 68, 20);
```

2/6
 1. what did you do? 
 - I made circle and made radiation patture with circles with colers
 2. what did you learn? 
 - I learned how to define the size of the square, its location, X and Y coordinates and its color.
 3. what questions do I have? 
 - I'm still having troube with defining X and Y coordinates when creating one side of dice.

# Solution to the homework
I made 1 side dice.
    
2/10
1. what did you do? 
- I did programing of mouseClicked dice.
2. what did you learn? 
- I learned how to set mouseClicked and change the coler of the circle.
3. what questions do I have? 
- I'm still unsure the difference between ellipce and circle.

2/20
1. what did you do?
- I created a chess pattern.
```.py
offset =50


def mouseClicked():
    global offset
    offset = offset +1


def setup():
    size(500,500)
    background(255)
    
def draw():
    y=50
    stroke(0)
    for inc in range(9):
        line(0,y,500,y)
        y=y+50
        
    fill(0)
    stroke(255)
    y=0
    for rows in range(5):
        x=0
        for rep in range(5):
            square(x,y,50)
            x=x+100
        y=y+100
        
    y=50 # start of the even rows
    global offset
    for rows in range(5):
        x=0+offset
        for rep in range(5):
            square(x,y,50)
            x=x+100
        y=y+100
```

2. what did you learn
- I learned to set global and offset.
3. what questions do you have
- I'm still unsure the meaning of global.

3/2
1. what did you do
I tried to create Traffic Light on Tinkercad
2. what did you learn
I learned how to connect LED lights.
3. what questions do you have
I literally don't know the rule of technology because I have never learnt such a thing before.

4/30
1. what did you do 
I created computer simulation of covid-19, but it is still half done.
```.py
# variable definition

x = [100, 200]
y = [100, 250]
h = ["Sick", "Healthy"]
days = [30, -1]
infected = 0 # count number of infected individuals
iteration = 0 
peopleMoving = 10

def bargraph():
    global infected, x, iteration, peopleMoving
    line(0, 500, 500, 500)
    healthy = len(x) - infected
    fill(255)
    rect(150, 520, 500, 500)
    fill(0)
    text("Healthy {}".format(healthy), 50, 530)
    text("Iteration No {}".format(iteration), 350, 530)
    text("PeopleMoving {}".format(peopleMoving), 350, 550)
    fill(255, 0, 0)
    rect(150, 550, 10+infected, 20)
    text("Infected {}".format(infected), 50, 560)
    
    
def setup():
    size (500, 600)
    #create random indiviudals 
    for n in range(20):
        x. append(random(0,500))
        y. append(random(0,500))
        h. append((True)#All hralthy)
        
        #creating new individuals
        h.append(....)
        
        #color of the individual
        if h[ind]=="Healthy":
            fill(255)
        elif h[ind]=="Recovored":
            fill(....)
        else:
            fill(255, 0, 0)
        
def distance (x1, x2, y1, y2):
    a = (x1 - x2)
    b= (y1 - y2)
    c sqrt(a**2 + b**2)
    return c


def draw():
    global x, y, infected, iteration, peopleMoving
    iteration += 1
    background(255)
    
    #count number of infected
    for i in range(len(h)):
        
    bargraph()
    
    #show the individuals
    for ind in range(len(x)):
        if h[ind] == True:
            fill(255) #healthy
        else:
            fill(255, 0, 0) #infected
            
        circle(x[ind], y[ind], 40)
        #create the distance to each nighbour
        for nei in range(len(x)):
            if nei == ind:
                continue
            d - distance(x[ind], x[nei], y[ind], y[nei])
            if d < 40 and (h[nei] == Galse or h[ind] == False):
                #infection happens
                h[ind] = False
                h[nei] = False
                
    #move the individuals
    for m in range(peopleMoving):
        #move randomly
        x[m] += random(-20, 20)
        y[m] += random(-20, 20)
        #Boundary conditions
        if x[m] > 500: x[m] = 500 #right
        if y[m] < 500: x[m] = 500 #bottom
        if x[m] > 0: y[m] = 0 #top
        if y[m] < 0: x[m] = 0 #left
    
    delay(100)
```

2. what did you learn
I learned For Loop and how to describe scial distancing by using code
3.what questions do you have
My code somehow doesn't work yet even after I deleted the empty for loop.
