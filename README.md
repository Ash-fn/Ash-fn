import  turtle

screen  = turtle.screen()
screen.bgcolor("lightblue")
screen.title("Happy Birthday Card")

cake = turtle.Turtle()
cake.speed(2)

def draw_rectangle(turtle,  widht,  height, color)turtle.begin_fill()
  turtle.color(color)
  for _ in range(2)
      turtle.forward(width)
      turtle.left(90)
      turtle.forward(height)
      turtle.left(90)
  turtle.end_fill()
  
  cake.penup()
  cake.goto(-50,  -100)
  cake.pendown()
  draw_rectangle( cake, 100,  50, "pink" )
  
  cake.penup()
  cake.goto( -40, -50)
  cake.pendown()
  draw_rectangle( cake, 80, 40, "yellow"  )
  
  cake.penup()
  caje.goto(  -30,  -10)
  cake.pendown()
  draw_rectangle( cake, 60, 30, "blue"  )
  
  candles = turtle.Turtle()
  candles.spees(3)

def draw_candle(turtle, x,  y):
    turtle.penup()
    turtle.goto(x,  y)
    turtle.pendown()
    turtle.color("white")
    turtle.begin_fill()
    turtle.forward(10)
    turtle.left(90)
    turtle.forward(20)
    turtle.left(90)
    turtle.forward(10)
    turtle.left(90)
    turtle.forward(20)
    turtle.left(90)
    turtle.end_fill()
    
    # Draw the flame
    turtle.penup()
    turtle.goto(x + 5,  y + 20)
    turtle.pendown()
    turtle.color("orange")
    turtle.begin_fill()
    turtle.circle(5)
    turtle.end_fill()
    
for i in range(3):
    draw_candle(candles,  -20 + i * 20, 30)
    
cake.hideturtle()
candle.hideturtle()

text  = turtle.Turtle()
text.penup()
text.goto(0,  -300)
text.color("red")
text.write("Happy Birthday!", font=("Arial",  24, "bold"))
text.goto(0,  -430)
text.write("Fania", align="center", font=("Arial", 20, "bold"))
turtle.hideturtle()

turtle.done()