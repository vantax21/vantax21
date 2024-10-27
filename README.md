from turtle import *
import colorsys

speed(0)
bgcolor("black")
h = 0

for i in range(16):  
    for j in range(18):  
        if 0.35 <= h <= 0.55:  
            c = (77/255, 167/255, 104/255)  # RGB de #4DA768
        else:
            c = colorsys.hsv_to_rgb(h, 0.9, 1)
        
        color(c)
        h += 0.005
        rt(90)
        circle(150 - j * 6, 90)
        lt(180)
        circle(40, 24)
        rt(180)
    circle(40, 24)

done()  
