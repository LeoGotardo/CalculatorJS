# Simple JavaScript Calculator

This project is a simple JavaScript-based calculator that allows users to perform basic arithmetic operations such as addition, subtraction, multiplication, and division. The calculator's interface is managed via HTML with operations handled through JavaScript, offering a straightforward and interactive user experience.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Dependencies](#dependencies)
- [Configuration](#configuration)
- [Documentation](#documentation)
- [Examples](#examples)
- [Contributors](#contributors)
- [License](#license)

## Installation

To install this calculator, simply clone the repository to your local machine:

```bash
git clone https://github.com/LeoGotardo/CalculatorJS/
cd CalculatorJS
```

Open the `index.html` file in a web browser to start using the calculator.

## Usage

To use the calculator:

1. Open the `index.html` file in any web browser.
2. Click on the buttons on the calculator to perform operations.

## Features

- **Basic Arithmetic Operations**: Perform addition, subtraction, multiplication, and division.
- **Continuous Operations**: Chain multiple operations together.
- **Decimal Support**: Perform decimal calculations.
- **Clear and Delete**: Clear the current input or all entries, and delete the last entered digit.

## Dependencies

This project does not rely on any external libraries or frameworks and only requires a modern web browser with JavaScript support.

## Configuration

No additional configuration is required to start using this calculator.

## Documentation

Detailed documentation on how the calculator processes operations can be found in the source code comments.

## Examples

```javascript
// Example of initializing the calculator
const calc = new Calculator(previousOperationText, currentOperationText);

// Example of handling button clicks
buttons.forEach(btn => {
    btn.addEventListener("click", (e) => {
        const value = e.target.innerText;
        if(+value >= 0 || value === ".") {
            calc.addDigt(value);
        }
        else {
            calc.processOperation(value);
        }
    });
});
```

## Contributors

- [Your Name](https://your-profile-url.com)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
