---
layout: post
title: "Writing Code in 3D"
category: code
description: "A script is more like sheet music than a novel."
featured: true
---

Code is made of line by line instructions neatly arranged in exact syntax. It's all logic and text, so the text-focused side of the brain defaults to trying to write one line, then the next, in order from top to bottom.

But, counter intuitively, writing code is not linear. A script is more like sheet music than a novel. Sheet music appears linear on the page, but when played the musician jumps from section to section based on the written instructions and creates a multi-dimensional expression of the music through layers of sound. The musical notation is a flat summary of the real 3D experience. The resulting music is played linearly, but it has depth in layers and doesn't follow the exact order of notes on the page because the notation often includes instructions to repeat, skip, or jump to different sections.

Similarly, a script appears linear on the screen, but when it's actually run it's more accurate to imagine what happens inside the computer as a 3D workspace with depth, repeated processes, and jumps to different points in the script.

This misconception is often a roadblock when learning how to write code. For someone learning how to read and write code, it's tempting to think you need to start at the top of the file and work your way to the bottom. This leads to frustration because it's not only an inaccurate model of what happens when the script runs, it limits your flexibility to sculpt the code iteratively and discover solutions through drafts and experiments.

I imagine many developers "think in 3D" when programming without realizing it, and likely rarely stop to practice it or explain how it works. It happens naturally and subconsciously with more fluency in programming. However, it can and should be practiced, especially if you're a new developer feeling stuck (which everyone feels most days when they're learning). Combining the logical, text-focused side of writing code with the visual, space/time process of imagining what happens when it runs is a vital part of programming, and practicing it will likely help you get unstuck.

To illustrate how "thinking in 3D" works, let's try it together. I'll walk through writing a short script and talk through how it might be imagined in a 3D space so you can try it on your own. If you've experienced this style of thinking when writing code, or try it after reading this, let me know your thoughts!

## The script as a landscape

Imagine a cube. It might be abstract and transparent, or it might be an imaginary landscape like a tropical island, a mountain, or a city block.

This cube is the space your script uses within the computer when it runs. Every instruction you write in your script will change this 3D space. (Feel free to draw this cube on paper and edit it as you write the script if it's helpful.)

If you're writing a script, hopefully you have a rough idea of what you want it to do. But this is where a developer might get stuck if they're not thinking in 3D. Where do we actually start? Thinking linearly, the only option is to start at the beginning, but it might not be obvious what the beginning should be because we haven't figured out the "solution" yet. If we knew every solution before we started, programming would be very easy. With the 3D landscape in mind, it's possible to start anywhere, beginning, middle, or end, and it's okay if the first attempt isn't the final solution because it can be adjusted later. We can build up the scene piece by piece and rearrange the pieces as needed, like deciding how furniture should be arranged in a room.

Let's say for our script we know we need variables that store a user's name:

```
const firstName = 'Jim';
const lastName = 'Henson';
```

Now let's imagine what effect this has on our 3D workspace. Maybe in one corner of the cube a box appears with the label `firstName` and inside the string 'Jim' is stored. Next to it, another box appears with the label `lastName` and the word 'Henson' inside of it. This is an imaginary representation of the computer's memory as it stores values in variables.

Now let's imagine we know we need a function that can give us a formatted full name:

```
function formatFullName(firstName, lastName) {
  return `${firstName} ${lastName}`;
}
```

This function also appears inside our 3D space, but since it's a function and not just a variable, it has different visual characteristics. If we're imagining a city block, maybe it's represented by a truck, or a crane, or some other symbol that indicates it can be used for a task, and it's given the label `formatFullName`.

Let's write an instruction for the function to be called:

```
const fullName = formatFullName(firstName, lastName);
```

Now, imagine what happens when the script actually runs. The boxes pop up with the names inside. The construction worker operating a crane pops up and waits for instructions. Then the worker maneuvers the crane to the name boxes, takes out each name, copies and combines them, and puts the result into a new box labelled `fullName`.

This is a small example, but you can imagine how this process might grow as more variables, functions, and other instructions are added to a script. A class might be imagined as a building or a tree. A whole web application might be a series of interconnected cubes, each with their own landscape of memory and tools. And when the script runs, we can imagine all the workers moving around completing tasks, sending messages to each other, boxes being created and destroyed, and complex structures being generated as the script does its job.

---

This imaginary, non-linear thinking is not only fun, it's also a more accurate representation of what happens when a computer runs a script. And it enables a more iterative approach to writing code, which is essential for exploring options and working toward refined drafts.

Do you ever find yourself thinking in 3D when writing code? Does this description seem familiar, or has it helped you think differently about writing code? Let me know your thoughts on [Twitter](https://twitter.com/kev_mcg) or by commenting below!
