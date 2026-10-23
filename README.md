## Digital Imaging processing Lab01

Python Basics & Image Processing Setup

This repository contains the initial setup and basic Python exercises required for the Digital Image Processing course.

Prerequisites

Before running the exercises, ensure you have Python installed on your system. The exercises require specific external libraries for numerical operations, image handling, and plotting.

Step 1: Install Required Packages

Open your terminal or command prompt and run the following command to install the necessary packages:

```bash
python -m pip install numpy pillow matplotlib
```

· NumPy: Supports numerical arrays.
· Pillow: Provides image tools.
· Matplotlib: Supports plotting.

To confirm the packages are installed correctly, run:

```bash
python -m pip show numpy pillow matplotlib
```

---

Project Structure

· basics.py: Contains the solutions to all six basic Python exercises.
· Note: Python files use the .py extension, and comments start with #.

---

Exercises Overview

Create a file named basics.py and complete the following exercises. Use four-space indentation for Python code blocks.

Exercise 1: Variables and Data Types

· Create variables: width = 640, height = 480, image_name = "sample.png", and is_color = True.
· Print each value and its type.
· Calculate and print the total number of pixels using width * height.
· Expected total: 307200

Exercise 2: if, elif, and else

Write a condition that evaluates an intensity value:

· Labels intensity < 0 or > 255 as Invalid.
· Labels values >= 128 as Bright pixel.
· Labels values < 128 as Dark pixel.
· Test with values: -1, 0, 127, 128, 255, 256.
· Expected Output: Invalid, Dark pixel, Dark pixel, Bright pixel, Bright pixel, Invalid.

Exercise 3: for and while Loops

· Use a for loop to visit [20, 130, 255] and print each value with its Bright/Dark label (using 128 as the threshold).
· Use a while loop to print 0, 1, and 2, stopping before 3 (Remember to update the loop counter).

Exercise 4: Functions

· Define a function is_bright(pixel, threshold=128) that returns True when the pixel is at least the threshold, and False otherwise.
· Print the results of: is_bright(127), is_bright(128), and is_bright(200, 210).
· Expected results: False, True, False

Exercise 5: Lists and Tuples

· Create pixels = [0, 128, 255].
· Print the first item, replace the middle item with 150, append 64, and print the final list and its length.
· Expected list: [0, 150, 255, 64], length: 4.
· Create a tuple size = (640, 480), unpack it into width and height, and print both.
· Include a comment explaining why a list item can be changed while a tuple item cannot.

Exercise 6: Dictionaries and Sets

· Create a dictionary image = {"width": 640, "height": 480}. Add "mode": "RGB", then print the width and mode using their keys.
· Convert the list ["cat", "dog", "cat", "bird"] into a set and print its length.
· Expected number of unique labels: 3 (Note: Set display order may vary).

---

How to Run

To run the completed exercises, execute the following command in your terminal:

```bash
python basics.py
```
