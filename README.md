# Task 1:- Change the position of the player.
# Refer the line number 175.

import turtle as t

# Background and field setup
t.speed(0)
t.up()
t.backward(450)
t.down()

# Sky (Blue Rectangle)
t.begin_fill()
t.color('sky blue')
for i in range(2):
    t.forward(800)
    t.left(90)
    t.forward(250)
    t.left(90)
t.end_fill()

t.up()
t.right(90)
t.forward(350)
t.left(90)
t.down()

# Grass (Green Rectangle)
t.begin_fill()
t.color('green')
for i in range(2):
    t.forward(800)
    t.left(90)
    t.forward(400)
    t.left(90)
t.end_fill()

#Border of the goal post
t.color('white')
t.up()
t.forward(200)
t.left(90)
t.forward(400)
t.right(90)
t.down()
t.width(5)
for i in range(2):
    t.forward(400)
    t.right(90)
    t.forward(100)
    t.right(90)

# Grid Lines for the Goal Post
for i in range(13):
    t.color('white')
    t.up()
    t.forward(15)
    t.width(1)
    t.right(90)
    t.down()
    t.forward(100)
    t.up()
    t.left(90)
    t.forward(15)
    t.down()
    t.left(90)
    t.forward(100)
    t.right(90)

t.up()
t.forward(10)
t.right(90)
t.forward(15)
t.down()

for i in range(5):
    t.right(90)
    t.forward(400)
    t.up()
    t.left(90)
    t.forward(15)
    t.left(90)
    t.down()
    t.forward(400)
    t.right(90)

t.up()
t.forward(12)
t.right(90)
t.forward(200)
t.left(90)
t.forward(200)
t.left(90)
t.backward(400)
t.down()

# Center Circle (White Circle)
t.forward(800)
t.up()
t.backward(400)
t.left(90)
t.forward(50)
t.right(90)
t.down()
t.circle(-50)

# Soccer Ball (Black and White Circle)
t.up()
t.right(90)
t.forward(50)
t.left(90)
t.forward(200)
t.left(90)
t.forward(100)
t.down()
t.begin_fill()
t.color('black','white')
t.circle(20)
t.end_fill()

t.up()
t.left(90)
t.forward(10)
t.down()

# 1st black dot of football
t.begin_fill()
t.color('black')
t.circle(5)
t.end_fill()

t.up()
t.forward(20)
t.right(90)
t.down()

# 2nd black dot of football
t.begin_fill()
t.color('black')
t.circle(5)
t.end_fill()


t.up()
t.forward(15)
t.right(90)
t.forward(15)
t.down()

# 3rd black dot of football
t.begin_fill()
t.color('black')
t.circle(-5)
t.end_fill()

#Drawing red flag
t.up()
t.forward(170)
t.right(90)
t.forward(115)
t.down()
t.backward(70)
t.begin_fill()
t.color('red')
for i in range(3):
    t.forward(30)
    t.left(120)
t.end_fill()

# Custom Player Shape (GIF Image)
t.register_shape("player.gif")
player = t.Turtle()
player.up()
#to change the player x y position
player.goto(100,-60)
player.down()
player.shape("player.gif")

t.done()




















