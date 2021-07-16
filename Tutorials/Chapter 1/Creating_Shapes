#GlowScript 3.1 VPython
'''
https://physics.weber.edu/schroeder/scicomp/PythonManual.pdf
Chapter 1 
'''


'''box()
#creates an opaque box'''
'''box(pos=vector(1,0,0), size=vector(.5,.3,.2), color=color.red)'''
#creating sphere
'''sphere(radius=0.25)'''
#creating a cylinder
'''cylinder(axis=vector(0,1.5,0))'''


'''
Problem 1
It would be helpful if your 3D space had some coordinate axes, right?
So create some now, in the form of very skinny cylinders running from −5 to 5 in
each of the three dimensions.'''
'''
cylinder(pos=vector(-5,0,0),size=vector(10,0.1,0.1),color = color.red)
cylinder(pos=vector(0,0,0),size=vector(0.1,10,0.1),color = color.blue)
cylinder(pos=vector(0,0,0),size=vector(0.1,0.1,10),color = color.yellow)
'''


#Naming Varriables
'''obj can be named
x_axis = cylinder(pos=vector(-5,0,0),size=vector(10,0.1,0.1),color = color.red)
'''
'''colour=xaxis.color'''


'''
Problem 2
Create dumble with sphere of 3r
'''
'''
#to change bg
scene.background = color.white

rod = cylinder(pos=vector(-5,0,0),length = 10,radius = 0.5,color = color.red)

sphere(pos = rod.pos,radius=3*rod.radius,color = color.blue)
sphere(pos = rod.pos + vector(10,0,0),radius=3*rod.radius,color=color.green)
'''


#Animation
'''
cylinder(pos=vector(-5,0,0),size=vector(10,0.1,0.1),color = color.red)
cylinder(pos=vector(0,0,0),size=vector(0.1,10,0.1),color = color.blue)
cylinder(pos=vector(0,0,0),size=vector(0.1,0.1,10),color = color.yellow)
movingBox = box(pos=vector(0,0,0), size=vector(.2,.2,.2), color=color.red)
while movingBox.pos.x < 5:
    rate(10)
    movingBox.pos.x += 0.05
    movingBox.pos.y += 0.05
'''


'''
Problem 3
Add code to your program to create a small sphere and then move
that sphere at a steady speed once around a circle in the xy plane, centered at the
origin. Use a variable called theta for the angle around the circle, and set this
variable equal to zero before your while loop begins. Also use a variable called r
for the circle’s radius, and x and y for its rectangular coordinates. To calculate x
and y you can use the built-in trigonometric functions cos and sin, for example,
x = r * cos(theta). Be careful, though, because the trig functions assume that
the parameter you pass to them is in radians; keep this in mind when deciding how
much to change theta during each loop iteration, and in deciding what conditions
to use in the while statement. To actually move the sphere in the graphics scene,
use an instruction of the form movingSphere.pos = vector(x, y, 0).
'''

sun = sphere(pos = vector(0,0,0), radius = 1,color=color.orange)
earth = sphere(pos = vector(0,0,5), radius = 0.5,color=color.blue)
theta = 0
while theta <20:
    rate(20)
    earth.pos.z = 5*cos(theta)
    earth.pos.x = 5*sin(theta)
    theta +=0.1


#Graphs
'''
graph(width=400, height=250)
xDots = gdots(color=color.green)#to give green dot
yDots = gdots(color=color.magenta)to give magenta dots
x=2
xDots.plot(x**2,x)
'''
