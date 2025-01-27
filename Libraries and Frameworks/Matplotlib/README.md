Matplotlib Tutorial

![Matplotlib Logo](https://github.com/AlaaAlshorbaji/Python/blob/b3a86b637e791015d95effce4c001629971669b7/Libraries%20and%20Frameworks/Matplotlib/course_thumbnail_default-new_171718030152.jpg)

**Matplotlib** is a powerful plotting library for Python and is often used for visualizing data in graphical form. Whether you're plotting simple line graphs, bar charts, histograms, or complex heatmaps, Matplotlib provides a wide array of functions to meet your needs. It is one of the most important libraries in Python for data visualization.

In this tutorial, we will cover the following topics:
- Basic Plotting
- Plotting with Different Types (Line, Scatter, Bar, Histogram, etc.)
- Customizing Plots (Titles, Labels, Legends)
- Saving Plots
- Subplots and Multiple Axes
- Advanced Plotting (Heatmaps, Contour Plots)

## Table of Contents

- [Introduction to Matplotlib](#introduction-to-matplotlib)
- [Creating Basic Plots](#creating-basic-plots)
- [Customizing Plots](#customizing-plots)
- [Subplots and Multiple Axes](#subplots-and-multiple-axes)
- [Saving Plots](#saving-plots)
- [Advanced Plotting](#advanced-plotting)

---

## Introduction to Matplotlib

Matplotlib is one of the most commonly used libraries for creating static, animated, and interactive plots in Python. It provides a wide range of features for generating complex visualizations with minimal code.

To install Matplotlib, run:
```bash
pip install matplotlib

Matplotlib's primary plotting interface is the pyplot module, which provides functions for creating and customizing various types of plots.

Importing Matplotlib

The main module to import is matplotlib.pyplot, which is often imported with the alias plt.

import matplotlib.pyplot as plt


---

Creating Basic Plots

The simplest plot in Matplotlib is a line plot, which can be created using plt.plot().

Example: Simple Line Plot

import matplotlib.pyplot as plt

# Data
x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

# Create a plot
plt.plot(x, y)

# Display the plot
plt.show()


---

Plotting with Different Types

Matplotlib supports a variety of plot types, including:

Line Plot

Scatter Plot

Bar Plot

Histogram


Example: Scatter Plot

x = [1, 2, 3, 4, 5]
y = [2, 3, 5, 7, 11]

plt.scatter(x, y)
plt.title("Scatter Plot Example")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()

Example: Bar Plot

categories = ['A', 'B', 'C', 'D']
values = [3, 7, 2, 5]

plt.bar(categories, values)
plt.title("Bar Plot Example")
plt.show()

Example: Histogram

data = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4]

plt.hist(data, bins=4, edgecolor='black')
plt.title("Histogram Example")
plt.show()


---

Customizing Plots

Matplotlib allows you to customize your plots with various options such as titles, axis labels, grid lines, and legends.

Example: Adding Titles and Labels

x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

plt.plot(x, y)
plt.title("Square Numbers")
plt.xlabel("X-axis: Number")
plt.ylabel("Y-axis: Square")
plt.show()

Example: Adding a Legend

x = [0, 1, 2, 3, 4]
y1 = [0, 1, 4, 9, 16]
y2 = [0, 1, 8, 27, 64]

plt.plot(x, y1, label="x^2")
plt.plot(x, y2, label="x^3")
plt.title("Comparison of x^2 and x^3")
plt.legend()
plt.show()

Example: Adding Grid Lines

x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

plt.plot(x, y)
plt.grid(True)
plt.show()


---

Subplots and Multiple Axes

Matplotlib supports creating multiple plots on the same figure using plt.subplot() and plt.subplots().

Example: Creating Multiple Subplots

x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

plt.subplot(1, 2, 1)  # 1 row, 2 columns, first subplot
plt.plot(x, y)
plt.title("Plot 1")

plt.subplot(1, 2, 2)  # 1 row, 2 columns, second subplot
plt.plot(x, y, color='red')
plt.title("Plot 2")

plt.tight_layout()  # Adjust spacing
plt.show()


---

Saving Plots

You can save your plots as image files (e.g., PNG, JPG) using plt.savefig().

Example: Save Plot as Image

x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

plt.plot(x, y)
plt.title("Saved Plot")
plt.savefig("plot.png")  # Save as PNG file
plt.show()


---

Advanced Plotting

Matplotlib also supports more complex visualizations, such as heatmaps, contour plots, and 3D plots.

Example: Heatmap

import numpy as np

data = np.random.rand(10, 10)

plt.imshow(data, cmap='hot', interpolation='nearest')
plt.title("Heatmap Example")
plt.colorbar()  # Add color bar to represent data values
plt.show()


---

Conclusion

This tutorial provided a comprehensive introduction to Matplotlib and its most commonly used features, including basic plotting, customizing plots, creating subplots, and saving plots. Matplotlib is a powerful tool for creating static, animated, and interactive visualizations in Python.

For more advanced examples and documentation, visit the official Matplotlib documentation: https://matplotlib.org/

Feel free to modify the code examples and experiment with your own datasets!

### How to Use:
1. **Installation**: Ensure you have Matplotlib installed by running `pip install matplotlib`.
2. **Explore**: Use the code examples provided to explore and learn about different types of plots.
3. **Practice**: Modify the code and experiment with your own data to gain a deeper understanding of how Matplotlib works.

Let me know if you need any further changes!

