📘 <span style="color:#3A8FB7">Project Overview</span>

This project is a calculator web application developed entirely by myself.

I began with a simple calculator and progressively improved it by adding scientific features, refining the logic, debugging complex issues, and making the interface responsive across devices.

The goal was not only to build a working calculator but to deeply understand:

JavaScript logic

DOM manipulation

Expression parsing

Debugging strategies

Responsive design

This project became a strong exercise in real-world problem solving.

🛠 <span style="color:#2F6F7E">Technologies Used</span>
🧱 <span style="color:#3A8FB7">HTML</span>

Structured the calculator layout

Created buttons for numbers, operators, and scientific functions

Built the display area for expressions and results

🎨 <span style="color:#3A8FB7">CSS</span>

Styled the calculator interface

Designed a responsive layout

Used a color palette based on duck-egg blue, blue, and grey

Improved button sizing and spacing for usability

📱 Mobile Compatibility Challenge

The website was not initially compatible with phones.

Issues included:

Broken layout on small screens

Misaligned buttons

Poor touch usability

Display scaling problems

To fix this, I:

Implemented media queries

Adjusted button sizes for touch devices

Improved spacing and alignment

Ensured the display resized correctly

The calculator is now responsive and works across different screen sizes.

⚙️ <span style="color:#3A8FB7">JavaScript</span>

JavaScript powers the core functionality:

Handles button clicks

Processes keyboard input

Performs calculations

Manages scientific functions

Controls and updates the display

Handles edge cases and error prevention

This is where most development challenges occurred.

🧮 <span style="color:#2F6F7E">Calculator Features</span>
➕ <span style="color:#3A8FB7">Basic Calculator</span>

Addition (+)

Subtraction (−)

Multiplication (×)

Division (÷)

Clear (C / AC)

Backspace (⌫)

Parentheses ( )

🔬 <span style="color:#3A8FB7">Scientific Features</span>

π (Pi)

sin, cos, tan (degrees)

x² (square)

x³ (cube)

± (plus/minus toggle)

% (percentage)

🚧 <span style="color:#2F6F7E">Development Process & Challenges</span>
🧩 <span style="color:#3A8FB7">1. Building the Basic Calculator</span>

Initially, I implemented:

Number display

Basic arithmetic

Expression evaluation

The logic worked correctly but was simple and linear.

🔄 <span style="color:#3A8FB7">2. Adding Scientific Functions</span>

After the basic version worked, I added:

π

sin, cos, tan

Square and cube

This caused multiple issues:

Display stopped updating correctly

Functions applied to the entire expression instead of the last number

JavaScript execution errors

To resolve this:

I used console debugging

Reworked how expressions were stored as strings

Ensured functions applied only to the last operand

Fixed incorrect DOM references

This required restructuring logic instead of quick fixes.

📊 <span style="color:#3A8FB7">3. Percentage Calculation — Major Challenge</span>

The percentage (%) feature was the most difficult part of the project.

❌ Initial Problems

When adding or subtracting percentages:

100 + 10%

200 − 15%

The calculator produced incorrect results.

The main issues:

Treating % as simple division by 100

Not referencing the previous operand

Incorrect formula logic

Breaking chained operations

Decimal handling errors

🧠 The Logical Problem

Percentage behavior depends on the operator used.

Correct formulas:

Addition

A + B% = A + (A × B / 100)

Subtraction

A − B% = A − (A × B / 100)

My mistake was:

Not properly extracting the previous operand

Not detecting which operator was active

Not recalculating percentage relative to that operand

🔁 Multiple Rewrites

I had to rewrite the percentage logic several times.

Every time I fixed one issue, another edge case appeared:

Multiple chained operations

Decimal percentages

Percent after multiplication

Percent after division

Parentheses interactions

± toggle with percentages

This forced me to:

Rethink expression parsing

Improve operand extraction logic

Carefully test edge cases

This was the most educational part of the entire project.

🖥 <span style="color:#3A8FB7">4. Display Problem with Large Numbers</span>

Originally, I used a single-line <input>.

Problems:

Long expressions overflowed

Large numbers were cut off

Hard to track full calculations

✅ <span style="color:#2F6F7E">Solution</span>

I replaced the <input> with a multi-line <textarea>:

Enabled text wrapping

Added scrolling

Automatically scrolled to the bottom

Preserved full expression visibility

Initially, this broke the display because:

Old DOM references were still used

.value was not updating correctly

Functions targeted incorrect elements

After debugging and fixing references, full functionality returned.

🎯 <span style="color:#2F6F7E">Final Result</span>

The final calculator:

Supports basic and scientific calculations

Correctly handles percentage logic

Displays large numbers and long expressions

Works on desktop and mobile devices

Demonstrates structured debugging and progressive enhancement

📚 <span style="color:#2F6F7E">What I Learned</span>

DOM manipulation with JavaScript

Expression parsing logic

Why percentage calculations are more complex than expected

The importance of testing edge cases

How small logic changes break large systems

Step-by-step debugging instead of rewriting everything

How to make a web app responsive

🚀 <span style="color:#2F6F7E">Future Improvements</span>

DEG / RAD toggle

Calculation history panel

Full keyboard-only support

Better error handling (invalid expressions, divide by zero)

Accessibility improvements

Refactoring into modular logic structure

✨ This project represents more than a calculator — it reflects growth in debugging, logical thinking, and building resilient front-end applications.
