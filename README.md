# Square Root Bisection Method

This repository contains an implementation of the square root approximation using the **bisection method** in Python. The script calculates the square root of a given number up to a specified level of accuracy (tolerance). This method ensures convergence for any non-negative input.

## How It Works

The bisection method is a numerical algorithm that approximates the square root by repeatedly dividing the range (initially between 0 and the target number) and narrowing it down based on the squared value of the midpoint. The process continues until the difference between the square of the midpoint and the target number is less than the specified tolerance or the maximum number of iterations is reached.

### Features
- Handles both integer and floating-point numbers.
- Supports user-defined precision using the `tolerance` parameter (default: `1e-7`).
- Maximum iteration limit can be customized (default: `100`).
- Detects invalid inputs like negative numbers and outputs appropriate error messages.

### Requirements
- Python 3.6+

No additional libraries are required.

## Usage

### Running the Script
1. Clone the repository:
   ```bash
   git clone https://github.com/misbah-ullah01/bisection-square-root-method.git
   ```
2. Navigate to the project directory:
   ```bash
   cd bisection-square-root-method
   ```
3. Run the script:
   ```bash
   python bisection_square_root.py
   ```
4. Enter a non-negative number when prompted to calculate its square root.

### Example Output
```bash
Please enter a number to Find Square Root: 25
The square root of 25 is approximately 5.0
```

### Function Overview
#### `square_root_bisection(square_target, tolerance=1e-7, max_iterations=100)`
- **Parameters:**
  - `square_target`: The number whose square root is to be approximated (must be non-negative).
  - `tolerance`: The acceptable error margin for the approximation (default: `1e-7`).
  - `max_iterations`: The maximum number of iterations to prevent infinite loops (default: `100`).
- **Returns:**
  - The approximated square root of `square_target`.
- **Raises:**
  - `ValueError` for negative inputs.

### Edge Cases Handled
- Input is 0 or 1: Returns 0 or 1 directly.
- Negative input: Raises an exception since square roots of negative numbers are not defined in the real number system.
- Non-convergence: Prints a failure message if the method does not converge within the maximum allowed iterations.

## Contributing
Contributions are welcome! If you have suggestions for improving the code or documentation, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Author
**Misbah Ullah**

GitHub: [misbah-ullah01](https://github.com/misbah-ullah01)

