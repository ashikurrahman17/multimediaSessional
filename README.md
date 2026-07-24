# 🎨 ANIMATION AND INTERACTIVE SYSTEMS Codebook using p5.js

<p align="center">
<img src="https://p5js.org/assets/img/p5js.svg" width="180">
</p>

<p align="center">
A complete practical guide for ANIMATION AND INTERACTIVE SYSTEMS using <b>p5.js</b>.
</p>

---

# Introduction

This repository contains the complete solutions of ANIMATION AND INTERACTIVE SYSTEMS Laboratory exercises using **p5.js**, a JavaScript library developed to make creative coding and graphics programming easier.

The code examples are beginner-friendly and demonstrate important graphics concepts such as

- Drawing
- Coloring
- Animation
- Transformations
- Interactivity
- Physics
- Sound
- Simple Game Development

Every program includes

- Objective
- Algorithm
- Source Code
- Explanation
- Expected Output
- Important Functions

---

# 📑 Index

## 🎨 Part 1 — Basic Drawing and Colors
- [Problem 1 – Basic Geometric Shapes and Colors](#problem-1)
- [Problem 2 – Simple Graphical Scene](#problem-2)
- [Problem 3 – Mouse Coordinates Display](#problem-3)

---

## 🎞 Part 2 — Basic Animation
- [Problem 4 – Moving Shapes](#problem-4)
- [Problem 5 – Bouncing Ball](#problem-5)
- [Problem 6 – Size and Color Animation](#problem-6)
- [Problem 7 – Multiple Moving Objects](#problem-7)

---

## 🔄 Part 3 — Transformations
- [Problem 8 – Translation](#problem-8)
- [Problem 9 – Rotation](#problem-9)
- [Problem 10 – Scaling](#problem-10)
- [Problem 11 – Combined Transformations](#problem-11)
- [Problem 12 – Interactive Transformations](#problem-12)

---

## 🖱 Part 4 — Interactivity
- [Problem 13 – Mouse Following Shapes](#problem-13)
- [Problem 14 – Mouse Click Effects](#problem-14)
- [Problem 15 – Keyboard Controlled Movement](#problem-15)
- [Problem 16 – Slider and Button Controls](#problem-16)

---

## ✨ Part 5 — Visual Effects and Physics
- [Problem 17 – Particle System](#problem-17)
- [Problem 18 – Glow and Pulsing Effect](#problem-18)
- [Problem 19 – Gravity Simulation](#problem-19)
- [Problem 20 – Bouncing Ball with Friction](#problem-20)
- [Problem 21 – Explosion Effect](#problem-21)

---

## 🎵 Part 6 — Sound and Audio
- [Problem 22 – Keyboard Sound](#problem-22)
- [Problem 23 – Audio Reactive Visualization](#problem-23)
- [Problem 24 – Animation Based on Sound](#problem-24)

---

## 🎮 Part 7 — Game Development
- [Problem 25 – Catch the Object Game](#problem-25)
- [Problem 26 – Pong Game](#problem-26)
- [Problem 27 – Shooting Game](#problem-27)

---

# What is p5.js?

**p5.js** is an open-source JavaScript library designed for visual programming.

It simplifies graphics programming by providing built-in functions for drawing shapes, animations, interactions, sound processing, and multimedia applications.

Official Website

https://p5js.org

Online Editor

https://editor.p5js.org

---

# How to Run a p5.js Program

### Method 1 (Recommended)

Open

https://editor.p5js.org

Create a new sketch.

Write the code.

Click ▶ Run.

---

### Method 2

Download

- p5.js library
- VS Code

Create

```
index.html
sketch.js
```

Link p5.js inside HTML.

Run the HTML file.

---

# Basic Structure of a p5.js Program

```javascript
function setup(){

    createCanvas(700,400);

}

function draw(){

    background(220);

}
```

---

# Understanding setup()

`setup()` executes only one time.

Usually used for

- Creating canvas
- Loading variables
- Setting colors
- Initializing objects

Example

```javascript
function setup(){

    createCanvas(600,400);

}
```

---

# Understanding draw()

`draw()` runs approximately **60 times per second**.

Anything written inside draw() keeps updating continuously.

Example

```javascript
function draw(){

    background(220);

    circle(100,100,50);

}
```

---

# Frequently Used Functions

| Function | Description |
|-----------|-------------|
| createCanvas() | Create drawing area |
| background() | Set background color |
| fill() | Fill color |
| stroke() | Border color |
| strokeWeight() | Border thickness |
| noStroke() | Remove border |
| circle() | Draw circle |
| ellipse() | Draw ellipse |
| rect() | Draw rectangle |
| square() | Draw square |
| triangle() | Draw triangle |
| line() | Draw line |
| point() | Draw point |
| arc() | Draw arc |
| text() | Display text |
| textSize() | Change font size |
| random() | Generate random number |
| map() | Convert one range into another |
| dist() | Calculate distance |
| mouseX | Mouse X position |
| mouseY | Mouse Y position |
| frameCount | Current animation frame |

---

# RGB Color System

Every color consists of three components.

```
Red
Green
Blue
```

Each value ranges from

```
0 → 255
```

Examples

```javascript
fill(255,0,0);
```

Red

```javascript
fill(0,255,0);
```

Green

```javascript
fill(0,0,255);
```

Blue

```javascript
fill(255,255,0);
```

Yellow

```javascript
fill(255);
```

White

```javascript
fill(0);
```

Black

---

# Coding Guidelines

✔ Use meaningful variable names.

✔ Keep indentation consistent.

✔ Comment important code.

✔ Use push() and pop() whenever transformations are used.

✔ Use background() inside draw() for animation.

✔ Use constrain() to keep objects inside canvas.

✔ Use random() whenever random colors or positions are needed.

---

# Problem 1
## Basic Drawing and Colors

### Objective

Draw

- Line
- Rectangle
- Circle
- Triangle

using RGB colors and randomly generated colors.

---

## Algorithm

Step 1

Create canvas.

Step 2

Draw line.

Step 3

Draw rectangle.

Step 4

Draw circle.

Step 5

Draw triangle.

Step 6

Use RGB colors.

Step 7

Use random colors.

---

## Source Code

```javascript
function setup(){

    createCanvas(700,400);

    background(220);

    strokeWeight(3);

    line(50,60,200,100);

    fill(255,0,0);

    rect(60,150,120,80);

    fill(0,255,0);

    circle(300,190,100);

    fill(random(255),random(255),random(255));

    triangle(500,250,450,100,600,100);

    fill(random(255),random(255),random(255));

    circle(300,60,60);

}
```

---

## Explanation

```
createCanvas()

creates the drawing window.
```

```
background()

changes background color.
```

```
line()

draws a straight line.
```

```
rect()

draws rectangle.
```

```
circle()

draws circle.
```

```
triangle()

draws triangle.
```

```
random()

creates random color every execution.
```

---

## Output

```
✓ Line

✓ Rectangle

✓ Circle

✓ Triangle

✓ RGB Colors

✓ Random Colors
```

---

# Problem 2
## Simple Graphical Scene

### Objective

Draw a beautiful scenery using multiple shapes.

---

## Algorithm

1. Draw sky.

2. Draw sun.

3. Draw grass.

4. Draw house.

5. Draw roof.

6. Draw windows.

7. Draw tree.

---

## Source Code

```javascript
function setup(){

createCanvas(700,500);

background(135,206,235);

fill(255,204,0);
circle(80,80,80);

fill(34,139,34);
rect(0,350,width,150);

fill(210,180,140);
rect(250,180,200,170);

fill(165,42,42);
triangle(230,180,470,180,350,90);

fill(101,67,33);
rect(330,260,45,90);

fill(173,216,230);
rect(275,220,40,40);

rect(390,220,40,40);

fill(139,69,19);
rect(100,240,25,110);

fill(0,155,0);
circle(112,210,90);

}
```

---

## Concepts Learned

- Background
- Shapes
- Positioning
- Colors
- Scene Composition

---

# Problem 3
## Mouse Coordinates

### Objective

Display current mouse position.

---

## Algorithm

1. Draw shapes.

2. Read mouseX.

3. Read mouseY.

4. Display using text().

---

## Source Code

```javascript
function setup(){

createCanvas(700,400);

}

function draw(){

background(240);

fill(255,0,0);

rect(80,100,120,80);

fill(0,0,255);

circle(350,170,100);

fill(0,255,0);

triangle(500,250,620,250,560,120);

line(50,350,650,350);

fill(0);

textSize(20);

text("Mouse X : "+mouseX,20,30);

text("Mouse Y : "+mouseY,20,60);

}
```

---

## Important Variables

```
mouseX

Current X position of mouse.
```

```
mouseY

Current Y position of mouse.
```

---

# Problem 4
## Basic Animation

### Objective

Move a circle continuously across the screen.

---

## Algorithm

1. Create variable x.

2. Draw circle.

3. Increase x every frame.

4. Reset after leaving canvas.

---

## Source Code

```javascript
let x=0;

function setup(){

createCanvas(700,400);

}

function draw(){

background(220);

fill(0,150,255);

circle(x,200,60);

x+=3;

if(x>width+30){

x=-30;

}

}
```

---

## Concepts Learned

- Animation
- Variables
- draw()
- Continuous Motion
- Updating Position

---

# Summary of Part 1

After completing this section, you should understand:

- ✔ Canvas Creation
- ✔ Basic Shapes
- ✔ RGB Colors
- ✔ Random Colors
- ✔ Mouse Coordinates
- ✔ Scene Drawing
- ✔ Continuous Animation

---

**Next:** Part 2 covers **Problems 5–8**, including:
- Bouncing Ball Physics
- Changing Size & Color Animation
- Multiple Moving Objects
- Translation Transformation

- 
# Part 2A — Basic Animation (Problems 05–06)

---

# Problem 5
# Bouncing Ball Animation

## Objective

Create a ball that moves inside the canvas and bounces whenever it touches any boundary.

This experiment introduces the basic concepts of **velocity**, **collision detection**, and **animation**.

---

## Theory

Animation is created by repeatedly updating the position of an object.

A bouncing ball has two velocity components:

- Horizontal Velocity (`dx`)
- Vertical Velocity (`dy`)

Every frame,

```
x = x + dx
y = y + dy
```

When the ball reaches a wall, its direction is reversed.

```
dx = -dx
```

or

```
dy = -dy
```

---

## Algorithm

Step 1

Create the canvas.

Step 2

Initialize the ball position.

Step 3

Initialize horizontal and vertical speed.

Step 4

Draw the ball.

Step 5

Update its position every frame.

Step 6

Check collision with left and right walls.

Step 7

Reverse horizontal velocity.

Step 8

Check collision with top and bottom walls.

Step 9

Reverse vertical velocity.

---

## Source Code

```javascript
let x = 100;
let y = 100;

let dx = 4;
let dy = 3;

function setup() {

    createCanvas(700,400);

}

function draw() {

    background(240);

    fill(255,120,0);

    circle(x,y,50);

    x += dx;

    y += dy;

    // Left & Right Collision
    if(x > width-25 || x < 25){

        dx = -dx;

    }

    // Top & Bottom Collision
    if(y > height-25 || y < 25){

        dy = -dy;

    }

}
```

---

# Code Explanation

### Ball Position

```javascript
let x = 100;
let y = 100;
```

Stores the current position of the ball.

---

### Ball Speed

```javascript
let dx = 4;
let dy = 3;
```

Ball moves

- 4 pixels horizontally
- 3 pixels vertically

every frame.

---

### Updating Position

```javascript
x += dx;
y += dy;
```

Equivalent to

```javascript
x = x + dx;
y = y + dy;
```

---

### Collision Detection

```javascript
if(x > width-25 || x < 25)
```

Checks

- Right wall
- Left wall

---

### Direction Change

```javascript
dx = -dx;
```

Positive speed becomes negative.

Negative speed becomes positive.

Exactly like reflection.

---

## Output

```
● Ball moves continuously.

● Ball bounces from all four walls.

● Motion never stops.
```

---

## Important Functions

| Function | Purpose |
|----------|----------|
| circle() | Draw ball |
| background() | Clear previous frame |
| width | Canvas width |
| height | Canvas height |

---

## Concepts Learned

✔ Animation

✔ Velocity

✔ Boundary Collision

✔ Reflection

✔ Continuous Motion

---

# Viva Questions

### Q1

Why is draw() used?

Answer

Because draw() executes continuously, making animation possible.

---

### Q2

Why do we reverse velocity?

Answer

To simulate reflection after collision.

---

### Q3

What happens if background() is removed?

Answer

The previous frames remain, producing a trail effect.

---

# Problem 6
# Changing Size and Color Animation

## Objective

Create a circle that continuously changes

- Size
- Color

over time.

---

## Theory

Animation is not limited to movement.

Properties like

- Size
- Color
- Opacity
- Rotation

can also change every frame.

The variable

```
frameCount
```

keeps increasing automatically.

Using

```
sin()
```

and

```
cos()
```

produces smooth periodic motion.

---

## Understanding frameCount

```
Frame 1

Frame 2

Frame 3

...

Frame 500
```

Each frame has a different value.

---

## Understanding sin()

The sine function oscillates between

```
-1

to

+1
```

This produces smooth animation.

Example

```
Size

150

↑

120

↑

90

↑

60

↓

90

↓

120

↓

150
```

---

## Algorithm

Step 1

Create canvas.

Step 2

Create size variable.

Step 3

Increase size.

Step 4

Decrease size after maximum.

Step 5

Use sine and cosine for RGB colors.

Step 6

Draw animated circle.

---

## Source Code

```javascript
let size = 50;

let grow = true;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(220);

    let r = map(
        sin(frameCount*0.05),
        -1,1,
        0,255
    );

    let g = map(
        cos(frameCount*0.05),
        -1,1,
        0,255
    );

    let b = map(
        sin(frameCount*0.03),
        -1,1,
        0,255
    );

    fill(r,g,b);

    noStroke();

    circle(width/2,height/2,size);

    if(grow){

        size++;

    }

    else{

        size--;

    }

    if(size>=150){

        grow=false;

    }

    if(size<=40){

        grow=true;

    }

}
```

---

# Code Explanation

### Size Variable

```javascript
let size = 50;
```

Stores the current diameter.

---

### Growing

```javascript
size++;
```

Diameter increases every frame.

---

### Shrinking

```javascript
size--;
```

Diameter decreases.

---

### RGB Animation

```javascript
fill(r,g,b);
```

Every frame,

the values of

```
r

g

b
```

change smoothly.

---

### map()

```javascript
map(value,-1,1,0,255)
```

Converts

```
-1 → 0

+1 → 255
```

Perfect for RGB values.

---

## Output

```
✓ Circle continuously grows.

✓ Circle continuously shrinks.

✓ Color smoothly changes.

✓ Animation never stops.
```

---

## Frequently Used Functions

| Function | Purpose |
|----------|----------|
| frameCount | Current frame number |
| sin() | Smooth oscillation |
| cos() | Smooth oscillation |
| map() | Convert one range into another |
| fill() | Apply RGB color |

---

## Concepts Learned

✔ Dynamic Animation

✔ RGB Transition

✔ frameCount

✔ Sine Wave

✔ Cosine Wave

✔ Growing and Shrinking Objects

---

# Viva Questions

### Q1

Why is frameCount useful?

Answer

It provides continuously increasing values for animation.

---

### Q2

Why use sin() instead of random()?

Answer

Random values change abruptly.

Sine produces smooth transitions.

---

### Q3

What is the purpose of map()?

Answer

It converts values from one range to another.

Example

```
-1 to 1

↓

0 to 255
```

---

# Common Mistakes

❌ Forgetting to call

```javascript
background();
```

Result

Old frames remain on screen.

---

❌ Using

```javascript
size = size++;
```

Correct

```javascript
size++;
```

---

❌ Forgetting

```javascript
grow = false;
```

The object will only increase forever.

---

❌ Using RGB values larger than 255.

Valid Range

```
0 – 255
```

---

# Summary of Part 2A

After completing this section, you should understand

✔ Ball Physics

✔ Collision Detection

✔ Reflection

✔ Velocity

✔ Dynamic Animation

✔ Changing Colors

✔ frameCount

✔ map()

✔ sin()

✔ cos()

---

## Next Part

**Part 2B** covers:

- **Problem 07:** Multiple Moving Objects with Different Speeds
- **Problem 08:** Translation Transformation (`translate()`, `push()`, `pop()`)

These two introduce object-oriented thinking and the foundation of computer graphics transformations.

# Part 2B — Basic Animation & Transformations (Problems 07–08)

---

# Problem 7
# Multiple Moving Objects

## Objective

Create an animation involving multiple objects moving simultaneously with different speeds and directions.

---

# Theory

In computer graphics, a scene usually contains multiple objects rather than a single object.

Each object should have its own:

- Position
- Speed
- Direction
- Color

Since every object has independent properties, they move independently.

---

## Understanding Multiple Objects

Example

```
Blue Circle

Moves Left → Right

Speed = 3
```

```
Red Rectangle

Moves Top → Bottom

Speed = 2
```

```
Green Ball

Moves Right → Left

Speed = 4
```

Since all objects are updated every frame, they appear to move simultaneously.

---

# Algorithm

Step 1

Create canvas.

Step 2

Initialize the positions of all objects.

Step 3

Draw the first object.

Step 4

Draw the second object.

Step 5

Draw the third object.

Step 6

Update every object's position.

Step 7

Reset object positions when they leave the screen.

---

# Source Code

```javascript
let circleX = 50;

let rectY = 50;

let ballX = 650;
let ballY = 350;

function setup(){

    createCanvas(700,450);

}

function draw(){

    background(230);

    // Blue Circle
    fill(0,100,255);

    circle(circleX,100,50);

    circleX += 3;

    if(circleX > width+25){

        circleX = -25;

    }

    // Red Rectangle

    fill(255,0,0);

    rect(300,rectY,80,50);

    rectY += 2;

    if(rectY > height){

        rectY = -50;

    }

    // Green Ball

    fill(0,180,0);

    circle(ballX,ballY,40);

    ballX -= 4;

    ballY -= 2;

    if(ballX < -20){

        ballX = width+20;

    }

    if(ballY < -20){

        ballY = height+20;

    }

}
```

---

# Code Explanation

### Blue Circle

Moves horizontally.

```javascript
circleX += 3;
```

---

### Red Rectangle

Moves vertically.

```javascript
rectY += 2;
```

---

### Green Ball

Moves diagonally.

```javascript
ballX -= 4;

ballY -= 2;
```

---

### Reset Position

Instead of bouncing,

the objects restart from the opposite side.

Example

```javascript
if(circleX > width){

circleX = 0;

}
```

---

# Output

```
Blue Circle

↓

Moves Left → Right

--------------------

Red Rectangle

↓

Moves Top → Bottom

--------------------

Green Ball

↓

Moves Diagonally
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| circle() | Draw circle |
| rect() | Draw rectangle |
| background() | Clear previous frame |
| width | Canvas width |
| height | Canvas height |

---

# Concepts Learned

✔ Multiple Objects

✔ Independent Motion

✔ Animation Loop

✔ Different Speeds

✔ Screen Wrapping

---

# Viva Questions

### Q1

Can multiple objects have different speeds?

Answer

Yes.

Every object has its own velocity.

---

### Q2

Why do we use different variables?

Answer

Each object must store its own position.

---

### Q3

Can one object move diagonally?

Answer

Yes.

Update both X and Y coordinates.

---

# Problem 8
# Translation Transformation

## Objective

Demonstrate translation by moving a rectangle using the `translate()` function.

---

# Theory

A **Transformation** changes the position, size, or orientation of an object.

There are three basic transformations:

- Translation
- Rotation
- Scaling

Translation simply moves an object from one location to another.

---

## Mathematical Formula

```
New X = Old X + Tx

New Y = Old Y + Ty
```

Where

```
Tx

=

Translation along X-axis
```

```
Ty

=

Translation along Y-axis
```

---

# Understanding translate()

Without translation

```
Rectangle

↓

Drawn at

(0,0)
```

With translation

```javascript
translate(200,100);
```

Now

```
(0,0)

becomes

(200,100)
```

Everything drawn afterward uses the new origin.

---

# Why Use push() and pop()?

Suppose we write

```javascript
translate(200,100);

rect(0,0,100,60);

circle(0,0,40);
```

Both shapes move because the coordinate system has changed.

Sometimes we want only one object to be translated.

Therefore we write

```javascript
push();

translate(...);

draw object;

pop();
```

After `pop()`, the coordinate system returns to normal.

---

# Algorithm

Step 1

Create canvas.

Step 2

Create translation variable.

Step 3

Translate coordinate system.

Step 4

Draw rectangle.

Step 5

Restore original coordinate system.

Step 6

Increase translation value.

---

# Source Code

```javascript
let x = 0;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(220);

    push();

    translate(x,200);

    fill(0,150,255);

    rect(0,0,100,60);

    pop();

    x += 2;

    if(x > width){

        x = -100;

    }

}
```

---

# Code Explanation

### Translation Variable

```javascript
let x = 0;
```

Stores the horizontal translation.

---

### push()

```javascript
push();
```

Saves the current coordinate system.

---

### translate()

```javascript
translate(x,200);
```

Moves the origin to

```
(x,200)
```

---

### Draw Rectangle

```javascript
rect(0,0,100,60);
```

Although drawn at `(0,0)`, it actually appears at the translated position.

---

### pop()

```javascript
pop();
```

Restores the original coordinate system.

---

### Update Translation

```javascript
x += 2;
```

Rectangle moves every frame.

---

# Visual Representation

Before Translation

```
Origin

(0,0)

□
```

After Translation

```
translate(300,200)

                □

Origin moved
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| translate() | Move coordinate system |
| push() | Save transformation state |
| pop() | Restore transformation state |
| rect() | Draw rectangle |

---

# Concepts Learned

✔ Coordinate System

✔ Translation

✔ Animation

✔ Transformation

✔ push()

✔ pop()

---

# Viva Questions

### Q1

Does `translate()` move the object?

Answer

No.

It moves the coordinate system, and the object is drawn relative to the new origin.

---

### Q2

Why use `push()` and `pop()`?

Answer

They prevent transformations from affecting other objects.

---

### Q3

Can translation be applied to any shape?

Answer

Yes.

It works with all drawing functions such as:

- `circle()`
- `rect()`
- `triangle()`
- `line()`
- `ellipse()`

---

# Common Mistakes

❌ Forgetting `pop()`

Result:

Every shape drawn afterward is translated.

---

❌ Calling `translate()` after drawing the shape

Incorrect

```javascript
rect(0,0,100,60);

translate(200,100);
```

Correct

```javascript
translate(200,100);

rect(0,0,100,60);
```

---

❌ Forgetting to update the translation variable

```javascript
x += 2;
```

Without this, the rectangle remains stationary.

---

# Summary of Part 2B

After completing this section, you should understand:

✔ Multiple Object Animation

✔ Independent Speeds

✔ Different Directions

✔ Translation Transformation

✔ Coordinate Systems

✔ `translate()`

✔ `push()` and `pop()`

✔ Screen Wrapping

---

# Next Part

**Part 3** covers **Problems 09–12**:

- Rotation Transformation
- Scaling Transformation
- Combined Transformations
- Interactive Transformations (Keyboard & Mouse)

These topics introduce the core transformation techniques used in modern computer graphics and game development.

# Part 3A — Transformations (Problems 09–10)

---

# Problem 9
# Rotation Transformation

## Objective

Create a program that continuously rotates a square around its center.

This experiment demonstrates the **rotation transformation** using the `rotate()` function.

---

# Theory

Rotation is one of the three fundamental geometric transformations.

It changes the orientation of an object while keeping its shape and size unchanged.

The three basic transformations are:

- Translation
- Rotation
- Scaling

Unlike translation, rotation occurs around a **pivot point (origin)**.

---

# Rotation Formula

For a point **(x, y)** rotated by angle **θ**:

```
x' = x cosθ − y sinθ

y' = x sinθ + y cosθ
```

Fortunately, p5.js performs these calculations automatically using `rotate()`.

---

# Understanding rotate()

The `rotate()` function rotates the **entire coordinate system**, not just one object.

Example

```javascript
rotate(PI/4);
```

Rotates the coordinate system by **45°**.

---

# Why use translate()?

By default, rotation happens around the origin `(0,0)`.

If we rotate without translating,

```
□

rotates around

top-left corner
```

Instead,

```javascript
translate(width/2,height/2);
```

moves the origin to the center of the canvas.

Now rotation looks natural.

---

# Why rectMode(CENTER)?

Normally,

```javascript
rect(x,y,w,h)
```

uses the top-left corner.

During rotation this looks awkward.

Instead,

```javascript
rectMode(CENTER);
```

makes the rectangle rotate around its own center.

---

# Algorithm

Step 1

Create canvas.

Step 2

Set rectangle mode to CENTER.

Step 3

Translate origin to center.

Step 4

Rotate coordinate system.

Step 5

Draw rectangle.

Step 6

Increase angle every frame.

---

# Source Code

```javascript
let angle = 0;

function setup(){

    createCanvas(700,400);

    rectMode(CENTER);

}

function draw(){

    background(240);

    push();

    translate(width/2,height/2);

    rotate(angle);

    fill(255,120,120);

    rect(0,0,120,120);

    pop();

    angle += 0.03;

}
```

---

# Code Explanation

### Angle Variable

```javascript
let angle = 0;
```

Stores the current rotation angle.

---

### Translate

```javascript
translate(width/2,height/2);
```

Moves the origin to the center of the canvas.

---

### Rotate

```javascript
rotate(angle);
```

Rotates the coordinate system.

---

### Update Angle

```javascript
angle += 0.03;
```

Every frame,

the angle increases,

producing continuous rotation.

---

# Output

```
Square

↓

Rotates continuously

around

its center.
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| rotate() | Rotate coordinate system |
| translate() | Move origin |
| rectMode(CENTER) | Rotate around center |
| push() | Save transformation |
| pop() | Restore transformation |

---

# Concepts Learned

✔ Rotation

✔ Coordinate System

✔ Origin

✔ Angle

✔ Continuous Rotation

---

# Viva Questions

### Q1

Why do we use `translate()` before `rotate()`?

Answer

To move the origin to the desired pivot point.

---

### Q2

What unit does `rotate()` use?

Answer

Radians.

---

### Q3

What is PI?

Answer

π (approximately 3.14159).

```
PI

=

180°
```

---

### Q4

What is TWO_PI?

Answer

```
360°
```

---

# Common Mistakes

❌ Forgetting

```javascript
rectMode(CENTER);
```

Rectangle rotates incorrectly.

---

❌ Rotating before translating.

Incorrect

```javascript
rotate(angle);

translate(...);
```

Correct

```javascript
translate(...);

rotate(angle);
```

---

# Problem 10
# Scaling Transformation

## Objective

Create a shape whose size continuously increases and decreases.

---

# Theory

Scaling changes the size of an object.

Unlike translation,

the object remains in the same position.

Unlike rotation,

its orientation does not change.

---

# Types of Scaling

### Uniform Scaling

```
scale(2);
```

Width and height increase equally.

---

### Non-uniform Scaling

```javascript
scale(2,1);
```

Width doubles.

Height remains unchanged.

---

# Understanding scale()

```
scale(1)
```

Original Size

```
scale(2)
```

Double Size

```
scale(0.5)
```

Half Size

---

# Algorithm

Step 1

Create canvas.

Step 2

Create scale variable.

Step 3

Translate to center.

Step 4

Apply scaling.

Step 5

Draw object.

Step 6

Increase and decrease scaling factor.

---

# Source Code

```javascript
let scaleFactor = 1;

let growing = true;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(220);

    push();

    translate(width/2,height/2);

    scale(scaleFactor);

    fill(0,180,120);

    circle(0,0,100);

    pop();

    if(growing){

        scaleFactor += 0.01;

    }

    else{

        scaleFactor -= 0.01;

    }

    if(scaleFactor >= 2){

        growing = false;

    }

    if(scaleFactor <= 0.5){

        growing = true;

    }

}
```

---

# Code Explanation

### Scale Variable

```javascript
scaleFactor
```

Stores the current scaling value.

---

### Scaling

```javascript
scale(scaleFactor);
```

Changes the size of everything drawn afterward.

---

### Growing

```javascript
scaleFactor += 0.01;
```

Object becomes larger.

---

### Shrinking

```javascript
scaleFactor -= 0.01;
```

Object becomes smaller.

---

### Direction Change

```javascript
growing = false;
```

Starts shrinking.

---

# Visual Representation

```
Small

↓

Medium

↓

Large

↓

Medium

↓

Small
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| scale() | Resize object |
| translate() | Move origin |
| circle() | Draw object |
| push() | Save state |
| pop() | Restore state |

---

# Concepts Learned

✔ Scaling

✔ Uniform Scaling

✔ Dynamic Size

✔ Transformation

✔ Animation

---

# Viva Questions

### Q1

Does scaling change position?

Answer

No.

Only the size changes.

---

### Q2

Can scaling make an object smaller?

Answer

Yes.

Example

```javascript
scale(0.5);
```

---

### Q3

Can scaling enlarge an object?

Answer

Yes.

Example

```javascript
scale(3);
```

---

# Common Mistakes

❌ Forgetting

```javascript
push();

pop();
```

Scaling affects every object drawn afterward.

---

❌ Using

```javascript
scaleFactor = 0;
```

The object disappears.

---

❌ Using negative scaling accidentally.

Negative scaling flips the object.

---

# Summary of Part 3A

After completing this section, you should understand:

✔ Rotation

✔ Pivot Point

✔ Radians

✔ PI and TWO_PI

✔ Scaling

✔ Uniform Scaling

✔ Dynamic Size Animation

✔ Coordinate Transformations

---

## Next Part

**Part 3B** covers:

- **Problem 11:** Combined Transformations (Translation + Rotation + Scaling)
- **Problem 12:** Interactive Transformations using Keyboard and Mouse

These complete the transformation chapter and prepare you for interactive graphics programming.

# Part 3B-1 — Transformations (Problem 11)

---

# Problem 11
# Combined Transformation
## (Translation + Rotation + Scaling)

---

# Objective

Create a p5.js program that combines all three basic transformations:

- Translation
- Rotation
- Scaling

on a single object.

This experiment demonstrates how multiple transformations can be applied together to create complex animations.

---

# Theory

In Computer Graphics, an object rarely undergoes only one transformation.

For example,

A moving wheel

- Moves forward
- Rotates
- Changes size depending on camera distance

Similarly,

A spaceship in a game may

- Move
- Rotate
- Zoom in/out

at the same time.

Therefore, transformations are usually combined.

---

# Three Basic Transformations

## 1. Translation

Moves an object from one position to another.

```
translate(x,y)
```

---

## 2. Rotation

Changes the orientation.

```
rotate(angle)
```

---

## 3. Scaling

Changes size.

```
scale(scaleFactor)
```

---

# Transformation Order

The order of transformations is extremely important.

Example

```javascript
translate();

rotate();

scale();
```

is NOT the same as

```javascript
scale();

rotate();

translate();
```

Changing the order changes the final output.

---

# Transformation Pipeline

```
Original Object

↓

Translation

↓

Rotation

↓

Scaling

↓

Final Object
```

---

# Why use push() and pop()?

Transformations affect everything drawn afterward.

Therefore,

```javascript
push();

translate(...);

rotate(...);

scale(...);

draw();

pop();
```

limits the transformation to only one object.

---

# Algorithm

Step 1

Create canvas.

Step 2

Create variables

- Position
- Rotation Angle
- Scale Factor

Step 3

Translate coordinate system.

Step 4

Rotate coordinate system.

Step 5

Scale coordinate system.

Step 6

Draw rectangle.

Step 7

Update all variables.

---

# Source Code

```javascript
let x = 0;

let angle = 0;

let scaleFactor = 1;

let growing = true;

function setup(){

    createCanvas(700,400);

    rectMode(CENTER);

}

function draw(){

    background(230);

    push();

    translate(x,height/2);

    rotate(angle);

    scale(scaleFactor);

    fill(255,150,0);

    rect(0,0,100,100);

    pop();

    // Translation

    x += 2;

    if(x > width+50){

        x = -50;

    }

    // Rotation

    angle += 0.04;

    // Scaling

    if(growing){

        scaleFactor += 0.01;

    }

    else{

        scaleFactor -= 0.01;

    }

    if(scaleFactor >= 1.8){

        growing = false;

    }

    if(scaleFactor <= 0.6){

        growing = true;

    }

}
```

---

# Program Output

The rectangle

✔ Moves across the screen

✔ Rotates continuously

✔ Grows larger

✔ Shrinks smaller

All at the same time.

---

# Step-by-Step Explanation

## Step 1

Move the origin.

```javascript
translate(x,height/2);
```

Now the rectangle moves horizontally.

---

## Step 2

Rotate the coordinate system.

```javascript
rotate(angle);
```

The rectangle spins.

---

## Step 3

Scale the coordinate system.

```javascript
scale(scaleFactor);
```

The rectangle grows and shrinks.

---

## Step 4

Draw the rectangle.

```javascript
rect(0,0,100,100);
```

Because of previous transformations,

the rectangle appears

- translated
- rotated
- scaled

simultaneously.

---

# Animation Variables

### Translation

```javascript
x += 2;
```

Moves object right.

---

### Rotation

```javascript
angle += 0.04;
```

Rotates continuously.

---

### Scaling

```javascript
scaleFactor += 0.01;
```

or

```javascript
scaleFactor -= 0.01;
```

Changes size.

---

# Visual Representation

```
Frame 1

□

↓

Frame 20

↻

↓

Frame 40

⬜

↓

Frame 60

↻⬛

↓

Frame 80

Large Rotating Square

Moving →
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| translate() | Move object |
| rotate() | Rotate object |
| scale() | Resize object |
| push() | Save state |
| pop() | Restore state |
| rectMode(CENTER) | Rotate around center |

---

# Concepts Learned

✔ Translation

✔ Rotation

✔ Scaling

✔ Animation

✔ Transformation Order

✔ Coordinate System

✔ Combined Transformations

---

# Why Order Matters

Example

### Correct

```javascript
translate();

rotate();

scale();

rect();
```

Output

```
Move

↓

Rotate

↓

Resize
```

---

Example

```javascript
scale();

translate();

rotate();
```

Produces an entirely different animation.

---

# Common Mistakes

## Mistake 1

Forgetting

```javascript
push();

pop();
```

Result

Every object becomes transformed.

---

## Mistake 2

Rotating before translation unintentionally.

Different transformation order

↓

Different animation.

---

## Mistake 3

Using

```javascript
rectMode(CORNER);
```

Rectangle rotates around its corner.

Instead use

```javascript
rectMode(CENTER);
```

---

## Mistake 4

Never changing

```javascript
angle
```

Rectangle never rotates.

---

## Mistake 5

Never changing

```javascript
scaleFactor
```

Rectangle never grows or shrinks.

---

# Viva Questions

## Q1

What are the three basic transformations?

Answer

- Translation
- Rotation
- Scaling

---

## Q2

Why are push() and pop() necessary?

Answer

To prevent transformations from affecting other objects.

---

## Q3

Does transformation order matter?

Answer

Yes.

Changing the order produces different results.

---

## Q4

Can multiple transformations be applied simultaneously?

Answer

Yes.

This is common in animation, games, robotics, and computer graphics.

---

## Q5

What happens if scale() is called before translate()?

Answer

The translation itself is scaled, changing the object's final position.

---

# Real-Life Applications

Combined transformations are used in

- Computer Games
- Animation Movies
- CAD Software
- Virtual Reality
- Robotics
- Mechanical Simulations
- 3D Graphics
- Mobile Applications

---

# Summary

After completing this experiment, you should understand

✔ Multiple Transformations

✔ Transformation Pipeline

✔ Transformation Order

✔ Coordinate Systems

✔ Animated Graphics

✔ Professional Graphics Programming

---

# Next Part

**Problem 12 – Interactive Transformations**

You will learn how to control

- Translation
- Rotation
- Scaling

using

- Keyboard
- Mouse

just like professional graphics editors and games.

# Part 3B-2 — Transformations (Problem 12)

---

# Problem 12
# Interactive Transformations
## (Keyboard & Mouse Controlled)

---

# Objective

Create an interactive animation where the user can control an object's

- Translation
- Rotation
- Scaling

using the keyboard.

This experiment introduces **user interaction** with graphical transformations.

---

# Theory

So far, every animation has been **automatic**.

The object moved because the program updated its position every frame.

In real applications such as

- Games
- Graphic Editors
- CAD Software
- Animation Tools

the user controls the object.

Interactive graphics combine

- User Input
- Animation
- Transformations

to create dynamic applications.

---

# Keyboard Controls

For this experiment, use:

| Key | Action |
|------|---------|
| ← | Move Left |
| → | Move Right |
| ↑ | Move Up |
| ↓ | Move Down |
| A | Rotate Left |
| D | Rotate Right |
| W | Increase Size |
| S | Decrease Size |

---

# Theory of Keyboard Input

p5.js provides two common ways to read keyboard input.

## Method 1

```javascript
keyPressed()
```

Runs once whenever a key is pressed.

---

## Method 2

```javascript
keyIsDown()
```

Runs continuously while a key is being held.

For smooth movement,

`keyIsDown()` is recommended.

---

# Variables Used

```javascript
x
```

Stores horizontal position.

---

```javascript
y
```

Stores vertical position.

---

```javascript
angle
```

Stores current rotation.

---

```javascript
scaleFactor
```

Stores current object size.

---

# Algorithm

Step 1

Create canvas.

Step 2

Initialize

- Position
- Rotation
- Scale

Step 3

Translate coordinate system.

Step 4

Rotate coordinate system.

Step 5

Scale coordinate system.

Step 6

Draw rectangle.

Step 7

Read keyboard input.

Step 8

Update transformation variables.

---

# Source Code

```javascript
let x = 350;
let y = 200;

let angle = 0;

let scaleFactor = 1;

function setup(){

    createCanvas(700,400);

    rectMode(CENTER);

}

function draw(){

    background(240);

    push();

    translate(x,y);

    rotate(angle);

    scale(scaleFactor);

    fill(80,170,255);

    rect(0,0,100,100);

    pop();

    // Translation

    if(keyIsDown(LEFT_ARROW)){

        x -= 3;

    }

    if(keyIsDown(RIGHT_ARROW)){

        x += 3;

    }

    if(keyIsDown(UP_ARROW)){

        y -= 3;

    }

    if(keyIsDown(DOWN_ARROW)){

        y += 3;

    }

    // Rotation

    if(keyIsDown(65)){     // A

        angle -= 0.05;

    }

    if(keyIsDown(68)){     // D

        angle += 0.05;

    }

    // Scaling

    if(keyIsDown(87)){     // W

        scaleFactor += 0.02;

    }

    if(keyIsDown(83)){     // S

        scaleFactor -= 0.02;

    }

    scaleFactor = constrain(scaleFactor,0.3,3);

    fill(0);

    textSize(18);

    text("Arrow Keys : Move",20,30);

    text("A / D : Rotate",20,60);

    text("W / S : Scale",20,90);

}
```

---

# Program Output

The rectangle can be

✔ Moved

✔ Rotated

✔ Enlarged

✔ Reduced

using the keyboard.

---

# Code Explanation

## Step 1

Move the coordinate system.

```javascript
translate(x,y);
```

The rectangle appears at `(x,y)`.

---

## Step 2

Rotate the coordinate system.

```javascript
rotate(angle);
```

The rectangle rotates around its center.

---

## Step 3

Apply scaling.

```javascript
scale(scaleFactor);
```

Changes the size of the rectangle.

---

## Step 4

Draw the rectangle.

```javascript
rect(0,0,100,100);
```

Because of the transformations, the rectangle is displayed at its updated position, orientation, and size.

---

# Understanding keyIsDown()

Example

```javascript
if(keyIsDown(LEFT_ARROW)){

    x -= 3;

}
```

As long as the Left Arrow is held,

the rectangle continues moving left.

---

# ASCII Representation

Initial Position

```
           □
```

Press →

```
              □
```

Press ↑

```
          □
```

Press A

```
         ◇
```

Press W

```
        ⬜
```

---

# Understanding constrain()

```javascript
scaleFactor = constrain(scaleFactor,0.3,3);
```

Limits the scaling factor.

Without it,

```
scaleFactor

↓

0

↓

Negative

↓

Object disappears
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| keyIsDown() | Detect held keys |
| translate() | Move object |
| rotate() | Rotate object |
| scale() | Resize object |
| constrain() | Restrict values |
| text() | Display instructions |

---

# Concepts Learned

✔ Keyboard Input

✔ Interactive Graphics

✔ Translation

✔ Rotation

✔ Scaling

✔ User-Controlled Animation

✔ Real-Time Interaction

---

# Common Mistakes

## Mistake 1

Using

```javascript
keyPressed()
```

instead of

```javascript
keyIsDown()
```

Result

Movement occurs only once per key press.

---

## Mistake 2

Not using `constrain()`.

Result

The object may become extremely large or disappear.

---

## Mistake 3

Forgetting `rectMode(CENTER)`.

Result

The rectangle rotates around a corner.

---

## Mistake 4

Drawing the rectangle before applying transformations.

Incorrect

```javascript
rect(...);

translate(...);
```

Correct

```javascript
translate(...);

rotate(...);

scale(...);

rect(...);
```

---

# Viva Questions

### Q1

What is the difference between `keyPressed()` and `keyIsDown()`?

**Answer**

- `keyPressed()` executes once when a key is pressed.
- `keyIsDown()` continues executing while the key is held.

---

### Q2

Why is `constrain()` used?

**Answer**

It limits a variable to a specified range.

Example:

```javascript
constrain(scaleFactor,0.3,3);
```

---

### Q3

Can multiple keys be pressed simultaneously?

**Answer**

Yes.

For example,

- Hold **Right Arrow** to move.
- Hold **D** to rotate.
- Hold **W** to enlarge.

All transformations occur together.

---

### Q4

Why use `push()` and `pop()`?

**Answer**

They isolate transformations so that only the intended object is affected.

---

### Q5

Where are interactive transformations used?

**Answer**

- Video Games
- Image Editors
- CAD Software
- Robotics
- Simulation Software
- 3D Modeling
- Virtual Reality
- User Interfaces

---

# Practice Exercises

Try the following improvements:

### Exercise 1

Replace the rectangle with a circle.

---

### Exercise 2

Use the mouse instead of the keyboard for movement.

---

### Exercise 3

Allow the mouse wheel to control scaling.

---

### Exercise 4

Change the object's color while rotating.

---

### Exercise 5

Add a reset key (`R`) to restore:

- Position
- Rotation
- Scale

---

# Chapter Summary — Transformations

After completing Problems **08–12**, you should understand:

✔ Translation

✔ Rotation

✔ Scaling

✔ Coordinate Systems

✔ Transformation Order

✔ `push()` / `pop()`

✔ Keyboard Interaction

✔ User-Controlled Animation

✔ Combined Transformations

✔ Real-Time Graphics

---

## What's Next?

The next chapter is **Interactivity (Problems 13–16)**, where you'll learn:

- Mouse Tracking
- Mouse Click Events
- Keyboard-Controlled Objects
- UI Components (Slider & Button)

These concepts are essential for building interactive graphics, games, and multimedia applications.

# 🎮 Part 4A — Interactivity (Problems 13–14)

---

# Chapter 4: Interactivity

## Introduction

So far, our programs have been **passive**—they ran automatically without any user input.

In this chapter, we introduce **interactivity**, where the user can control the program using:

- 🖱 Mouse
- ⌨ Keyboard
- 🎛 UI Elements (Slider, Button)

Interactive graphics are used in almost every modern application, including:

- Video Games
- Drawing Software
- Animation Tools
- CAD Software
- Mobile Applications
- Data Visualization
- Robotics Simulation

---

# User Interaction Flow

```text
        User

          │

          ▼

     Mouse / Keyboard

          │

          ▼

     p5.js Event

          │

          ▼

 Update Object Properties

          │

          ▼

     Redraw Canvas
```

---

# Problem 13

# Graphical Shapes Follow Mouse

---

## 🎯 Objective

Create a program where a graphical object follows the mouse cursor in real time.

---

# Theory

One of the most useful features of p5.js is that it continuously tracks the mouse position.

Two built-in variables are always available.

```javascript
mouseX
mouseY
```

These values automatically update every frame.

---

## Coordinate System

```text
(0,0)
+------------------------------------------→ X

|

|

|

↓

Y
```

---

## Mouse Tracking

```text
Mouse

        ●

        │

        ▼

     Circle follows
```

---

# Real-Life Applications

Mouse tracking is used in

- Paint Applications
- Cursor Effects
- Games
- Drag-and-Drop Systems
- Object Selection
- Graphic Editors

---

# Algorithm

```
Start

↓

Create Canvas

↓

Read mouseX

↓

Read mouseY

↓

Draw Shape

↓

Repeat
```

---

# Source Code

```javascript
function setup(){

    createCanvas(700,400);

}

function draw(){

    background(230);

    // Heading
    fill(0);

    textSize(22);

    text("Move the Mouse",20,30);

    // Circle follows mouse

    fill(50,150,255);

    circle(mouseX,mouseY,60);

}
```

---

# Program Output

```
Mouse

        ●

        Circle always follows.
```

---

# Step-by-Step Explanation

### Canvas

```javascript
createCanvas(700,400);
```

Creates the drawing area.

---

### Mouse Position

```javascript
mouseX
```

Returns the current horizontal position.

Example

```
0

↓

350

↓

700
```

---

### Vertical Position

```javascript
mouseY
```

Returns the current vertical position.

---

### Draw Circle

```javascript
circle(mouseX,mouseY,60);
```

Since the center of the circle is the mouse position,

the object continuously follows the cursor.

---

# Challenge Version

Instead of one object,

create five circles.

```text
        ○

   ○    ●    ○

        ○
```

Hint

Use

```javascript
circle(mouseX+50,mouseY,30);
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| mouseX | Horizontal mouse position |
| mouseY | Vertical mouse position |
| circle() | Draw circle |
| background() | Refresh animation |

---

# Tips

💡 `mouseX` and `mouseY` are updated automatically.

You never need to assign values manually.

---

# Common Mistakes

❌ Writing

```javascript
circle(100,100,60);
```

The object never follows the mouse.

Correct

```javascript
circle(mouseX,mouseY,60);
```

---

❌ Forgetting

```javascript
background();
```

Result

The mouse leaves a trail.

---

# Practice Exercises

### Exercise 1

Replace the circle with a rectangle.

---

### Exercise 2

Make the object larger.

---

### Exercise 3

Change color depending on mouse position.

Hint

```javascript
fill(mouseX,100,mouseY);
```

---

# Viva Questions

### Q1

What is mouseX?

**Answer**

It stores the current horizontal position of the mouse.

---

### Q2

What is mouseY?

**Answer**

It stores the current vertical position of the mouse.

---

### Q3

Why does the object move without updating variables?

**Answer**

Because p5.js automatically updates `mouseX` and `mouseY` every frame.

---

# Quick Revision

✔ mouseX

✔ mouseY

✔ circle()

✔ background()

---

# Problem 14

# Mouse Click Changes Color and Size

---

## 🎯 Objective

Create a program where clicking the mouse changes

- Color
- Size

of a shape.

---

# Theory

p5.js supports several mouse events.

The most common is

```javascript
mousePressed()
```

This function runs once whenever the mouse button is clicked.

---

# Event Flow

```text
Mouse Click

      │

      ▼

mousePressed()

      │

      ▼

Update Variables

      │

      ▼

Draw New Object
```

---

# Real-Life Applications

Mouse click events are used in

- Buttons
- Menus
- Drawing Apps
- Interactive Games
- UI Components

---

# Algorithm

```
Create Canvas

↓

Draw Circle

↓

Wait for Mouse Click

↓

Generate Random Color

↓

Generate Random Size

↓

Redraw
```

---

# Source Code

```javascript
let r = 255;
let g = 0;
let b = 0;

let size = 80;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(240);

    fill(r,g,b);

    circle(width/2,height/2,size);

    fill(0);

    textSize(18);

    text("Click Anywhere",20,30);

}

function mousePressed(){

    r = random(255);

    g = random(255);

    b = random(255);

    size = random(40,160);

}
```

---

# Output

Initially

```text
🔴
```

After every click

```text
🟢

🔵

🟣

🟡

🟠
```

Different color

Different size

---

# Step-by-Step Explanation

## Color Variables

```javascript
r
g
b
```

Store RGB values.

---

## Random Color

```javascript
random(255)
```

Generates a random value between

```
0

↓

255
```

---

## Random Size

```javascript
size = random(40,160);
```

Every click produces a new diameter.

---

## Mouse Event

```javascript
mousePressed()
```

Runs automatically when the mouse button is clicked.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| mousePressed() | Detect click |
| random() | Generate random values |
| fill() | Apply color |
| circle() | Draw object |

---

# Tips

💡 `mousePressed()` runs **once** for each click.

Unlike `draw()`, it does **not** repeat continuously.

---

# Common Mistakes

❌ Calling

```javascript
random()
```

inside

```javascript
draw()
```

Result

Color changes every frame.

Correct

Use

```javascript
mousePressed()
```

---

❌ Forgetting global variables.

Incorrect

```javascript
function mousePressed(){

    let r = random(255);

}
```

The color won't update outside the function.

---

# Practice Exercises

### Exercise 1

Draw a rectangle instead of a circle.

---

### Exercise 2

Generate a random background color.

---

### Exercise 3

Display the number of mouse clicks.

Hint

```javascript
count++;
```

---

# Viva Questions

### Q1

When does `mousePressed()` execute?

**Answer**

Once whenever the mouse button is clicked.

---

### Q2

Why use `random()`?

**Answer**

To generate unpredictable colors and sizes.

---

### Q3

Can multiple properties change in one click?

**Answer**

Yes.

You can change:

- Color
- Size
- Position
- Rotation
- Speed

all inside `mousePressed()`.

---

# Chapter Summary

After completing Problems **13–14**, you should understand:

✔ Mouse Tracking

✔ Mouse Events

✔ Random Colors

✔ Random Sizes

✔ Event-Driven Programming

✔ Interactive Graphics

---

# Coming Next

## 🎮 Part 4B

Problems **15–16**

- Keyboard-Controlled Object Movement
- Slider and Button UI Controls

These experiments introduce keyboard interaction and graphical user interface (GUI) components, completing the Interactivity chapter.

# 🎮 Part 4B-1 — Interactivity

---

# Problem 15

# Keyboard Controlled Object Movement

---

## 🎯 Objective

Create a p5.js program where a graphical object can be moved using the keyboard.

The object should respond to:

- ⬅ Left Arrow
- ➡ Right Arrow
- ⬆ Up Arrow
- ⬇ Down Arrow

(or alternatively W, A, S, D keys).

---

# 📖 Theory

One of the most common interactions in computer graphics is **keyboard input**.

Unlike automatic animation, the movement depends entirely on the user's actions.

The keyboard is used extensively in

- 🎮 Games
- 🤖 Robotics
- 🚗 Driving Simulators
- 🎨 Drawing Software
- 🧩 Puzzle Games
- 🛸 Space Simulations

---

# Keyboard Event Flow

```text
        Keyboard

            │

            ▼

      keyIsDown()

            │

            ▼

      Update Position

            │

            ▼

      Draw New Frame
```

---

# Understanding Coordinates

```text
           Y

           ▲

           |

           |

(0,0)----------------------------► X
```

Moving Right

```
x = x + speed
```

Moving Left

```
x = x - speed
```

Moving Down

```
y = y + speed
```

Moving Up

```
y = y - speed
```

---

# 📚 Built-in Keyboard Functions

There are two commonly used keyboard functions.

## Method 1

```javascript
keyPressed()
```

Runs only once.

---

## Method 2

```javascript
keyIsDown()
```

Runs continuously while the key is pressed.

For smooth movement,

always use

```javascript
keyIsDown()
```

---

# Algorithm

```
Start

↓

Create Canvas

↓

Create Object

↓

Check Keyboard

↓

Update Position

↓

Draw Object

↓

Repeat
```

---

# Source Code

```javascript
let x = 350;
let y = 200;

let speed = 5;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(230);

    // Keyboard Input

    if(keyIsDown(LEFT_ARROW)){

        x -= speed;

    }

    if(keyIsDown(RIGHT_ARROW)){

        x += speed;

    }

    if(keyIsDown(UP_ARROW)){

        y -= speed;

    }

    if(keyIsDown(DOWN_ARROW)){

        y += speed;

    }

    // Prevent object from leaving canvas

    x = constrain(x,25,width-25);

    y = constrain(y,25,height-25);

    // Draw Player

    fill(60,170,255);

    circle(x,y,50);

    // Instructions

    fill(0);

    textSize(18);

    text("Use Arrow Keys to Move",20,30);

}
```

---

# ▶ Output

Initially

```text
          ●
```

Press Right

```text
                ●
```

Press Left

```text
      ●
```

Press Up

```text
      ●
```

Press Down

```text

      ●
```

The circle follows the direction of the pressed arrow key.

---

# 📝 Code Explanation

## Step 1

Create the position variables.

```javascript
let x = 350;

let y = 200;
```

These store the current location of the circle.

---

## Step 2

Create speed.

```javascript
let speed = 5;
```

This controls how many pixels the object moves each frame.

Higher value

↓

Faster movement

Lower value

↓

Slower movement

---

## Step 3

Detect keyboard input.

```javascript
if(keyIsDown(LEFT_ARROW))
```

If the left arrow key is held,

the condition becomes true.

---

## Step 4

Move object.

```javascript
x -= speed;
```

Moves left.

---

```javascript
x += speed;
```

Moves right.

---

```javascript
y -= speed;
```

Moves up.

---

```javascript
y += speed;
```

Moves down.

---

## Step 5

Prevent object leaving the screen.

```javascript
constrain(x,25,width-25);
```

This keeps the center of the circle inside the canvas.

Without this,

the object can disappear outside the screen.

---

# 📊 Movement Table

| Key | Operation |
|------|-----------|
| ← | x -= speed |
| → | x += speed |
| ↑ | y -= speed |
| ↓ | y += speed |

---

# 🎯 Important Functions

| Function | Purpose |
|----------|----------|
| keyIsDown() | Detect key continuously |
| constrain() | Limit movement |
| circle() | Draw player |
| background() | Refresh screen |

---

# 💡 Pro Tips

### Tip 1

Store movement speed in a variable.

Instead of

```javascript
x += 5;
```

Use

```javascript
x += speed;
```

Changing one variable updates the entire movement system.

---

### Tip 2

Always use

```javascript
background()
```

inside

```javascript
draw()
```

Otherwise,

old frames remain visible.

---

### Tip 3

Use

```javascript
constrain()
```

to prevent objects from leaving the screen.

---

# ⚠ Common Mistakes

## Mistake 1

Using

```javascript
keyPressed()
```

instead of

```javascript
keyIsDown()
```

Result

The object moves only once.

---

## Mistake 2

Updating position outside

```javascript
draw()
```

Animation stops.

---

## Mistake 3

Forgetting

```javascript
background();
```

Leaves trails behind the object.

---

## Mistake 4

Not using

```javascript
constrain();
```

Object disappears outside the canvas.

---

# 🚀 Challenge Exercises

### ⭐ Easy

Replace the circle with a rectangle.

---

### ⭐⭐ Medium

Use W, A, S, D keys instead.

Hint

```javascript
keyIsDown(65)
```

A key

---

```javascript
keyIsDown(68)
```

D key

---

```javascript
keyIsDown(87)
```

W key

---

```javascript
keyIsDown(83)
```

S key

---

### ⭐⭐⭐ Hard

Increase speed while holding

SHIFT

Hint

```javascript
if(keyIsDown(SHIFT)){

speed = 10;

}
```

---

### ⭐⭐⭐⭐ Expert

Move two different objects using

Arrow Keys

and

WASD

simultaneously.

---

# 🌍 Real-Life Applications

Keyboard movement is used in

- 🎮 Video Games
- 🚗 Driving Games
- 🤖 Robot Navigation
- ✈ Flight Simulators
- 📍 Map Navigation
- 🛰 Drone Controllers

---

# 🎓 Viva Questions

### Q1

What is the difference between

```javascript
keyPressed()
```

and

```javascript
keyIsDown()
```

### Answer

`keyPressed()`

runs once.

`keyIsDown()`

runs continuously while the key is held.

---

### Q2

Why do we use

```javascript
constrain()
```

### Answer

To prevent the object from moving outside the canvas.

---

### Q3

Can multiple keys be pressed together?

### Answer

Yes.

For example,

Press

```
UP

+

RIGHT
```

The object moves diagonally.

---

### Q4

Why use a speed variable?

### Answer

Changing a single variable changes the movement speed everywhere in the program.

---

# 📌 Quick Revision

✅ keyIsDown()

✅ constrain()

✅ Arrow Keys

✅ Variables

✅ Animation Loop

✅ Interactive Graphics

---

# 📖 Summary

After completing this experiment, you should understand

✔ Keyboard Interaction

✔ Continuous Key Detection

✔ Object Movement

✔ Speed Control

✔ Boundary Restriction

✔ Interactive Animation

---

# 🔜 Next Experiment

## Problem 16

### UI Controls (Slider & Button)

You will learn

- createSlider()
- createButton()
- Event Handling
- Dynamic Object Control
- Graphical User Interfaces (GUI)

This completes the **Interactivity** chapter.

# 🎮 Part 4B-2 — Interactivity

---

# Problem 16

# UI Controls (Slider & Button)

---

## 🎯 Objective

Create a p5.js program that uses **UI elements** such as a **slider** and a **button** to control the properties of an object.

The program should demonstrate how graphical user interface (GUI) components can interact with canvas objects in real time.

---

# 📖 Theory

Besides drawing shapes and animations, p5.js provides built-in **DOM (Document Object Model)** functions that allow us to create graphical user interface (GUI) components.

Some commonly used UI elements are:

- Slider
- Button
- Checkbox
- Input Box
- Dropdown Menu

These elements allow users to interact with programs without writing code.

---

# What is a GUI?

GUI stands for **Graphical User Interface**.

Instead of typing commands, users interact using visual controls.

Examples include:

- Volume controls
- Brightness sliders
- Submit buttons
- Zoom controls
- Media players

---

# GUI Interaction Flow

```text
        User

          │

          ▼

   Slider / Button

          │

          ▼

     Update Variable

          │

          ▼

      draw() Function

          │

          ▼

      Updated Object
```

---

# Real-Life Applications

UI controls are used in:

- 🎮 Games
- 🎵 Music Players
- 📷 Photo Editors
- 🎬 Animation Software
- 📊 Data Visualization
- 🎨 Drawing Applications

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Create Slider

↓

Create Button

↓

Read Slider Value

↓

Draw Circle

↓

If Button Clicked

↓

Change Color

↓

Repeat
```

---

# Source Code

```javascript
let slider;
let button;

let r = 100;
let g = 150;
let b = 255;

function setup(){

    createCanvas(700,400);

    slider = createSlider(30,200,80);

    slider.position(20,420);

    button = createButton("Change Color");

    button.position(220,420);

    button.mousePressed(changeColor);

}

function draw(){

    background(230);

    let size = slider.value();

    fill(r,g,b);

    noStroke();

    circle(width/2,height/2,size);

    fill(0);

    textSize(18);

    text("Circle Size: " + size,20,30);

}

function changeColor(){

    r = random(255);

    g = random(255);

    b = random(255);

}
```

---

# Program Output

Initially

```text
          🔵
```

Move Slider →

```text
Small ●

↓

Medium ●

↓

Large ●
```

Click Button →

```text
🔵

↓

🟢

↓

🟣

↓

🟡
```

The circle changes color every time the button is clicked.

---

# Step-by-Step Code Explanation

## Step 1 — Create Slider

```javascript
slider = createSlider(30,200,80);
```

Creates a slider.

Parameters:

```text
Minimum Value : 30

Maximum Value : 200

Default Value : 80
```

---

## Step 2 — Position Slider

```javascript
slider.position(20,420);
```

Places the slider below the canvas.

---

## Step 3 — Create Button

```javascript
button = createButton("Change Color");
```

Creates a clickable button with the text:

```
Change Color
```

---

## Step 4 — Button Event

```javascript
button.mousePressed(changeColor);
```

Whenever the button is clicked,

the function

```javascript
changeColor()
```

is executed.

---

## Step 5 — Read Slider Value

```javascript
slider.value();
```

Returns the current slider position.

Example

```text
Slider

30 ---------- 200

        ▲

Value = 95
```

---

## Step 6 — Draw Circle

```javascript
circle(width/2,height/2,size);
```

The diameter depends on the slider value.

---

## Step 7 — Random Color

```javascript
random(255)
```

Generates a random RGB value.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| createSlider() | Creates a slider |
| slider.value() | Reads slider value |
| createButton() | Creates a button |
| mousePressed() | Executes on button click |
| random() | Generates random values |

---

# Slider vs Button

| Slider | Button |
|---------|---------|
| Continuous control | Single action |
| Returns numeric value | Executes a function |
| Used for size, speed, volume | Used for reset, play, color change |

---

# Visual Illustration

## Slider

```text
30 ------------------------ 200

             ▲

         Current Value
```

---

## Button

```text
+-------------------+

|   Change Color    |

+-------------------+
```

Click

↓

Program executes a function.

---

# Tips

### Tip 1

Always store UI elements in variables.

Example

```javascript
slider
button
```

---

### Tip 2

Read slider values inside `draw()`.

That way, changes appear immediately.

---

### Tip 3

Use a separate function for button actions.

Example

```javascript
button.mousePressed(changeColor);
```

instead of placing all code inside `draw()`.

---

# Common Mistakes

## Mistake 1

Creating the slider inside `draw()`.

❌ Wrong

```javascript
function draw(){

    createSlider(...);

}
```

Result:

Hundreds of sliders are created every second.

---

## Mistake 2

Forgetting

```javascript
slider.value()
```

The program cannot read the slider position.

---

## Mistake 3

Using

```javascript
button.mousePressed()
```

inside `draw()`.

Register button events only once in `setup()`.

---

## Mistake 4

Using fixed size.

```javascript
circle(...,80);
```

Instead,

```javascript
circle(...,slider.value());
```

---

# Challenge Exercises

## ⭐ Easy

Control the rectangle width using a slider.

---

## ⭐⭐ Medium

Add another slider for color.

Example

```
Red Slider

Green Slider

Blue Slider
```

---

## ⭐⭐⭐ Hard

Create three sliders

- Red
- Green
- Blue

to manually control RGB values.

---

## ⭐⭐⭐⭐ Expert

Add a **Reset Button**.

When clicked,

restore:

- Original Color
- Original Size

---

# Experiment Result

Successfully created an interactive graphical application where:

- The slider controls the size of the circle.
- The button changes the circle's color.
- Changes are reflected instantly on the canvas.

---

# Viva Questions

### Q1

What is GUI?

**Answer**

GUI (Graphical User Interface) allows users to interact with programs using visual elements such as buttons, sliders, and menus.

---

### Q2

What does `createSlider()` return?

**Answer**

It returns a slider object that can be used to read and modify slider values.

---

### Q3

How do you read the current slider value?

**Answer**

```javascript
slider.value();
```

---

### Q4

What is the purpose of `createButton()`?

**Answer**

It creates a clickable button that can execute a function when pressed.

---

### Q5

Why is `button.mousePressed()` placed inside `setup()`?

**Answer**

Because the button event needs to be registered only once. Registering it repeatedly inside `draw()` is inefficient and can lead to unexpected behavior.

---

# 📌 Quick Revision

✅ createSlider()

✅ slider.value()

✅ createButton()

✅ mousePressed()

✅ GUI Components

✅ Event Handling

---

# Chapter Summary

After completing Problems **13–16**, you should understand:

- ✔ Mouse Interaction
- ✔ Mouse Events
- ✔ Keyboard Input
- ✔ Keyboard-Controlled Movement
- ✔ GUI Components
- ✔ Sliders
- ✔ Buttons
- ✔ Event-Driven Programming
- ✔ Interactive Graphics

---

# 🚀 Next Chapter

## Part 5 — Visual Effects and Physics

Problems **17–21**

You will learn:

- ✨ Particle Systems
- 🌟 Glow & Pulsing Effects
- 🌍 Gravity Simulation
- ⚽ Bouncing Balls with Friction
- 💥 Explosion Effects

These topics introduce the fundamentals of game physics and visual effects used in modern graphics applications.

# 🌌 Part 5A — Visual Effects and Physics

---

# Chapter 5: Visual Effects and Physics

## Introduction

Visual effects and physics make computer graphics more realistic and interactive. Instead of drawing static objects, we can simulate natural phenomena such as:

- ✨ Fire
- 🌧 Rain
- ❄ Snow
- 💨 Smoke
- 💥 Explosions
- 🌟 Magic Effects
- 🍂 Falling Leaves

These effects are commonly created using **Particle Systems**.

---

# Problem 17

# Particle System with Fading Effect

---

## 🎯 Objective

Create a particle system where particles

- move in random directions,
- gradually fade over time,
- disappear after a certain lifetime.

---

# 📖 Theory

A **Particle System** is a collection of many small objects called **particles**.

Each particle has its own

- Position
- Velocity
- Size
- Color
- Lifetime

Instead of controlling one object, we control hundreds of tiny particles simultaneously.

Together they create realistic effects.

---

# Real-Life Applications

Particle systems are used in

- 🔥 Fire
- 💨 Smoke
- 💥 Explosion Effects
- 🌊 Water Splash
- ✨ Sparkles
- 🌧 Rain
- ❄ Snow
- 🌌 Galaxy Simulations
- 🎮 Video Games

---

# Particle Life Cycle

```text
Create Particle

      │

      ▼

 Move Randomly

      │

      ▼

 Reduce Lifetime

      │

      ▼

 Become Transparent

      │

      ▼

 Remove Particle
```

---

# Internal Structure of One Particle

```text
Particle

├── Position (x,y)

├── Velocity (vx,vy)

├── Size

├── Alpha

└── Lifetime
```

---

# Mathematical Concept

Every frame,

```
Position

=

Position + Velocity
```

Transparency decreases as

```
Alpha

=

Alpha - FadeSpeed
```

When

```
Alpha ≤ 0
```

the particle disappears.

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Create Empty Particle List

↓

Create New Particle

↓

Move Particle

↓

Decrease Alpha

↓

Display Particle

↓

Remove Dead Particle

↓

Repeat
```

---

# Source Code

```javascript
let particles = [];

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(20);

    particles.push(new Particle(mouseX,mouseY));

    for(let i = particles.length-1; i>=0; i--){

        particles[i].update();

        particles[i].display();

        if(particles[i].finished()){

            particles.splice(i,1);

        }

    }

}

class Particle{

    constructor(x,y){

        this.x = x;

        this.y = y;

        this.vx = random(-2,2);

        this.vy = random(-2,2);

        this.alpha = 255;

        this.size = random(8,16);

    }

    update(){

        this.x += this.vx;

        this.y += this.vy;

        this.alpha -= 4;

    }

    display(){

        noStroke();

        fill(0,200,255,this.alpha);

        circle(this.x,this.y,this.size);

    }

    finished(){

        return this.alpha <= 0;

    }

}
```

---

# Program Output

Move the mouse around the canvas.

Particles continuously appear at the mouse position.

```text
            *

       *   *  *

    *    ●    *

       *   *

           *
```

Older particles become transparent and disappear, creating a smooth trail effect.

---

# Step-by-Step Code Explanation

## Step 1 — Create an Array

```javascript
let particles = [];
```

The array stores every particle currently visible on the screen.

---

## Step 2 — Create a New Particle

```javascript
particles.push(new Particle(mouseX,mouseY));
```

A new particle is created every frame at the current mouse position.

---

## Step 3 — Random Velocity

```javascript
this.vx = random(-2,2);

this.vy = random(-2,2);
```

Each particle moves in a different direction.

Example

```text
↖ ↑ ↗

← ● →

↙ ↓ ↘
```

---

## Step 4 — Update Position

```javascript
this.x += this.vx;

this.y += this.vy;
```

Particles move based on their velocity.

---

## Step 5 — Fade Out

```javascript
this.alpha -= 4;
```

Transparency decreases every frame.

Eventually,

```text
255

↓

200

↓

100

↓

20

↓

0
```

---

## Step 6 — Remove Dead Particles

```javascript
particles.splice(i,1);
```

Deletes particles whose lifetime has ended.

This prevents memory from filling with invisible particles.

---

# Behind the Code

Each frame:

```
Mouse

↓

New Particle

↓

Move

↓

Fade

↓

Disappear

↓

Repeat
```

Over time, hundreds of particles are created and removed automatically.

---

# Important Functions

| Function | Purpose |
|----------|---------|
| random() | Random direction |
| push() | Add particle |
| splice() | Remove particle |
| fill() | Apply transparency |
| noStroke() | Remove border |

---

# Output Observation

- Particles originate from the mouse.
- Each particle follows a unique path.
- Older particles fade smoothly.
- The animation appears continuous and natural.

---

# Optimization Tips

### Tip 1

Always remove finished particles.

Otherwise, the array grows indefinitely and slows the program.

---

### Tip 2

Iterate backwards when deleting objects.

```javascript
for(let i=particles.length-1;i>=0;i--)
```

This avoids index shifting issues.

---

### Tip 3

Keep particle size small for smoother animation.

Large particles require more rendering time.

---

# Common Mistakes

## Mistake 1

Looping forward while deleting particles.

Incorrect

```javascript
for(let i=0;i<particles.length;i++)
```

Some particles may be skipped.

---

## Mistake 2

Never decreasing alpha.

Particles never disappear.

---

## Mistake 3

Never removing dead particles.

Memory usage continuously increases.

---

## Mistake 4

Creating particles outside `draw()`.

Only one particle is created.

---

# Challenge Exercises

### ⭐ Easy

Change particle color to red.

---

### ⭐⭐ Medium

Create larger particles.

---

### ⭐⭐⭐ Hard

Generate particles only when the mouse is pressed.

Hint

```javascript
if(mouseIsPressed){

...
}
```

---

### ⭐⭐⭐⭐ Expert

Use random colors for every particle.

Example

```javascript
fill(random(255),random(255),random(255),this.alpha);
```

---

# 🎓 Viva Questions

### Q1

What is a particle system?

**Answer**

A particle system is a collection of many small particles that work together to simulate natural visual effects.

---

### Q2

Why do particles have a lifetime?

**Answer**

To remove old particles and improve performance.

---

### Q3

Why is transparency reduced gradually?

**Answer**

It creates a smooth fading effect instead of particles disappearing suddenly.

---

### Q4

Why do we use an array?

**Answer**

Because many particles exist simultaneously, and each particle must be stored and updated independently.

---

### Q5

Why do particles move in different directions?

**Answer**

Random velocity values create natural-looking motion.

---

# 📌 Quick Revision

✅ Arrays

✅ Classes

✅ Objects

✅ Random Velocity

✅ Transparency

✅ Particle Lifetime

✅ Fade Effect

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Particle Systems

✔ Arrays of Objects

✔ Random Motion

✔ Transparency

✔ Particle Lifetime

✔ Memory Management

✔ Real-Time Animation

---

# 🚀 Next Experiment

## Problem 18 — Glow and Pulsing Effects

You will learn how to use

- `sin()`
- `cos()`
- Oscillation
- Dynamic Brightness
- Smooth Visual Effects

to create glowing objects commonly seen in games and modern user interfaces.

# 🌟 Part 5A — Visual Effects and Physics

---

# Problem 18

# Glow and Pulsing Effect using Sine and Cosine Functions

---

## 🎯 Objective

Create a glowing circle whose

- Brightness changes smoothly
- Size continuously increases and decreases

using **sine** and **cosine** functions.

This experiment demonstrates mathematical animation techniques used in modern computer graphics.

---

# 📖 Theory

Many natural movements are **periodic**, meaning they repeat over time.

Examples include:

- ❤️ Heartbeat
- 🌊 Ocean Waves
- 🌙 Moon Phases
- 💡 LED Glow
- ✨ Magic Effects
- 🔊 Sound Waves

Instead of changing values randomly, we use mathematical functions like:

- `sin()`
- `cos()`

These produce smooth and continuous motion.

---

# Real-Life Applications

Glow effects are used in:

- 🎮 Video Games
- 💎 Magic Effects
- 🚦 Neon Signs
- 📱 Mobile UI
- 🌟 Stars
- 🔥 Energy Balls
- ⚡ Electricity Effects

---

# Understanding Sine Wave

The value of `sin()` always changes smoothly between

```text
-1

↓

0

↓

1

↓

0

↓

-1
```

Graphically,

```text
1  ─────╮      ╭─────
         ╰────╯

0 ─────────────────────────

-1 ───╯      ╰─────────────
```

This repeating motion is called **oscillation**.

---

# How p5.js Uses sin()

Suppose

```javascript
sin(frameCount * 0.05)
```

Every frame,

`frameCount`

increases.

Therefore,

the sine value changes smoothly.

---

# Converting Sine Values

Since

```text
sin()

↓

-1 → 1
```

we convert it into useful values.

Example

```javascript
map(value,-1,1,80,150)
```

becomes

```text
-1 → 80

0 →115

1 →150
```

Perfect for animation.

---

# Animation Flow

```text
Frame

↓

sin(frameCount)

↓

Size Changes

↓

Brightness Changes

↓

Draw Circle

↓

Repeat
```

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Calculate Sine

↓

Convert Value

↓

Apply Size

↓

Apply Brightness

↓

Draw Circle

↓

Repeat
```

---

# Source Code

```javascript
function setup(){

    createCanvas(700,400);

}

function draw(){

    background(20);

    let glow = map(

        sin(frameCount*0.05),

        -1,1,

        120,255

    );

    let size = map(

        sin(frameCount*0.05),

        -1,1,

        80,160

    );

    noStroke();

    // Outer Glow

    fill(0,180,255,80);

    circle(width/2,height/2,size+40);

    // Middle Glow

    fill(0,180,255,140);

    circle(width/2,height/2,size+20);

    // Main Circle

    fill(glow,255,255);

    circle(width/2,height/2,size);

}
```

---

# Program Output

```text
Frame 1

      ◉

↓

Frame 20

     ◎

↓

Frame 40

    ⬤

↓

Frame 60

     ◎

↓

Frame 80

      ◉
```

The circle appears to breathe or pulse naturally.

---

# Step-by-Step Code Explanation

## Step 1

Calculate the sine value.

```javascript
sin(frameCount*0.05)
```

Produces values between

```text
-1

↓

1
```

---

## Step 2

Convert the value.

```javascript
map(...,80,160)
```

Now the size becomes

```text
80

↓

160
```

instead of

```text
-1

↓

1
```

---

## Step 3

Create Glow Brightness.

```javascript
glow
```

stores the brightness value.

Higher value

↓

Brighter object.

---

## Step 4

Draw Multiple Circles.

Three circles are drawn.

```text
Large Transparent Circle

↓

Medium Transparent Circle

↓

Solid Circle
```

Together they create a glow effect.

---

# Visual Representation

```text
      ***********

    ****     ****

   ***   ●    ***

    ****     ****

      ***********
```

Outer circles have transparency,

making them appear like light.

---

# Why Use Multiple Circles?

Instead of one circle,

multiple transparent circles create a soft glowing appearance.

```text
Circle 1

Alpha = 80

↓

Circle 2

Alpha = 140

↓

Circle 3

Alpha = 255
```

This simulates light spreading outward.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| sin() | Smooth oscillation |
| map() | Convert ranges |
| frameCount | Animation timing |
| fill() | Apply color |
| circle() | Draw circles |

---

# Mathematical Background

The sine function follows

```text
y = sin(x)
```

Properties

- Smooth
- Continuous
- Periodic

This makes it ideal for animations.

---

# Output Observation

The object

✔ Expands smoothly

✔ Shrinks smoothly

✔ Appears brighter

✔ Appears dimmer

No sudden jumps occur.

---

# Optimization Tips

### Tip 1

Use

```javascript
frameCount
```

instead of manually increasing a variable.

---

### Tip 2

Keep the sine multiplier small.

Example

```javascript
0.03

0.05

0.08
```

Large values produce extremely fast animation.

---

### Tip 3

Use transparent layers for realistic glow.

---

# Common Mistakes

## Mistake 1

Using

```javascript
random()
```

instead of

```javascript
sin()
```

Random values create jerky motion.

---

## Mistake 2

Forgetting

```javascript
map()
```

The size becomes

```text
-1

↓

1
```

which is too small to see.

---

## Mistake 3

Using only one circle.

Glow becomes much less realistic.

---

## Mistake 4

Using a very large frame multiplier.

Example

```javascript
sin(frameCount)
```

The animation becomes too fast.

---

# Challenge Exercises

### ⭐ Easy

Change the glow color to red.

---

### ⭐⭐ Medium

Use

```javascript
cos()
```

instead of

```javascript
sin()
```

Observe the difference.

---

### ⭐⭐⭐ Hard

Create two glowing circles with different speeds.

Hint

```javascript
sin(frameCount*0.03)

sin(frameCount*0.07)
```

---

### ⭐⭐⭐⭐ Expert

Create a glowing solar system where each planet pulses independently.

---

# Viva Questions

### Q1

Why is `sin()` preferred over `random()`?

**Answer**

Because `sin()` produces smooth, continuous changes, while `random()` changes abruptly.

---

### Q2

What is the purpose of `map()`?

**Answer**

It converts values from one range to another.

Example:

```text
-1 → 1

↓

80 → 160
```

---

### Q3

Why do we use `frameCount`?

**Answer**

It automatically increases every frame and acts as a timer for animation.

---

### Q4

How is the glow effect created?

**Answer**

By drawing multiple transparent circles of different sizes on top of each other.

---

### Q5

Name two real-life applications of sine-based animation.

**Answer**

- Heartbeat animation
- Neon light effects

(Other examples include waves, breathing indicators, and pulsing buttons.)

---

# 📌 Quick Revision

✅ sin()

✅ cos()

✅ map()

✅ frameCount

✅ Transparency

✅ Layered Drawing

✅ Glow Effect

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Periodic Motion

✔ Sine and Cosine Functions

✔ Smooth Animation

✔ Glow Effects

✔ Brightness Control

✔ Mathematical Animation

✔ Layered Rendering

---

# 🚀 Next Experiment

## Part 5B – Problem 19

### Gravity Simulation

In the next experiment, you will simulate gravity acting on a falling object using concepts of:

- 🌍 Gravity
- 📉 Acceleration
- 🚀 Velocity
- ⚽ Free Fall
- 🧮 Basic Physics

This introduces the foundation of realistic motion used in games, simulations, and physics engines.

# 🌍 Part 5B — Visual Effects and Physics

---

# Problem 19

# Gravity Simulation of Falling Objects

---

## 🎯 Objective

Create a p5.js program to simulate **gravity** acting on a falling object.

The object should:

- Fall from the top of the canvas.
- Accelerate naturally due to gravity.
- Stop when it reaches the ground.

---

# 📖 Theory

Gravity is a natural force that pulls objects toward the Earth.

In computer graphics and game development, gravity is simulated mathematically by continuously increasing the object's downward velocity.

Unlike constant-speed movement, gravity causes objects to **accelerate** as they fall.

---

# Real-Life Applications

Gravity simulation is used in:

- 🎮 Video Games
- 🏀 Sports Simulations
- 🚗 Driving Games
- 🛰 Physics Engines
- 🤖 Robotics
- 🏗 Engineering Simulations
- 🎬 Animation Movies

---

# Understanding Gravity

Imagine dropping a ball.

```text
Start

      ●

      ↓

     ↓↓

    ↓↓↓

   ↓↓↓↓

────────────── Ground
```

Notice that the ball moves faster every moment.

---

# Physics Behind Gravity

Three important quantities are used.

### Position

Current location of the object.

```
y
```

---

### Velocity

How fast the object moves.

```
velocity
```

---

### Acceleration

How quickly velocity changes.

```
gravity
```

---

# Motion Equation

Each frame,

```text
Velocity

=

Velocity + Gravity
```

Then,

```text
Position

=

Position + Velocity
```

This produces realistic falling motion.

---

# Animation Flow

```text
Create Ball

↓

Apply Gravity

↓

Increase Velocity

↓

Update Position

↓

Touch Ground?

↓

No → Continue

↓

Yes → Stop
```

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Initialize Position

↓

Initialize Velocity

↓

Initialize Gravity

↓

Update Velocity

↓

Update Position

↓

Check Ground Collision

↓

Repeat
```

---

# Source Code

```javascript
let y = 50;

let velocity = 0;

let gravity = 0.4;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(220);

    // Apply gravity

    velocity += gravity;

    // Update position

    y += velocity;

    // Ground collision

    if(y > height-25){

        y = height-25;

        velocity = 0;

    }

    // Ground

    stroke(0);

    line(0,height,width,height);

    // Ball

    noStroke();

    fill(255,80,80);

    circle(width/2,y,50);

    // Display information

    fill(0);

    textSize(18);

    text("Velocity : " + nf(velocity,1,2),20,30);

    text("Gravity : " + gravity,20,60);

}
```

---

# Program Output

Initially

```text
      ●
```

After a few frames

```text
      ●

       ↓
```

Later

```text
          ●

         ↓↓↓
```

Finally

```text
──────────────

      ●
```

The ball accelerates while falling and stops at the ground.

---

# Step-by-Step Code Explanation

## Step 1 — Initial Position

```javascript
let y = 50;
```

The ball starts near the top of the canvas.

---

## Step 2 — Velocity

```javascript
let velocity = 0;
```

Initially, the ball is not moving.

---

## Step 3 — Gravity

```javascript
let gravity = 0.4;
```

Gravity increases the downward speed every frame.

---

## Step 4 — Apply Gravity

```javascript
velocity += gravity;
```

Velocity becomes

```text
Frame 1

0.4

↓

Frame 2

0.8

↓

Frame 3

1.2

↓

Frame 4

1.6
```

The object falls faster and faster.

---

## Step 5 — Update Position

```javascript
y += velocity;
```

The ball moves downward based on its current velocity.

---

## Step 6 — Ground Collision

```javascript
if(y > height-25)
```

Checks whether the ball has reached the ground.

If true,

```javascript
velocity = 0;
```

stops the ball.

---

# Internal Working

Every frame,

```text
Gravity

↓

Velocity

↓

Position

↓

Draw Ball
```

This sequence repeats about 60 times every second.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| circle() | Draw the ball |
| line() | Draw the ground |
| background() | Refresh the canvas |
| text() | Display information |
| nf() | Format numeric output |

---

# Output Observation

✔ Slow movement at the beginning

✔ Increasing speed while falling

✔ Smooth animation

✔ Stops exactly at the ground

---

# Optimization Tips

### Tip 1

Keep gravity small.

Typical values:

```text
0.2

0.3

0.4

0.5
```

Large values make the object fall unrealistically fast.

---

### Tip 2

Separate

- Position
- Velocity
- Gravity

into different variables.

This makes the code easier to understand and modify.

---

### Tip 3

Always check for ground collision to prevent the object from falling outside the canvas.

---

# Common Mistakes

## Mistake 1

Updating position before velocity.

Incorrect

```javascript
y += velocity;

velocity += gravity;
```

Although the animation still works, the physics becomes less accurate.

---

## Mistake 2

Using

```javascript
velocity = gravity;
```

instead of

```javascript
velocity += gravity;
```

Velocity never increases.

---

## Mistake 3

Not checking ground collision.

The ball disappears below the canvas.

---

## Mistake 4

Using a very large gravity value.

The ball appears to teleport instead of falling smoothly.

---

# Challenge Exercises

### ⭐ Easy

Change the ball color.

---

### ⭐⭐ Medium

Increase gravity using a slider.

---

### ⭐⭐⭐ Hard

Press the **Spacebar** to reset the ball to the top.

---

### ⭐⭐⭐⭐ Expert

Create three balls with different gravity values.

Example

```text
Ball A

Gravity = 0.2

Ball B

Gravity = 0.4

Ball C

Gravity = 0.8
```

Observe how they fall at different rates.

---

# Viva Questions

### Q1

What is gravity?

**Answer**

Gravity is the force that pulls objects toward the Earth. In this program, it is simulated by increasing the object's downward velocity.

---

### Q2

What is velocity?

**Answer**

Velocity is the speed and direction of an object's movement.

---

### Q3

Why does the ball accelerate?

**Answer**

Because gravity increases the velocity every frame.

---

### Q4

Why is ground collision necessary?

**Answer**

To prevent the object from moving outside the visible canvas.

---

### Q5

Which variables control the falling motion?

**Answer**

- Position (`y`)
- Velocity (`velocity`)
- Gravity (`gravity`)

---

# 📌 Quick Revision

✅ Gravity

✅ Velocity

✅ Position

✅ Acceleration

✅ Ground Collision

✅ Physics Simulation

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Gravity Simulation

✔ Acceleration

✔ Velocity

✔ Free Fall

✔ Collision Detection

✔ Basic Game Physics

---

# 🚀 Next Experiment

## Problem 20 — Bouncing Balls with Friction

In the next experiment, you will learn how to simulate:

- ⚽ Bouncing Motion
- 🧲 Energy Loss
- 🪂 Friction
- 🔄 Repeated Collisions
- 🎮 Realistic Physics

These concepts form the basis of many modern game physics engines.

# 🌍 Part 5B — Visual Effects and Physics

---

# Problem 20

# Bouncing Ball with Friction and Realistic Collision

---

## 🎯 Objective

Create a p5.js program to simulate a bouncing ball affected by:

- 🌍 Gravity
- ⚽ Ground Collision
- 🧲 Friction (Energy Loss)

The ball should bounce repeatedly, with each bounce becoming smaller until it eventually comes to rest.

---

# 📖 Theory

In the real world, a ball does **not** bounce forever.

Whenever it hits the ground,

- Some energy is lost as heat.
- Some energy is lost as sound.
- Some energy is lost due to deformation.

This gradual loss of energy is represented in computer graphics using a **friction** (or restitution) coefficient.

---

# Real-Life Applications

This concept is used in:

- 🎮 Physics-based Games
- ⚽ Sports Simulators
- 🚗 Driving Simulations
- 🤖 Robotics
- 🎬 Animation Software
- 🛰 Physics Engines

Examples include:

- Angry Birds
- Cut the Rope
- Hill Climb Racing
- Unity Physics
- Box2D Physics Engine

---

# Understanding the Motion

Initially

```text
      ●

      ↓
```

After hitting the ground

```text
──────────────

      ●

      ↑
```

After each bounce

```text
High Bounce

↓

Medium Bounce

↓

Small Bounce

↓

Very Small Bounce

↓

Stops
```

---

# Physics Concept

The simulation uses three quantities:

### Position

```text
y
```

Current vertical location.

---

### Velocity

```text
velocity
```

Current speed of movement.

---

### Gravity

```text
gravity
```

Pulls the ball downward.

---

### Friction (Restitution)

```text
friction
```

Reduces the ball's speed after each bounce.

---

# Mathematical Model

Every frame

```text
Velocity

=

Velocity + Gravity
```

Position

```text
Position

=

Position + Velocity
```

When the ball hits the ground

```text
Velocity

=

Velocity × (-Friction)
```

Example

```text
Before Collision

Velocity = 12

↓

Friction = 0.80

↓

After Collision

Velocity = -9.6
```

The negative sign changes the direction upward.

---

# Collision Flow

```text
Falling

↓

Ground Collision

↓

Reverse Direction

↓

Reduce Speed

↓

Bounce

↓

Repeat
```

---

# Algorithm

```text
Start

↓

Create Ball

↓

Apply Gravity

↓

Update Position

↓

Touch Ground?

↓

Yes

↓

Reverse Velocity

↓

Multiply by Friction

↓

Repeat
```

---

# Source Code

```javascript
let y = 50;

let velocity = 0;

let gravity = 0.5;

let friction = 0.80;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(225);

    velocity += gravity;

    y += velocity;

    if(y >= height-25){

        y = height-25;

        velocity *= -friction;

        // Stop tiny bouncing

        if(abs(velocity) < 1){

            velocity = 0;

        }

    }

    // Ground

    stroke(0);

    strokeWeight(2);

    line(0,height,width,height);

    // Ball

    noStroke();

    fill(255,120,50);

    circle(width/2,y,50);

    // Information

    fill(0);

    textSize(18);

    text("Gravity : " + gravity,20,30);

    text("Friction : " + friction,20,60);

    text("Velocity : " + nf(velocity,1,2),20,90);

}
```

---

# Program Output

Beginning

```text
      ●
```

After first bounce

```text
────────────

      ●

      ↑
```

Second bounce

```text
────────────

      ●

     ↑
```

Final stage

```text
────────────

      ●
```

The bouncing gradually decreases until the ball stops.

---

# Step-by-Step Code Explanation

## Step 1

Apply gravity.

```javascript
velocity += gravity;
```

The downward speed increases every frame.

---

## Step 2

Move the ball.

```javascript
y += velocity;
```

Updates the vertical position.

---

## Step 3

Detect collision.

```javascript
if(y >= height-25)
```

Checks whether the ball has touched the ground.

---

## Step 4

Reverse direction.

```javascript
velocity *= -friction;
```

The negative sign

```text
↓

Changes

Downward

↓

Upward
```

The friction value

```text
↓

Reduces

Bounce Height
```

---

## Step 5

Stop tiny bouncing.

```javascript
if(abs(velocity)<1)
```

Very small movements are ignored.

This prevents endless tiny vibrations.

---

# Motion Illustration

```text
Bounce 1

      ●

↓

────────────

↑

      ●

↓

Bounce 2

    ●

↓

────────────

↑

    ●

↓

Bounce 3

  ●

↓

────────────

↑

  ●

↓

Stop
```

---

# Why Does the Bounce Become Smaller?

Every collision reduces velocity.

Example

```text
12

↓

9.6

↓

7.68

↓

6.14

↓

4.91

↓

3.93

↓

...
```

Eventually

```text
Velocity

↓

0
```

The ball stops.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| abs() | Absolute value |
| nf() | Number formatting |
| line() | Draw ground |
| circle() | Draw ball |
| background() | Refresh screen |

---

# Output Observation

✔ Ball falls naturally.

✔ Speed increases due to gravity.

✔ Ball bounces after collision.

✔ Bounce height decreases.

✔ Ball finally stops.

---

# Optimization Tips

### Tip 1

Keep friction between

```text
0.70

↓

0.95
```

Lower values lose energy quickly.

Higher values bounce longer.

---

### Tip 2

Use

```javascript
abs()
```

to detect very small velocities.

---

### Tip 3

Separate gravity and friction variables.

This makes the simulation easy to adjust.

---

# Common Mistakes

## Mistake 1

Using

```javascript
velocity = friction;
```

instead of

```javascript
velocity *= -friction;
```

The ball will not bounce correctly.

---

## Mistake 2

Forgetting the negative sign.

```javascript
velocity *= friction;
```

The ball continues moving downward.

---

## Mistake 3

Not checking

```javascript
abs(velocity)
```

The ball vibrates forever.

---

## Mistake 4

Using friction greater than

```text
1
```

The bounce becomes larger every time, which is unrealistic.

---

# Challenge Exercises

### ⭐ Easy

Change the ball color after every bounce.

---

### ⭐⭐ Medium

Allow the user to control gravity using a slider.

---

### ⭐⭐⭐ Hard

Create three bouncing balls with different friction values.

Example

```text
Ball A

0.60

↓

Stops Quickly

Ball B

0.80

↓

Normal Bounce

Ball C

0.95

↓

Bounces Many Times
```

---

### ⭐⭐⭐⭐ Expert

Add wall collisions so the ball bounces left, right, and downward.

---

# Comparison Table

| Without Friction | With Friction |
|------------------|---------------|
| Bounce forever | Bounce decreases |
| Unrealistic | Realistic |
| Constant energy | Energy loss |
| Simple animation | Physics simulation |

---

# Viva Questions

### Q1

Why does the ball bounce?

**Answer**

Because its velocity is reversed when it collides with the ground.

---

### Q2

Why is friction used?

**Answer**

To simulate energy loss during each collision, making the motion more realistic.

---

### Q3

Why do we multiply velocity by a negative value?

**Answer**

The negative sign changes the direction of motion, while the friction value reduces its magnitude.

---

### Q4

Why is `abs()` used?

**Answer**

It checks the magnitude of the velocity regardless of its direction, allowing the program to stop tiny oscillations.

---

### Q5

What happens if friction is equal to 1?

**Answer**

The ball keeps bouncing to approximately the same height (ignoring numerical errors), because no energy is lost.

---

# 📌 Quick Revision

✅ Gravity

✅ Velocity

✅ Friction

✅ Collision Detection

✅ Energy Loss

✅ Bouncing Motion

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Gravity Simulation

✔ Ground Collision

✔ Friction

✔ Velocity Reversal

✔ Energy Conservation and Loss

✔ Realistic Bouncing Motion

✔ Basic Physics Engine Concepts

---

# 🚀 Next Experiment

## Part 5C — Problem 21

### Explosion Effect Using Particles

In the next experiment, you will build an interactive **explosion effect** where:

- 💥 Clicking the mouse creates an explosion.
- ✨ Hundreds of particles burst outward.
- 🌈 Particles move in random directions.
- 👻 Particles gradually fade and disappear.

This combines everything learned in this chapter—particles, random motion, transparency, and animation—to create a professional visual effect commonly used in games and simulations.

# 💥 Part 5C — Visual Effects and Physics

---

# Problem 21

# Explosion Effect Using Particles

---

## 🎯 Objective

Create a p5.js program where clicking the mouse generates an explosion effect using multiple particles.

Each particle should:

- Move outward in random directions.
- Gradually slow down.
- Fade over time.
- Disappear after its lifetime ends.

---

# 📖 Theory

An explosion effect is created by releasing a large number of particles from a single point.

Unlike the particle trail in **Problem 17**, where particles continuously followed the mouse, an explosion creates **many particles at once**, moving rapidly away from the center.

This technique is commonly used in modern games and animations.

---

# Real-Life Applications

Explosion particle effects are used in:

- 🎮 Video Games
- 🎆 Fireworks
- 💥 Bomb Explosions
- ✨ Magic Spells
- ⚡ Energy Bursts
- 🚀 Rocket Launches
- 🎬 Movie Visual Effects

---

# Explosion Process

```text
Mouse Click

      │

      ▼

 Create Explosion

      │

      ▼

Generate Particles

      │

      ▼

Move Outward

      │

      ▼

Slow Down

      │

      ▼

Fade Away

      │

      ▼

Disappear
```

---

# Particle Explosion Diagram

```text
             *

        *    ↑    *

           ↖ | ↗

      * ←  ●  → *

           ↙ | ↘

        *    ↓    *
```

The center point is the explosion origin.

Each particle travels in a unique random direction.

---

# Physics Behind the Effect

Each particle has:

- Position `(x, y)`
- Velocity `(vx, vy)`
- Size
- Transparency (Alpha)
- Lifetime

Every frame:

```text
Position

↓

Position + Velocity
```

Velocity gradually decreases:

```text
Velocity

↓

Velocity × 0.98
```

Transparency decreases:

```text
Alpha

↓

Alpha - 4
```

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Wait for Mouse Click

↓

Create 100 Particles

↓

Move Particles

↓

Reduce Speed

↓

Reduce Alpha

↓

Remove Dead Particles

↓

Repeat
```

---

# Source Code

```javascript
let particles = [];

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(15);

    for(let i = particles.length-1; i >= 0; i--){

        particles[i].update();

        particles[i].display();

        if(particles[i].finished()){

            particles.splice(i,1);

        }

    }

    fill(255);

    textSize(18);

    text("Click Anywhere to Create Explosion",20,30);

}

function mousePressed(){

    for(let i=0;i<100;i++){

        particles.push(new Particle(mouseX,mouseY));

    }

}

class Particle{

    constructor(x,y){

        this.x = x;
        this.y = y;

        this.vx = random(-6,6);
        this.vy = random(-6,6);

        this.alpha = 255;

        this.size = random(4,10);

        this.r = random(255);
        this.g = random(255);
        this.b = random(255);

    }

    update(){

        this.x += this.vx;
        this.y += this.vy;

        this.vx *= 0.98;
        this.vy *= 0.98;

        this.alpha -= 4;

    }

    display(){

        noStroke();

        fill(this.r,this.g,this.b,this.alpha);

        circle(this.x,this.y,this.size);

    }

    finished(){

        return this.alpha <= 0;

    }

}
```

---

# Program Output

Clicking the mouse creates an explosion.

```text
Before

          ●

Click

↓

      *   ↑   *

   *   ↖ ● ↗   *

      ←     →

   *   ↙   ↘   *

      *   ↓   *
```

Particles spread in all directions.

After a few seconds,

they fade and disappear.

---

# Step-by-Step Code Explanation

## Step 1 — Store Particles

```javascript
let particles = [];
```

The array stores every particle currently visible.

---

## Step 2 — Mouse Click

```javascript
mousePressed()
```

Creates a new explosion.

---

## Step 3 — Generate 100 Particles

```javascript
for(let i=0;i<100;i++)
```

Each click creates 100 independent particles.

---

## Step 4 — Random Direction

```javascript
random(-6,6)
```

Assigns a different velocity to every particle.

```text
↖

↑

↗

←

→

↙

↓

↘
```

---

## Step 5 — Slow Down

```javascript
this.vx *= 0.98;

this.vy *= 0.98;
```

Simulates air resistance.

Particles gradually lose speed.

---

## Step 6 — Fade

```javascript
this.alpha -= 4;
```

Particles slowly become transparent.

---

## Step 7 — Remove

```javascript
particles.splice(i,1);
```

Deletes invisible particles.

---

# Internal Working

```text
Mouse Click

↓

100 New Particles

↓

Random Velocity

↓

Move

↓

Slow Down

↓

Fade

↓

Delete
```

This cycle repeats for every explosion.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| mousePressed() | Detect mouse click |
| random() | Random velocity and color |
| push() | Add particles |
| splice() | Remove particles |
| fill() | Apply RGBA color |
| noStroke() | Remove outlines |

---

# Why Use Classes?

Instead of managing hundreds of variables manually,

the `Particle` class groups related properties and behavior into a single object.

Benefits:

- Cleaner code
- Easy to reuse
- Easier debugging
- Better organization

---

# Output Observation

✔ Explosion starts instantly.

✔ Particles move independently.

✔ Speed gradually decreases.

✔ Colors remain different.

✔ Particles fade smoothly.

✔ Explosion disappears naturally.

---

# Optimization Tips

### Tip 1

Use 50–150 particles for smooth performance.

Too many particles may reduce frame rate.

---

### Tip 2

Always remove finished particles.

Otherwise, memory usage continuously increases.

---

### Tip 3

Reduce particle size for faster rendering.

---

### Tip 4

Use backward iteration while deleting particles.

```javascript
for(let i=particles.length-1;i>=0;i--)
```

This avoids skipping elements.

---

# Common Mistakes

## Mistake 1

Looping forward while deleting particles.

Result:

Some particles remain undeleted.

---

## Mistake 2

Not decreasing alpha.

Particles never disappear.

---

## Mistake 3

Using identical velocity.

All particles move together instead of spreading.

---

## Mistake 4

Creating particles inside `setup()`.

Only one explosion appears.

---

## Mistake 5

Using too many particles (e.g., 1000+).

Performance decreases significantly.

---

# Challenge Exercises

### ⭐ Easy

Increase the explosion size.

Create 200 particles instead of 100.

---

### ⭐⭐ Medium

Make particles change color while fading.

---

### ⭐⭐⭐ Hard

Play an explosion sound when the mouse is clicked.

(Hint: Use `loadSound()` and `play()` from the p5.sound library.)

---

### ⭐⭐⭐⭐ Expert

Create a **firework animation**:

1. Launch a particle upward.
2. At its highest point, trigger an explosion.
3. Repeat automatically.

---

# Comparison

| Problem 17 | Problem 21 |
|------------|------------|
| Continuous particle trail | Instant explosion |
| One particle per frame | Many particles at once |
| Mouse movement | Mouse click |
| Gentle motion | Rapid outward motion |
| Trail effect | Explosion effect |

---

# Viva Questions

### Q1

What is a particle explosion?

**Answer**

It is a visual effect created by generating many particles that move outward from a single point.

---

### Q2

Why do particles move in different directions?

**Answer**

Each particle receives a random velocity, making the explosion appear natural.

---

### Q3

Why do particles slow down?

**Answer**

Velocity is multiplied by a value less than 1, simulating air resistance or energy loss.

---

### Q4

Why is transparency reduced?

**Answer**

It allows particles to fade smoothly instead of disappearing suddenly.

---

### Q5

Why do we remove finished particles?

**Answer**

To free memory and maintain good performance.

---

# 📌 Quick Revision

✅ Particle System

✅ Mouse Interaction

✅ Random Velocity

✅ Air Resistance

✅ Transparency

✅ Arrays of Objects

✅ Classes

---

# 📚 Chapter 5 Summary

After completing Problems **17–21**, you should understand:

✔ Particle Systems

✔ Random Motion

✔ Glow & Pulsing Effects

✔ Gravity

✔ Velocity

✔ Friction

✔ Collision Detection

✔ Explosion Effects

✔ Physics-Based Animation

✔ Object-Oriented Programming in p5.js

These concepts form the foundation of many modern games, simulations, and interactive graphics applications.

---

# 🚀 Next Chapter

# 🎵 Part 6 — Sound and Audio (Problems 22–24)

In the next chapter, you will learn how to:

- 🎹 Play sounds using keyboard input.
- 🎤 Capture live microphone input.
- 📊 Create audio-reactive visualizations.
- 🌈 Animate graphics based on sound intensity.

This introduces multimedia programming and interactive audio in p5.js.

# 🎵 Part 6A — Sound and Audio

---

# Chapter 6: Sound and Audio

## Introduction

Modern multimedia applications are not limited to graphics alone. Sound plays a vital role in creating interactive and engaging experiences.

Using the **p5.sound** library, we can:

- 🎹 Play sound files
- 🎤 Capture microphone input
- 📊 Analyze sound intensity
- 🎵 Create music visualizations
- 🎮 Add sound effects to games

In this chapter, we will learn how graphics and audio work together.

---

# Before You Start

## Include the p5.sound Library

If you are using the **p5.js Web Editor**, the library is already available.

If you are using **VS Code** or a local project, include:

```html
<script src="p5.min.js"></script>
<script src="p5.sound.min.js"></script>
<script src="sketch.js"></script>
```

Without **p5.sound**, audio functions such as `loadSound()` and `AudioIn()` will not work.

---

# Problem 22

# Play Different Sounds Using Keyboard Keys

---

## 🎯 Objective

Create a p5.js program that plays different sound effects when specific keyboard keys are pressed.

Example:

- **A** → Sound 1
- **S** → Sound 2
- **D** → Sound 3

---

# 📖 Theory

Sound files can be loaded into memory before the program starts.

Whenever the user presses a key, the corresponding sound is played.

This technique is commonly used in:

- 🎹 Virtual Piano
- 🎮 Video Games
- 🎧 Music Applications
- 🎤 Drum Machines
- 📚 Educational Software

---

# Sound Interaction Flow

```text
Keyboard Press

      │

      ▼

Detect Key

      │

      ▼

Play Sound

      │

      ▼

Wait for Next Input
```

---

# Required Audio Files

Create an **assets** folder and place three sound files inside it.

```text
project/

│

├── index.html

├── sketch.js

└── assets/

      ├── sound1.mp3

      ├── sound2.mp3

      └── sound3.mp3
```

---

# Algorithm

```text
Start

↓

Load Sounds

↓

Create Canvas

↓

Wait for Key Press

↓

Detect Pressed Key

↓

Play Matching Sound

↓

Repeat
```

---

# Source Code

```javascript
let sound1;
let sound2;
let sound3;

function preload(){

    sound1 = loadSound("assets/sound1.mp3");

    sound2 = loadSound("assets/sound2.mp3");

    sound3 = loadSound("assets/sound3.mp3");

}

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(220);

    textSize(22);

    fill(0);

    text("Press A, S or D to Play Sounds",120,200);

}

function keyPressed(){

    if(key == 'A' || key == 'a'){

        sound1.play();

    }

    if(key == 'S' || key == 's'){

        sound2.play();

    }

    if(key == 'D' || key == 'd'){

        sound3.play();

    }

}
```

---

# Program Output

```text
Press A

↓

🔊 Sound 1

----------------

Press S

↓

🔊 Sound 2

----------------

Press D

↓

🔊 Sound 3
```

---

# Step-by-Step Code Explanation

## Step 1

Load sound files.

```javascript
preload()
```

This function loads all assets before the sketch starts.

---

## Step 2

Load each audio file.

```javascript
loadSound()
```

Example:

```javascript
sound1 = loadSound("assets/sound1.mp3");
```

---

## Step 3

Detect keyboard input.

```javascript
keyPressed()
```

Runs once whenever a key is pressed.

---

## Step 4

Play the sound.

```javascript
sound1.play();
```

The selected sound starts playing immediately.

---

# Understanding preload()

```text
Program Starts

↓

preload()

↓

Load Images

↓

Load Sounds

↓

setup()

↓

draw()
```

Using `preload()` ensures all files are available before the program begins.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| preload() | Load assets before execution |
| loadSound() | Load an audio file |
| play() | Play the sound |
| keyPressed() | Detect key press |

---

# Output Observation

✔ Different keys trigger different sounds.

✔ Sounds play immediately.

✔ Keyboard interaction controls audio playback.

---

# Optimization Tips

### Tip 1

Keep sound files short for faster loading.

---

### Tip 2

Store all sounds in an **assets** folder.

---

### Tip 3

Use meaningful filenames.

Example:

```text
jump.mp3

coin.mp3

explosion.mp3
```

instead of

```text
audio1.mp3
```

---

# Common Mistakes

## Mistake 1

Forgetting to include **p5.sound.min.js**.

Result:

```
loadSound is not defined
```

---

## Mistake 2

Using the wrong file path.

Incorrect:

```javascript
loadSound("sound1.mp3");
```

Correct:

```javascript
loadSound("assets/sound1.mp3");
```

(if the file is inside the `assets` folder)

---

## Mistake 3

Calling

```javascript
play()
```

before the sound is loaded.

Always load sounds inside `preload()`.

---

## Mistake 4

Using

```javascript
keyIsDown()
```

instead of

```javascript
keyPressed()
```

The sound may restart continuously while the key is held.

---

# Challenge Exercises

### ⭐ Easy

Add two more keyboard keys.

---

### ⭐⭐ Medium

Display the name of the sound currently playing.

---

### ⭐⭐⭐ Hard

Control sound volume using a slider.

(Hint: Use `setVolume()`.)

---

### ⭐⭐⭐⭐ Expert

Create a mini virtual piano using the keys:

```text
A S D F G H J
```

Each key should play a different musical note.

---

# Viva Questions

### Q1

Why is `preload()` used?

**Answer**

It ensures that sound files are completely loaded before the program starts.

---

### Q2

What does `loadSound()` do?

**Answer**

It loads an audio file into memory so it can be played later.

---

### Q3

What is the purpose of `play()`?

**Answer**

It starts playing the loaded sound.

---

### Q4

Why should audio files be stored in an `assets` folder?

**Answer**

It keeps the project organized and makes file paths easier to manage.

---

### Q5

Which library is required for audio in p5.js?

**Answer**

The **p5.sound** library.

---

# 📌 Quick Revision

✅ preload()

✅ loadSound()

✅ play()

✅ keyPressed()

✅ Audio Assets

✅ Keyboard Interaction

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Loading Sound Files

✔ Audio Playback

✔ Keyboard-Controlled Audio

✔ Asset Management

✔ p5.sound Library

---

# 🚀 Next Experiment

## Problem 23 — Audio-Reactive Visualization

In the next experiment, you will use:

- 🎤 Live Microphone Input
- 📈 Sound Amplitude
- 📊 Real-Time Audio Analysis
- 🎨 Dynamic Visual Effects

to create graphics that respond to your voice and surrounding sounds.

# 🎵 Part 6B — Sound and Audio

---

# Problem 23

# Audio-Reactive Visualization Using Microphone Input

---

## 🎯 Objective

Create a p5.js program that uses the computer's **microphone input** to generate a real-time visualization.

The visualization should change according to the loudness of the surrounding sound or the user's voice.

---

# 📖 Theory

Audio-reactive visualization is a technique where graphics respond to sound.

Instead of controlling animation with the keyboard or mouse, the program continuously analyzes the microphone input and converts sound into visual effects.

The louder the sound, the larger or brighter the graphics become.

---

# Real-Life Applications

Audio visualization is used in:

- 🎵 Music Players
- 🎧 Spotify Visualizers
- 🎤 Voice Assistants
- 📺 Audio Spectrum Displays
- 🎮 Rhythm Games
- 🎬 Live Concert Effects
- 📊 Sound Analysis Software

---

# Sound Processing Flow

```text
Microphone

      │

      ▼

Capture Audio

      │

      ▼

Measure Amplitude

      │

      ▼

Convert to Graphics

      │

      ▼

Display Animation
```

---

# What is Amplitude?

Amplitude represents the **loudness** of a sound.

```text
Quiet Voice

Amplitude

↓

0.05

------------------------

Normal Voice

↓

0.20

------------------------

Loud Voice

↓

0.60

------------------------

Very Loud

↓

1.00
```

In p5.js,

```javascript
mic.getLevel()
```

returns a value between

```text
0

↓

1
```

---

# Microphone Permission

When the program starts,

your browser will display a message similar to:

```text
Allow this site to use your microphone?

[ Allow ]

[ Block ]
```

Select **Allow**.

Otherwise,

the microphone cannot capture sound.

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Start Microphone

↓

Read Audio Level

↓

Convert Level to Size

↓

Draw Circle

↓

Repeat
```

---

# Source Code

```javascript
let mic;

function setup(){

    createCanvas(700,400);

    mic = new p5.AudioIn();

    mic.start();

}

function draw(){

    background(20);

    let level = mic.getLevel();

    let size = map(level,0,1,50,300);

    fill(0,180,255);

    noStroke();

    circle(width/2,height/2,size);

    fill(255);

    textSize(18);

    text("Microphone Level : " + nf(level,1,3),20,30);

}
```

---

# Program Output

No Sound

```text
      ●
```

Speak Normally

```text
        ⬤
```

Speak Loudly

```text
           ⬤
```

The louder the sound,

the larger the circle becomes.

---

# Step-by-Step Code Explanation

## Step 1 — Create Microphone Object

```javascript
mic = new p5.AudioIn();
```

This creates an audio input object.

---

## Step 2 — Start Microphone

```javascript
mic.start();
```

Requests microphone permission and begins capturing sound.

---

## Step 3 — Measure Loudness

```javascript
let level = mic.getLevel();
```

Returns the current microphone amplitude.

Example values:

```text
Silent

↓

0.01

Speaking

↓

0.20

Shouting

↓

0.75
```

---

## Step 4 — Convert Amplitude

```javascript
map(level,0,1,50,300)
```

Converts

```text
0 → 50

1 → 300
```

making the circle easier to see.

---

## Step 5 — Draw Circle

```javascript
circle(width/2,height/2,size);
```

The diameter changes according to microphone input.

---

# Internal Working

```text
Voice

↓

Microphone

↓

Amplitude

↓

map()

↓

Circle Size

↓

Display
```

This process repeats approximately 60 times every second.

---

# Visual Representation

```text
Quiet

      ○

↓

Speaking

      ◉

↓

Loud

      ⬤
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| p5.AudioIn() | Create microphone object |
| start() | Activate microphone |
| getLevel() | Read microphone amplitude |
| map() | Convert values |
| circle() | Draw visualization |

---

# Output Observation

✔ Circle grows when sound becomes louder.

✔ Circle shrinks when the environment becomes quieter.

✔ Visualization updates continuously in real time.

---

# Optimization Tips

### Tip 1

Always allow microphone permission.

Otherwise,

`getLevel()` returns nearly zero.

---

### Tip 2

Use `map()` to convert the small amplitude values into a visible animation.

---

### Tip 3

Speak close to the microphone for clearer results.

---

### Tip 4

Test in a quiet room to observe changes more accurately.

---

# Common Mistakes

## Mistake 1

Forgetting

```javascript
mic.start();
```

The microphone never begins recording.

---

## Mistake 2

Blocking microphone permission.

No audio data is received.

---

## Mistake 3

Drawing directly with

```javascript
level
```

instead of

```javascript
map(level,...)
```

The size changes are almost invisible.

---

## Mistake 4

Not including

```text
p5.sound.min.js
```

Audio functions will not work.

---

# Challenge Exercises

### ⭐ Easy

Change the circle color based on microphone level.

---

### ⭐⭐ Medium

Use a rectangle instead of a circle.

---

### ⭐⭐⭐ Hard

Display five circles whose sizes all depend on the microphone level.

---

### ⭐⭐⭐⭐ Expert

Create a microphone-controlled equalizer with multiple animated bars.

---

# Viva Questions

### Q1

What does `p5.AudioIn()` do?

**Answer**

It creates a microphone input object that captures live audio.

---

### Q2

Why is `mic.start()` necessary?

**Answer**

It activates the microphone and requests permission from the browser.

---

### Q3

What does `getLevel()` return?

**Answer**

It returns the current sound amplitude, usually between **0** and **1**.

---

### Q4

Why do we use `map()`?

**Answer**

Because microphone amplitude values are very small. `map()` converts them into a useful range for graphics.

---

### Q5

Give two applications of audio-reactive visualization.

**Answer**

- Music visualizers
- Live concert lighting

(Other examples include voice-controlled interfaces and rhythm games.)

---

# 📌 Quick Revision

✅ p5.AudioIn()

✅ mic.start()

✅ getLevel()

✅ map()

✅ Microphone Input

✅ Audio Visualization

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Live Audio Capture

✔ Microphone Input

✔ Sound Amplitude

✔ Audio-Reactive Graphics

✔ Real-Time Visualization

---

# 🚀 Next Experiment

## Problem 24 — Animation Based on Sound Intensity

In the next experiment, you will combine animation and audio by making multiple graphical objects change their:

- 🌈 Color
- 📏 Size
- ⚡ Speed

according to sound intensity, creating a dynamic multimedia visualization.

# 🎵 Part 6C — Sound and Audio

---

# Problem 24

# Dynamic Animation Based on Sound Intensity

---

## 🎯 Objective

Create a p5.js program where an animation dynamically changes according to the intensity of sound captured by the microphone.

The program should demonstrate how sound can control:

- 🌈 Color
- 📏 Size
- ⚡ Animation Speed

in real time.

---

# 📖 Theory

In **Problem 23**, microphone input controlled only the size of a single object.

In this experiment, the microphone controls **multiple visual properties simultaneously**, making the animation more dynamic and interactive.

This technique is widely used in:

- 🎵 Music Visualizers
- 🎤 Live Concert Effects
- 🎮 Rhythm Games
- 📺 Multimedia Installations
- 🎬 Motion Graphics

---

# How It Works

The microphone continuously measures sound intensity.

```text
Microphone

↓

Amplitude

↓

Animation Properties

↓

Display Graphics
```

The louder the sound,

the larger, brighter, and faster the animation becomes.

---

# Sound Intensity Scale

```text
Silence

↓

0.00

↓

Soft Voice

↓

0.10

↓

Normal Voice

↓

0.30

↓

Loud Voice

↓

0.70

↓

Very Loud

↓

1.00
```

---

# Animation Flow

```text
Capture Sound

↓

Measure Amplitude

↓

Map to Size

↓

Map to Color

↓

Map to Rotation Speed

↓

Draw Animation

↓

Repeat
```

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Initialize Microphone

↓

Read Sound Level

↓

Convert Values

↓

Draw Animated Object

↓

Repeat
```

---

# Source Code

```javascript
let mic;
let angle = 0;

function setup(){

    createCanvas(700,400);

    mic = new p5.AudioIn();

    mic.start();

}

function draw(){

    background(20);

    let level = mic.getLevel();

    let size = map(level,0,1,60,220);

    let redValue = map(level,0,1,50,255);

    let speed = map(level,0,1,0.02,0.20);

    angle += speed;

    translate(width/2,height/2);

    rotate(angle);

    noStroke();

    fill(redValue,150,255);

    rectMode(CENTER);

    rect(0,0,size,size);

    resetMatrix();

    fill(255);

    textSize(18);

    text("Sound Level : " + nf(level,1,3),20,30);

    text("Rotation Speed : " + nf(speed,1,3),20,60);

}
```

---

# Program Output

Quiet Environment

```text
      □
```

Speaking

```text
        ◇
```

Loud Voice

```text
          ◆
```

The square:

- Rotates faster.
- Becomes larger.
- Changes color.

---

# Step-by-Step Code Explanation

## Step 1 — Create Microphone

```javascript
mic = new p5.AudioIn();
```

Creates the microphone object.

---

## Step 2 — Start Recording

```javascript
mic.start();
```

Begins capturing live sound.

---

## Step 3 — Read Sound Level

```javascript
let level = mic.getLevel();
```

Returns the current sound intensity.

---

## Step 4 — Convert Values

### Size

```javascript
map(level,0,1,60,220)
```

Converts sound into object size.

---

### Color

```javascript
map(level,0,1,50,255)
```

Converts sound into color intensity.

---

### Rotation Speed

```javascript
map(level,0,1,0.02,0.20)
```

Louder sound means faster rotation.

---

## Step 5 — Rotate Object

```javascript
angle += speed;
```

The rotation speed changes continuously based on sound.

---

## Step 6 — Draw the Square

```javascript
translate(width/2,height/2);

rotate(angle);

rect(0,0,size,size);
```

The square rotates around the center of the canvas.

---

# Internal Working

```text
Voice

↓

Microphone

↓

Amplitude

↓

map()

↓

Size

↓

Color

↓

Speed

↓

Animation
```

This sequence repeats continuously during execution.

---

# Visual Representation

```text
Quiet

     □

↓

Normal Voice

     ◇

↓

Loud Voice

     ◆
```

The animation becomes more energetic as the sound level increases.

---

# Important Functions

| Function | Purpose |
|----------|----------|
| p5.AudioIn() | Create microphone input |
| getLevel() | Measure sound intensity |
| map() | Convert value ranges |
| rotate() | Rotate object |
| translate() | Move origin |
| resetMatrix() | Restore default coordinate system |

---

# Output Observation

✔ Louder sounds increase object size.

✔ Color becomes brighter with higher intensity.

✔ Rotation speed changes dynamically.

✔ Animation responds instantly to microphone input.

---

# Optimization Tips

### Tip 1

Use small speed values.

Example:

```text
0.02

↓

0.20
```

Large values rotate too quickly.

---

### Tip 2

Use `map()` for all animation properties.

This provides smooth transitions.

---

### Tip 3

Keep the microphone close for better responsiveness.

---

### Tip 4

Experiment with different shapes.

Examples:

- Circle
- Triangle
- Star
- Polygon

---

# Common Mistakes

## Mistake 1

Not calling

```javascript
resetMatrix();
```

Text and other drawings may also rotate unexpectedly.

---

## Mistake 2

Using

```javascript
rotate(level);
```

The rotation becomes almost unnoticeable because the sound level is too small.

---

## Mistake 3

Forgetting to start the microphone.

```javascript
mic.start();
```

No sound data is received.

---

## Mistake 4

Omitting the p5.sound library.

Audio functions become unavailable.

---

# Challenge Exercises

### ⭐ Easy

Change the background color based on sound intensity.

---

### ⭐⭐ Medium

Animate three rotating squares with different speeds.

---

### ⭐⭐⭐ Hard

Create a microphone-controlled solar system where planets rotate faster as the sound becomes louder.

---

### ⭐⭐⭐⭐ Expert

Build a complete music visualizer with:

- Multiple rotating shapes
- Dynamic colors
- Pulsing circles
- Background glow
- Animated particles

---

# Comparison of Sound Experiments

| Problem | Main Concept |
|---------|--------------|
| **22** | Keyboard-controlled sound playback |
| **23** | Microphone-controlled visualization |
| **24** | Animation driven by sound intensity |

---

# Viva Questions

### Q1

What is sound intensity?

**Answer**

Sound intensity represents the loudness of a sound, measured in this program using the microphone's amplitude.

---

### Q2

Why is `map()` used repeatedly?

**Answer**

Because the microphone returns values between **0** and **1**, while animation properties require larger ranges.

---

### Q3

Why do we use `translate()` before `rotate()`?

**Answer**

To move the origin to the center of the canvas so the object rotates around its own center.

---

### Q4

What is the purpose of `resetMatrix()`?

**Answer**

It restores the default coordinate system, preventing subsequent drawings from inheriting the previous transformations.

---

### Q5

Name two real-world applications of sound-reactive animation.

**Answer**

- Music visualizers
- Concert lighting systems

(Other examples include interactive art installations and rhythm-based games.)

---

# 📌 Quick Revision

✅ p5.AudioIn()

✅ getLevel()

✅ map()

✅ translate()

✅ rotate()

✅ resetMatrix()

✅ Audio-Driven Animation

---

# 📚 Chapter 6 Summary

After completing Problems **22–24**, you should understand:

✔ Audio Playback

✔ Keyboard-Controlled Sound

✔ Microphone Input

✔ Sound Amplitude

✔ Audio-Reactive Visualization

✔ Dynamic Animation

✔ Multimedia Programming with p5.js

These concepts enable the creation of interactive applications that combine graphics, animation, and sound.

---

# 🚀 Next Chapter

# 🎮 Part 7 — Game Development (Problems 25–27)

In the final chapter, you will build complete interactive games by combining everything learned throughout this codebook:

- 🎯 Object Movement
- ⚽ Collision Detection
- ⌨️ Keyboard Controls
- 🖱️ Mouse Interaction
- 📊 Score Management
- 💥 Animation
- 🎵 Sound Effects (Optional)

You will create:

- **Problem 25:** Catch-the-Object Game
- **Problem 26:** Pong Game
- **Problem 27:** Shooting Game

This chapter brings together graphics, animation, physics, interactivity, and sound to develop complete games using p5.js.

# 🎮 Part 7A — Game Development

---

# Chapter 7: Game Development

## Introduction

Game development combines multiple concepts of computer graphics and programming to create interactive applications.

Throughout the previous chapters, you learned:

- Basic Drawing
- Animation
- Transformations
- Mouse & Keyboard Interaction
- Particle Systems
- Physics
- Sound

In this chapter, all of these concepts are combined to build simple yet complete games.

The main concepts covered are:

- 🎮 Player Control
- ⚽ Collision Detection
- 📊 Score System
- ❤️ Game Logic
- ⌨️ Keyboard Input
- 🎯 Object Interaction

---

# Problem 25

# Catch-the-Object Game

---

## 🎯 Objective

Create a game where the player controls a basket using the keyboard.

A ball continuously falls from the top of the screen.

The objective is to catch the falling ball to increase the score.

---

# 📖 Theory

A catch game consists of three main components.

1. Player
2. Falling Object
3. Score

The falling object continuously moves downward.

If the object touches the player,

✔ Score increases.

Otherwise,

the object simply restarts from the top.

---

# Real-Life Applications

The same game mechanics are used in

- 🍎 Fruit Catch Games
- 🎁 Gift Catch Games
- 💰 Coin Collection Games
- 🧸 Arcade Games
- 📱 Mobile Games

---

# Game Flow

```text
Start

↓

Create Player

↓

Create Falling Object

↓

Move Object

↓

Move Player

↓

Collision?

↓

Yes

↓

Increase Score

↓

Restart Object

↓

Repeat
```

---

# Collision Detection

The object is caught when

```text
Ball

↓

Touches

↓

Basket
```

In code,

```text
Distance

↓

Less Than

↓

Threshold
```

---

# Algorithm

```text
Start

↓

Create Canvas

↓

Initialize Basket

↓

Initialize Ball

↓

Move Ball

↓

Move Basket

↓

Check Collision

↓

Update Score

↓

Repeat
```

---

# Source Code

```javascript
let basketX = 350;

let ballX;

let ballY = 0;

let score = 0;

function setup(){

    createCanvas(700,400);

    ballX = random(width);

}

function draw(){

    background(220);

    // Basket

    rectMode(CENTER);

    fill(50,120,255);

    rect(basketX,height-20,100,20);

    // Move basket

    if(keyIsDown(LEFT_ARROW))

        basketX -= 6;

    if(keyIsDown(RIGHT_ARROW))

        basketX += 6;

    basketX = constrain(basketX,50,width-50);

    // Ball

    fill(255,80,80);

    circle(ballX,ballY,30);

    ballY += 4;

    // Collision

    if(dist(ballX,ballY,basketX,height-20) < 55){

        score++;

        ballY = 0;

        ballX = random(width);

    }

    // Miss

    if(ballY > height){

        ballY = 0;

        ballX = random(width);

    }

    // Score

    fill(0);

    textSize(22);

    text("Score : " + score,20,30);

}
```

---

# Program Output

```text
Score : 4

          ●

          ↓

──────────────────

      ███████
```

Move the basket using the **Left** and **Right** arrow keys to catch the falling ball.

---

# Step-by-Step Code Explanation

## Step 1

Create the basket.

```javascript
rect()
```

The basket stays near the bottom of the screen.

---

## Step 2

Move the basket.

```javascript
keyIsDown()
```

Arrow keys control the basket.

---

## Step 3

Move the ball.

```javascript
ballY += 4;
```

The ball falls continuously.

---

## Step 4

Check collision.

```javascript
dist(...)
```

Measures the distance between the basket and the ball.

If the distance is small enough,

the ball is considered caught.

---

## Step 5

Increase score.

```javascript
score++;
```

Each successful catch earns one point.

---

## Step 6

Restart the ball.

```javascript
ballY = 0;

ballX = random(width);
```

The ball starts falling again from a random horizontal position.

---

# Internal Working

```text
Ball Falls

↓

Player Moves

↓

Collision

↓

Score Update

↓

Restart Ball
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| random() | Random ball position |
| keyIsDown() | Keyboard movement |
| dist() | Collision detection |
| constrain() | Keep basket inside canvas |
| text() | Display score |

---

# Output Observation

✔ Ball falls continuously.

✔ Basket moves smoothly.

✔ Collision increases score.

✔ Missed balls restart automatically.

---

# Optimization Tips

### Tip 1

Use `constrain()` to prevent the basket from leaving the screen.

---

### Tip 2

Increase ball speed gradually to make the game more challenging.

Example

```javascript
ballSpeed += 0.1;
```

after every few successful catches.

---

### Tip 3

Separate game logic into functions if the game becomes larger.

---

# Common Mistakes

## Mistake 1

Forgetting to reset the ball after a catch.

The score increases continuously.

---

## Mistake 2

Not constraining the basket.

It moves outside the canvas.

---

## Mistake 3

Using a collision threshold that is too small.

The ball appears to pass through the basket.

---

## Mistake 4

Resetting only `ballY` and not `ballX`.

The ball always falls from the same position.

---

# Challenge Exercises

### ⭐ Easy

Change the basket color.

---

### ⭐⭐ Medium

Increase ball speed every five points.

---

### ⭐⭐⭐ Hard

Add three lives.

The game ends when all lives are lost.

---

### ⭐⭐⭐⭐ Expert

Create multiple falling objects with different colors and scores.

Example:

- 🍎 Apple = +1
- ⭐ Star = +5
- 💣 Bomb = −3

---

# Viva Questions

### Q1

What is the objective of this game?

**Answer**

To catch the falling object and increase the score.

---

### Q2

Which function detects the collision?

**Answer**

The `dist()` function.

---

### Q3

Why is `random()` used?

**Answer**

To generate a different horizontal position each time the ball restarts.

---

### Q4

Why is `constrain()` used?

**Answer**

To keep the basket within the canvas boundaries.

---

### Q5

How can the game be made more difficult?

**Answer**

By increasing the falling speed, adding multiple objects, reducing basket size, or introducing obstacles.

---

# 📌 Quick Revision

✅ Keyboard Input

✅ Object Movement

✅ Collision Detection

✅ Random Position

✅ Score System

✅ Simple Game Logic

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Basic Game Structure

✔ Player Movement

✔ Collision Detection

✔ Score Management

✔ Random Object Generation

✔ Interactive Gameplay

---

# 🚀 Next Experiment

## Problem 26 — Pong Game

In the next experiment, you will build a complete **Pong-style game** featuring:

- 🏓 Paddle Control
- ⚽ Ball Movement
- 💥 Wall & Paddle Collision
- 📊 Score Tracking
- 🎮 Continuous Gameplay

This introduces one of the most iconic games in video game history and demonstrates the core mechanics behind many arcade games.

# 🎮 Part 7B — Game Development

---

# Problem 26

# Pong Game with Paddle Control, Ball Movement, Collision Detection, and Scoring

---

## 🎯 Objective

Develop a simple Pong-style game where:

- The player controls a paddle using the keyboard.
- A ball continuously moves across the screen.
- The ball bounces off the top, bottom, and paddle.
- Missing the ball increases the opponent's score.
- The game continues indefinitely.

---

# 📖 Theory

Pong is one of the earliest arcade games ever created.

It demonstrates several important concepts of computer graphics and game programming:

- Object Animation
- Keyboard Interaction
- Collision Detection
- Boundary Checking
- Score Management

Unlike previous experiments, this game continuously updates multiple objects at the same time.

---

# Historical Background

Pong was released by **Atari** in **1972** and became one of the first commercially successful video games.

Although the game is simple, many modern sports and arcade games use the same core mechanics.

---

# Real-Life Applications

The techniques learned in this experiment are used in:

- 🏓 Sports Games
- 🎮 Arcade Games
- 🤖 AI Opponent Programming
- ⚽ Ball Physics
- 🧩 Puzzle Games
- 🕹 Multiplayer Games

---

# Game Components

```text
Player Paddle

      █

Ball

      ●

Opponent Wall

│

Playing Area

──────────────
```

---

# Game Flow

```text
Start Game

↓

Move Ball

↓

Move Paddle

↓

Collision?

↓

Yes

↓

Reverse Ball Direction

↓

Continue

↓

No

↓

Ball Leaves Screen

↓

Increase Score

↓

Reset Ball

↓

Repeat
```

---

# Collision Logic

```text
Ball

↓

Touches Paddle

↓

Reverse X Velocity

↓

Continue Moving
```

If the ball misses the paddle,

```text
Opponent Score

↓

+1

↓

Ball Reset
```

---

# Algorithm

```text
Start

↓

Create Paddle

↓

Create Ball

↓

Move Ball

↓

Move Paddle

↓

Check Wall Collision

↓

Check Paddle Collision

↓

Check Score

↓

Repeat
```

---

# Source Code

```javascript
let paddleY = 150;

let ballX = 350;
let ballY = 200;

let ballSpeedX = 5;
let ballSpeedY = 4;

let score = 0;

function setup(){

    createCanvas(700,400);

}

function draw(){

    background(30);

    // Paddle

    fill(0,200,255);

    rect(20,paddleY,15,100);

    // Paddle Movement

    if(keyIsDown(UP_ARROW))

        paddleY -= 6;

    if(keyIsDown(DOWN_ARROW))

        paddleY += 6;

    paddleY = constrain(paddleY,0,height-100);

    // Ball

    fill(255);

    circle(ballX,ballY,20);

    ballX += ballSpeedX;

    ballY += ballSpeedY;

    // Top and Bottom Collision

    if(ballY < 10 || ballY > height-10){

        ballSpeedY *= -1;

    }

    // Paddle Collision

    if(ballX < 35 &&
       ballY > paddleY &&
       ballY < paddleY+100){

        ballSpeedX *= -1;

    }

    // Right Wall

    if(ballX > width-10){

        ballSpeedX *= -1;

    }

    // Missed Ball

    if(ballX < 0){

        score++;

        ballX = width/2;

        ballY = height/2;

        ballSpeedX = 5;

        ballSpeedY = random(-4,4);

    }

    // Score

    fill(255);

    textSize(24);

    text("Opponent Score : " + score,420,30);

}
```

---

# Program Output

```text
Opponent Score : 2


█

          ●

────────────────────────────
```

Use the **↑** and **↓** arrow keys to move the paddle and prevent the ball from passing.

---

# Step-by-Step Code Explanation

## Step 1 — Create Paddle

```javascript
rect(20,paddleY,15,100);
```

Draws the player's paddle on the left side.

---

## Step 2 — Keyboard Control

```javascript
keyIsDown(UP_ARROW)

keyIsDown(DOWN_ARROW)
```

Moves the paddle vertically.

---

## Step 3 — Move the Ball

```javascript
ballX += ballSpeedX;

ballY += ballSpeedY;
```

Updates the ball position every frame.

---

## Step 4 — Wall Collision

```javascript
ballSpeedY *= -1;
```

Reverses the vertical direction when the ball touches the top or bottom wall.

---

## Step 5 — Paddle Collision

```javascript
ballSpeedX *= -1;
```

The ball bounces back after touching the paddle.

---

## Step 6 — Score System

If the ball passes the paddle,

```javascript
score++;
```

The opponent earns one point.

---

## Step 7 — Reset Ball

The ball returns to the center.

```javascript
ballX = width/2;

ballY = height/2;
```

A new round begins immediately.

---

# Internal Working

```text
Move Ball

↓

Move Paddle

↓

Check Wall

↓

Check Paddle

↓

Score?

↓

Reset Ball

↓

Repeat
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| keyIsDown() | Paddle movement |
| constrain() | Limit paddle position |
| random() | Random ball direction |
| rect() | Draw paddle |
| circle() | Draw ball |
| text() | Display score |

---

# Output Observation

✔ Paddle responds instantly to keyboard input.

✔ Ball bounces realistically from walls.

✔ Ball reverses direction after hitting the paddle.

✔ Score increases whenever the paddle misses the ball.

---

# Optimization Tips

### Tip 1

Increase the ball speed gradually to make the game more challenging.

Example

```javascript
ballSpeedX *= 1.05;
```

after every successful paddle hit.

---

### Tip 2

Display both **Player Score** and **Opponent Score** for a complete Pong game.

---

### Tip 3

Use functions such as

```javascript
moveBall();

drawBall();

checkCollision();
```

to organize larger game projects.

---

### Tip 4

Add sound effects for collisions to improve user experience.

---

# Common Mistakes

## Mistake 1

Not constraining the paddle.

The paddle disappears outside the canvas.

---

## Mistake 2

Forgetting to reverse the ball direction.

The ball passes through the paddle.

---

## Mistake 3

Resetting only the ball position but not its speed.

The game becomes predictable.

---

## Mistake 4

Using incorrect collision dimensions.

The paddle appears to miss even when it touches the ball.

---

# Challenge Exercises

### ⭐ Easy

Change the paddle and ball colors.

---

### ⭐⭐ Medium

Display the player's score in addition to the opponent's score.

---

### ⭐⭐⭐ Hard

Create an AI-controlled paddle on the right side that follows the ball.

---

### ⭐⭐⭐⭐ Expert

Develop a complete two-player Pong game using:

- Player 1 → **W / S**
- Player 2 → **↑ / ↓**

Include:

- Winning score
- Restart button
- Sound effects
- Start screen
- Game over screen

---

# Viva Questions

### Q1

What is the purpose of the paddle?

**Answer**

The paddle prevents the ball from leaving the screen by hitting it back into the playing area.

---

### Q2

How is wall collision detected?

**Answer**

By checking whether the ball reaches the top or bottom boundary and reversing its vertical velocity.

---

### Q3

Why do we reverse the X velocity after paddle collision?

**Answer**

Reversing the horizontal velocity changes the direction of the ball, creating the bouncing effect.

---

### Q4

Why is `random()` used when resetting the ball?

**Answer**

It gives the ball a different vertical direction after each reset, making gameplay less predictable.

---

### Q5

How can Pong be made more interesting?

**Answer**

By adding an AI opponent, increasing ball speed, introducing power-ups, sound effects, and multiplayer support.

---

# 📌 Quick Revision

✅ Paddle Movement

✅ Ball Animation

✅ Wall Collision

✅ Paddle Collision

✅ Score Management

✅ Continuous Game Loop

---

# 📚 Summary

After completing this experiment, you should understand:

✔ Keyboard-Controlled Gameplay

✔ Collision Detection

✔ Boundary Checking

✔ Ball Physics

✔ Score Tracking

✔ Core Arcade Game Mechanics

---

# 🚀 Next Experiment

## Problem 27 — Shooting Game

In the final experiment, you will create a complete shooting game featuring:

- 🔫 Bullet Firing
- 🎯 Target Generation
- 💥 Collision Detection
- 📊 Score System
- 🎮 Real-Time Gameplay

This experiment combines nearly every concept learned throughout the codebook into one interactive game.

# 🎮 Part 7C — Game Development

---

# Problem 27

# Shooting Game with Bullet Collision Detection and Score System

---

## 🎯 Objective

Create a shooting game where the player controls a cannon at the bottom of the screen.

The player can:

- Move left and right.
- Fire bullets using the **Spacebar**.
- Hit moving targets.
- Earn points for every successful hit.

---

# 📖 Theory

A shooting game combines several important concepts of computer graphics and game programming.

These include:

- Keyboard Input
- Object Animation
- Collision Detection
- Arrays
- Object Management
- Score System

Unlike previous experiments, multiple objects (bullets and targets) exist simultaneously and interact with one another.

---

# Real-Life Applications

The same concepts are used in:

- 🎮 Space Shooter Games
- 🚀 Arcade Games
- 🛡 Defense Games
- 🎯 Target Practice Simulators
- 🤖 Robotics Simulations
- 🛰 Space Battle Games

---

# Game Components

```text
Target

        ●

        ↓

---------------------------

          ↑

        Bullet

---------------------------

      ███████

       Player
```

---

# Game Flow

```text
Start

↓

Move Player

↓

Fire Bullet

↓

Move Bullet

↓

Move Target

↓

Collision?

↓

Yes

↓

Increase Score

↓

Generate New Target

↓

Repeat
```

---

# Collision Logic

```text
Bullet

↓

Touches

↓

Target

↓

Destroy Target

↓

Increase Score
```

---

# Algorithm

```text
Start

↓

Create Player

↓

Create Target

↓

Move Player

↓

Fire Bullet

↓

Move Bullet

↓

Move Target

↓

Check Collision

↓

Update Score

↓

Repeat
```

---

# Source Code

```javascript
let playerX = 350;

let bullets = [];

let targetX;
let targetY = 40;

let score = 0;

function setup(){

    createCanvas(700,400);

    targetX = random(50,width-50);

}

function draw(){

    background(20);

    // Player

    fill(0,180,255);

    rectMode(CENTER);

    rect(playerX,height-20,80,20);

    // Move Player

    if(keyIsDown(LEFT_ARROW))

        playerX -= 6;

    if(keyIsDown(RIGHT_ARROW))

        playerX += 6;

    playerX = constrain(playerX,40,width-40);

    // Target

    fill(255,80,80);

    circle(targetX,targetY,30);

    targetY += 2;

    if(targetY > height){

        targetY = 40;

        targetX = random(50,width-50);

    }

    // Bullets

    fill(255,255,0);

    for(let i=bullets.length-1;i>=0;i--){

        bullets[i].y -= 8;

        circle(bullets[i].x,bullets[i].y,10);

        // Collision

        if(dist(bullets[i].x,bullets[i].y,targetX,targetY)<20){

            score++;

            targetY = 40;

            targetX = random(50,width-50);

            bullets.splice(i,1);

        }

        // Remove Bullet

        else if(bullets[i].y<0){

            bullets.splice(i,1);

        }

    }

    // Score

    fill(255);

    textSize(22);

    text("Score : "+score,20,30);

}

function keyPressed(){

    if(key==' '){

        bullets.push({

            x:playerX,

            y:height-30

        });

    }

}
```

---

# Program Output

```text
Score : 8


        ●

        ↓


        ↑

      Bullet


██████████

 Player
```

Move using the **Left** and **Right** arrow keys.

Press the **Spacebar** to shoot bullets.

Destroy targets to earn points.

---

# Step-by-Step Code Explanation

## Step 1

Create the player.

```javascript
rect()
```

The player remains near the bottom of the canvas.

---

## Step 2

Move the player.

```javascript
keyIsDown()
```

Arrow keys move the player horizontally.

---

## Step 3

Fire bullets.

```javascript
bullets.push(...)
```

Every Spacebar press creates a new bullet.

---

## Step 4

Move bullets.

```javascript
bullets[i].y -= 8;
```

Bullets travel upward.

---

## Step 5

Move target.

```javascript
targetY += 2;
```

The target continuously falls downward.

---

## Step 6

Collision Detection

```javascript
dist(...)
```

If the distance between a bullet and the target is small enough,

the target is considered destroyed.

---

## Step 7

Increase Score

```javascript
score++;
```

Each successful hit earns one point.

---

## Step 8

Generate New Target

```javascript
targetX = random(...);
```

The target reappears at a new random position.

---

# Internal Working

```text
Player

↓

Fire Bullet

↓

Move Bullet

↓

Move Target

↓

Collision

↓

Increase Score

↓

Create New Target
```

---

# Important Functions

| Function | Purpose |
|----------|----------|
| keyPressed() | Detect Spacebar |
| keyIsDown() | Move player |
| push() | Create bullet |
| splice() | Remove bullet |
| random() | Generate target |
| dist() | Collision detection |
| constrain() | Keep player inside canvas |

---

# Output Observation

✔ Player moves smoothly.

✔ Multiple bullets can exist simultaneously.

✔ Targets continuously move downward.

✔ Successful hits increase the score.

✔ Destroyed targets reappear randomly.

---

# Optimization Tips

### Tip 1

Use arrays for bullets instead of individual variables.

---

### Tip 2

Remove bullets after they leave the screen.

This improves performance.

---

### Tip 3

Increase target speed as the score increases.

Example

```javascript
targetSpeed += 0.2;
```

---

### Tip 4

Use images instead of simple shapes for a more attractive game.

---

# Common Mistakes

## Mistake 1

Not removing old bullets.

Memory usage continuously increases.

---

## Mistake 2

Checking collision before moving the bullet.

This may produce inaccurate results.

---

## Mistake 3

Not generating a new target after a hit.

The game appears to stop.

---

## Mistake 4

Using only one bullet variable.

The player cannot fire multiple shots.

---

# Challenge Exercises

### ⭐ Easy

Change the bullet color.

---

### ⭐⭐ Medium

Create multiple targets.

---

### ⭐⭐⭐ Hard

Add three lives and a Game Over screen.

---

### ⭐⭐⭐⭐ Expert

Develop a complete shooting game featuring:

- Multiple enemy types
- Different bullet speeds
- Health system
- Power-ups
- Sound effects
- Particle explosions
- High score saving
- Start menu
- Pause feature
- Game Over screen

---

# Comparison of Game Development Experiments

| Problem | Main Concept |
|---------|--------------|
| **25** | Catch-the-Object Game |
| **26** | Pong Game |
| **27** | Shooting Game |

---

# Viva Questions

### Q1

Why are bullets stored in an array?

**Answer**

Because multiple bullets can exist at the same time, and an array allows us to store and update each bullet independently.

---

### Q2

How is collision detected?

**Answer**

The `dist()` function calculates the distance between the bullet and the target. If the distance is less than a specified threshold, a collision is detected.

---

### Q3

Why do we use `splice()`?

**Answer**

`splice()` removes bullets that have either hit the target or moved off the screen, preventing unnecessary memory usage.

---

### Q4

How can the game become more challenging?

**Answer**

Increase target speed, spawn multiple targets, reduce player movement speed, or introduce moving enemies.

---

### Q5

Which programming concepts are demonstrated in this experiment?

**Answer**

- Arrays
- Keyboard Input
- Collision Detection
- Animation
- Random Number Generation
- Score Management
- Game Logic

---

# 📌 Quick Revision

✅ Keyboard Input

✅ Bullet Creation

✅ Arrays

✅ Collision Detection

✅ Score System

✅ Object Management

✅ Simple Game Loop

---

# 📚 Chapter 7 Summary

After completing Problems **25–27**, you should understand:

✔ Game Loops

✔ Player Control

✔ Keyboard Interaction

✔ Bullet Mechanics

✔ Collision Detection

✔ Score Management

✔ Random Object Generation

✔ Object Arrays

✔ Basic Game Design

These concepts provide a strong foundation for developing more advanced 2D games in p5.js.

---

# 🎉 Congratulations!

You have successfully completed all **27 p5.js laboratory experiments**.

Throughout this codebook, you learned:

- 🎨 Basic Drawing and Colors
- 🎞 Animation
- 🔄 Transformations
- 🖱 Mouse and Keyboard Interactivity
- ✨ Particle Systems
- 🌍 Physics Simulation
- 🎵 Audio Programming
- 🎮 Game Development

By mastering these topics, you now have the fundamental skills required to create interactive graphics, simulations, multimedia applications, and simple games using **p5.js**.

---

# 📚 References

- **p5.js Official Documentation:** https://p5js.org/reference/
- **p5.js Website:** https://p5js.org/
- **The Coding Train (Daniel Shiffman):** https://thecodingtrain.com/
- **Processing Foundation:** https://processing.org/
- **Mozilla Developer Network (JavaScript):** https://developer.mozilla.org/

---

# 👨‍💻 Author

**Prepared by:**

**Ashikur Rahman**

Department of Computer Science and Engineering (CSE)

Hajee Mohammad Danesh Science and Technology University (HSTU)

---

# 📄 License

This codebook is prepared for **educational and academic purposes only**.

Students are encouraged to study, modify, and experiment with the source code to improve their understanding of computer graphics and interactive programming using p5.js.

---

# 🙏 Acknowledgements

Special thanks to:

- The Processing Foundation
- The p5.js Community
- Course Instructor
- Department of CSE, HSTU
- Everyone who contributes to open-source educational resources

---

# ⭐ Keep Learning

> *"The best way to learn programming is by building projects. Experiment, modify the code, make mistakes, and keep creating."*

**Happy Coding! 🚀**
