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
3. what questions do I have
- I'm still unsure the meaning of global.
