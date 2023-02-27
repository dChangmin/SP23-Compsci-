# Daniel Lee's Compsci for Designers and Artists
for SP23 Compsci for Designers and Artists

Midterm quiz submission

import js
p5 = js.window

random_size = p5.random(25,125)
random_square(random_size)



def setup():
    p5.createCanvas(300, 300)    # 300 x 300 pixel canvas 
    print('finished setup')
   



def draw():
    p5.background(255)           # white background
    p5.text(str(p5.mouseX) + ", " + str(p5.mouseY), 10, 15)
    p5.strokeWeight(2)  # set stroke thickness
    p5.text(random_size, 10, 30)

    p5.line(50, 50, 50 + random_size, 50)
    p5.line(50 + random_size, 50, 50 + random_size, 50 + random_size)
    p5.line(50 + random_size, 50 + random_size, 50, 50 + random_size)
    p5.line(50, 50 + random_size, 50, 50)
