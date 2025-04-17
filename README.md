# fractalicious
a visualization of the Mandelbrot Set 
Mandelbrot Set Visualization

This Python script generates a visualization of the Mandelbrot set, a famous fractal named after the mathematician Benoit Mandelbrot. The script uses NumPy for efficient array computations and Matplotlib for plotting the resulting image.

Requirements
Python 3.x
NumPy (pip install numpy)
Matplotlib (pip install matplotlib)

Usage
Ensure the required libraries are installed.
Save the script as mandelbrot.py.
Run the script using Python:
python mandelbrot.py

A window will display the Mandelbrot set with a color map representing the escape time of points.

Parameters
width, height: Resolution of the output image (default: 1000x1000 pixels).
max_iter: Maximum number of iterations to determine if a point is in the Mandelbrot set (default: 100).
threshold: Escape threshold for the magnitude of the complex number (default: 2.0).

x, y: Range of the complex plane to visualize (x: [-2, 1], y: [-1.5, 1.5]).

How It Works
The script:
Creates a grid of complex numbers c representing points in the complex plane.

Iteratively applies the Mandelbrot function z = z^2 + c for each point.

Tracks the iteration at which each point escapes (magnitude exceeds threshold) or marks it as part of the set if it doesn't escape within max_iter.

Visualizes the result using Matplotlib, where colors represent the escape time, and a color bar indicates the iteration count.

Output
The script generates a plot of the Mandelbrot set with:

Black regions indicating points in the Mandelbrot set.
Colored regions showing the escape time for points outside the set, using the 'hot' colormap.
A color bar to interpret the iteration counts.

Customization
Adjust width and height for higher or lower resolution.
Increase max_iter for more detailed iteration counts (may increase computation time).
Change the cmap parameter in plt.imshow to use different color schemes (e.g., 'viridis', 'plasma').
Modify the x and y ranges to zoom into specific regions of the Mandelbrot set.

Notes
Higher max_iter or resolution increases computation time.
The script uses vectorized operations for efficiency but may still be slow for very high resolutions.
developed with xAI (Grok 3), Google Colab & Microsoft Copilot for the purposes of learning and teaching python scripting. Music & vibes by wifiknight45
