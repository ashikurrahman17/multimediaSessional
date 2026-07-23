# 🎨 Computer Graphics Laboratory Codebook using p5.js

<p align="center">
<img src="https://p5js.org/assets/img/p5js.svg" width="180">
</p>

<p align="center">
A complete practical guide for Computer Graphics Laboratory using <b>p5.js</b>.
</p>

---

# Table of Contents

- Introduction
- What is p5.js?
- Installing & Running p5.js
- Basic Structure of a p5.js Program
- Frequently Used Functions
- Coding Guidelines
- Problem 01 – Basic Shapes and Colors
- Problem 02 – Simple Graphical Scene
- Problem 03 – Mouse Coordinates
- Problem 04 – Moving Shape Animation

---

# Introduction

This repository contains the complete solutions of Computer Graphics Laboratory exercises using **p5.js**, a JavaScript library developed to make creative coding and graphics programming easier.

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

# Problem 01
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

# Problem 02
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

# Problem 03
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

# Problem 04
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

# Problem 05
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

# Problem 06
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

# Problem 07
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

# Problem 08
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

# Problem 09
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

