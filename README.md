# CSS calc() Errors: Handling Invalid Calculations and Negative Values

This repository demonstrates common errors and solutions related to using the `calc()` function in CSS.  The `calc()` function is powerful but can lead to unexpected issues if not handled correctly.  The `bug.css` file showcases examples of these issues, while `bugSolution.css` provides corrected versions.

**Common Issues:**

* **Negative values for width/height:**  Attempting to set a negative width or height using `calc()` can cause elements to disappear or behave unexpectedly.
* **Invalid operands:**  Using non-numeric values or invalid operators within the `calc()` function will result in errors.
* **Unit mismatches:** Inconsistent use of units within the calculation can also lead to issues.

**Solutions:**

* **Conditional statements:** Use CSS preprocessors (like Sass or Less) or media queries to conditionally apply styles depending on the available space.
* **Math.max():** Use `Math.max()` (within a preprocessor) to ensure values remain non-negative.
* **Careful unit handling:** Ensure consistent use of units throughout your calculations.
* **Thorough testing:**  Test your `calc()` expressions with various dimensions to identify potential issues early on.