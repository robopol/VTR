# Schwarzschild Metric Visualization

![Schwarzschild Metric](path/to/screenshot.png) <!-- Add a screenshot of your visualization here -->

## Overview

The **Schwarzschild Metric Visualization** is an interactive web application that visualizes the curvature of space around a spherically symmetric, non-rotating massive object (e.g., a black hole) as described by the Schwarzschild metric in General Relativity. Utilizing HTML, CSS, and JavaScript along with the Plotly.js library, this project offers dynamic 2D and 3D representations to help users understand complex spacetime geometries.

## Features

- **2D Visualization of Curved Space:** Interactive scatter plots representing the effective radial distance.
- **3D Visualization of Curved Space:** Comprehensive 3D scatter plots with an event horizon overlay.
- **2D Time Flow Simulation:** Animated visualization demonstrating time dilation effects.
- **2D Vertical Cross-Section of Curved Space:** Displays the "funnel" effect as radial distance approaches infinity.
- **Language Toggle:** Switch between Slovak and English descriptions for accessibility.
- **Responsive Design:** Adjusts seamlessly to different screen sizes.

## Mathematical Foundations

### Schwarzschild Metric

The Schwarzschild metric in spherical coordinates \((t, r, \theta, \phi)\) is defined as:

\[
ds^2 = -\left(1 - \frac{r_s}{r}\right) c^2 dt^2 + \left(1 - \frac{r_s}{r}\right)^{-1} dr^2 + r^2 (d\theta^2 + \sin^2 \theta \, d\phi^2)
\]

where \( r_s \) is the Schwarzschild radius:

\[
r_s = \frac{2GM}{c^2}
\]

### Effective Radial Distance

The effective radial distance \( R(r) \) is given by the integral:

\[
R(r) = \int_{r_0}^{r} \frac{dr'}{\sqrt{1 - \frac{r_s}{r'}}}
\]

This integral can be expressed analytically as:

\[
R(r) = \sqrt{r(r - r_s)} + r_s \ln \left( \frac{\sqrt{r} + \sqrt{r - r_s}}{\sqrt{r_s}} \right) - \left( \sqrt{r_0(r_0 - r_s)} + r_s \ln \left( \frac{\sqrt{r_0} + \sqrt{r_0 - r_s}}{\sqrt{r_s}} \right) \right)
\]

where \( r_0 \) is a reference point, typically just above the Schwarzschild radius \( r_s \).

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/Schwarzschild-Metric-Visualization.git
