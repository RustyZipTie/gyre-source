# Gyre manual
<img src="../img/pretty/main-demo.png" height="300px">  

## Welcome to the world of Gyre!
> In reality, this is less of a complete manual than a compilation of tips and tricks that I have stumbled upon
in the process of designing and testing the system. I intend to continually update it as I learn more, and I
hope to hear from all of you about what you have found that works and what doesn't. There is no single "correct"
way to print or assemble Gyre- whatever works for you is what you should do.
>
> Have fun!

## Contents
[Planning](#planning)

[Printing](#printing)

[Assembling](#assembling)

[Mounting](#mounting)

## Planning
<img src="../img/pretty/dwg.png" height="200px">

>Note: all measurements are in inches unless stated otherwise.

Currently, there are two basic layouts: linear and hex.

<img src="../source/img/linear_layout.png" height="30px">

<img src="../source/img/hex_layout.png" height="200px">

I recommend sticking with one of these, especially if you are just starting out with Gyre.
Once you get the "feel" of the system, you will almost certainly think of new ways to use it (see the pictures at the end of this section).
If you find a cool new layout, I would love to hear about it in the [feedback form]() or [thingiverse comments]().

In my opinion, the best way to design your layout is as follows:
- Start with a rough idea of what you want
- Print a few parts
- Put them together and hold them up on the wall
- Looking at them, form a guesstimate of how many more pieces you need
- Repeat as necessary

However, for those of you that need or want to be more precise, here are some tips and formulas to plan your
Gyre layout ahead of time:

#### Linear
Linear layout forms a single horizontal line. Rails can be any length, and they are connected by linear joints.
I recommend using a standard length of rail, but you can mix it up if you want.
To calculate the length of a linear setup, use the following formula (assumes that you are using mounting locks on the ends):
|Variable|Represents|
|:---:|:---:|
|W|total width|
|Lr|length of rail|
|Nr|number of rails|

$$W = ((Lr - 1) * Nr) + (2 * (Nr - 1)) + 1.25$$

For instance, if you are using 8-slot rails, and you have 5 of them, the length will be $$((8-1) * 5) + (2*(5-1)) + 1.25 = 44.25$$ inches long.

#### Hex

There is a little more variability when it comes to hexagonal layouts. You can, of course, make all the sides  
equal, like this:  
%%pictures  
However, you may prefer to use different lengths of rails for the horizontal and diagonal sides, like this:  
%%pictures  
or this:  
%%pictures  
If your imagination is bigger than your print bed, you can even use two or more rails per side, using linear  
joints.  
%%pictures  
The formulas below should work as long as all of the diagonal sides are the same length, and all of the
horizontal sides are the same length. They also assume that you are using 120° joints all around the outside (rather than tri joints).

|Variable|Represents|
|:---:|:---:|
|H|total height|
|W|total width|
|Ld|length of diagonal rails|
|Lv|length of vertical rails|
|Nd|number of diagonal rails|
|Nh|number of horizontal rails|
> Note- Nd and Nh refer to the number of rails in a given row or column. 
For instance, in the layout below, Nh = 3 (purple) and Nw = 3 (green)

><img src="../source/img/h-w_final.png" height="150px">

**W = ((Lh + 1) \* Nh) + (0.5 \* (Ld + 1) \* (Nh + 1)) + 0.95**

**H = ((Ld + 1) \* Nd \* 0.87) + 1.25**  

#### Other layouts
%%pictures

## Printing
<img src="../source/img/sliced.png" height="200px">

There is nothing special about printing Gyre parts- default settings should be just fine most of the time.

Print settings for Gyre attachments may vary. These are beyond the scope of this tipsheet. 
For more info, check out the thingiverse page for the attachment you are printing.

A few notes for printing parts in the core framework:
- I have only printed them in PLA, so I don't know how well other materials work. 
Feel free to experiment with other materials. I'd love to hear what your results are.
- No supports should be needed, as long as the prints are oriented correctly, and your printer can manage a 45° overhang. 
- Brims are a pain to remove, so only use them if you're having adhesion issues.
- Always use common sense!

## Assembling

## Mounting