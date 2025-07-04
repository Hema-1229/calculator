BODMAS Calculator
> Overview
This is a simple, interactive web-based calculator that evaluates mathematical expressions following the BODMAS rule (Brackets, Orders, Division/Multiplication, Addition/Subtraction). It supports basic arithmetic operations, parentheses, square roots, percentages, powers, and memory functions.

> Technologies Used
* HTML5 – For structuring the calculator layout.
* CSS3 – For styling and responsive design.
* JavaScript – For calculator logic and interactivity.

> Features
* Basic operations: +, -, *, /
* Advanced operations: ^ (power), % (percentage), √ (square root)
* Parentheses support for BODMAS order
* Memory functions: M+ (add to memory), MR (recall memory)
* Clear (C) and Delete (Del) buttons
* Responsive and visually appealing UI

> Code Structure
1. HTML (<body>)
* Contains a .calculator container with:
* An <input> field (#display) to show the expression/result.
* A grid of <button> elements for digits, operators, and functions.
2. CSS (<style>)
* Styles the calculator with:
* Centered layout using Flexbox.
* Rounded buttons with hover effects.
* Colorful theme using soft blues and yellows.
3. JavaScript (<script>)
Handles all calculator logic:
4. appendToDisplay(value)
* Appends the clicked button's value to the display.
5. clearDisplay()
*  Clears the entire input field.
6. calculate()
* Converts:
* √ to Math.sqrt
* % to *0.01
* ^ to ** (exponentiation)
* Uses eval() to compute the result.
* Displays the result or "Error" if invalid.
7. memoryAdd()
* Evaluates the current expression.
* Adds the result to a memory variable if it's a valid number.
8. memoryRecall()
* Appends the stored memory value to the display.
9. deleteEachItem()
* Removes the last character from the display (like backspace).

> Notes
* eval() is used for simplicity but should be avoided in production apps due to security risks.
* The calculator assumes valid input; malformed expressions may return "Error".

> How to Use
* Open the HTML file in any modern browser.
* Click buttons to build your expression.
* Press = to evaluate.
* Use M+ to store results and MR to reuse them.

> Example Expressions
* 5 + 3 * (2 ^ 2) → 17
* √(16) + 10% → 4 + 0.1 → 4.1


