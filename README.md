# Manim Installation Guide

## Introduction
Manim (Mathematical Animation Engine) is an open-source Python library used for creating animations for mathematical concepts, educational videos, and presentations. It allows you to produce high-quality animations using Python code, making it an excellent tool for educators and content creators.

## Purpose
This guide will help you install Manim on your local machine so you can start creating your own animations.

## Installation Steps

1. **Download Manim:**
   - Go to the [Manim download page](https://sourceforge.net/projects/manim.mirror/) and download the latest version of the source code.

2. **Extract the ZIP File:**
   - Locate the downloaded ZIP file (e.g., `Manim v0.18.1 source code.zip`) on your computer.
   - Right-click the file and select "Extract All" or use any extraction tool to unzip it.

3. **Navigate to the Extracted Directory:**
   - Open a terminal (Command Prompt on Windows, Terminal on macOS/Linux).
   - Use the `cd` command to navigate to the directory where you extracted the Manim files. For example:
     ```bash
     cd path/to/extracted/Manim-v0.18.1
     ```

4. **Install Manim:**
   - Ensure you have Python and pip installed. You can verify this by running:
     ```bash
     python --version
     pip --version
     ```
   - If you have Python and pip installed, run the following command to install Manim:
     ```bash
     pip install .
     ```

5. **Verify the Installation:**
   - To check if Manim has been installed correctly, run:
     ```bash
     manim --version
     ```

6. **Creating Your First Animation:**
   - Create a new Python file (e.g., `test.py`) with the following code to test your installation:
     ```python
     from manim import *

     class HelloWorld(Scene):
         def construct(self):
             text = Text("Hello, World!")
             self.play(Write(text))
             self.wait(1)
     ```
   - Run the animation with the following command:
     ```bash
     manim -pql test.py HelloWorld
     ```

## Conclusion
You have successfully installed Manim and created your first animation! Explore the Manim documentation for more examples and advanced features.

## Additional Resources
- [Manim Documentation](https://docs.manim.community/en/stable/)
- [Manim GitHub Repository](https://github.com/ManimCommunity/manim)
