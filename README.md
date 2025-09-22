📋 Project Overview
This project implements an advanced calculator with memory functions, calculation history, and comprehensive unit tests. The calculator supports basic arithmetic operations, power functions, square roots, percentages, and memory operations.

🚀 Features
Core Calculator Functions
Basic Operations: Addition, Subtraction, Multiplication, Division

Advanced Operations: Power, Square Root, Percentage

Memory Operations: Store, Recall, Add to Memory, Subtract from Memory

Calculation History: Track all operations with results

Error Handling: Division by zero, negative square roots

Testing Features
Unit Test Coverage: 100% of calculator methods

Edge Case Testing: Division by zero, negative inputs

Mock Testing: Input/Output simulation

Integration Testing: Menu system and user interaction

Boundary Testing: Extreme values and error conditions

🛠️ Installation
bash
# Clone the repository
git clone https://github.com/yourusername/calculator-project.git
cd calculator-project

# No additional dependencies required
# Uses only Python standard library

📁 Project Structure
text
calculator-project/
│
├── calculator.py          # Main calculator implementation
├── test_calculator.py     # Comprehensive test suite
├── README.md             # Project documentation
└── requirements.txt      # Python dependencies

🧪 Running Tests
Run All Tests
bash
python -m unittest test_calculator.py
Run Tests with Verbose Output
bash
python -m unittest test_calculator.py -v

Run Specific Test Methods
bash
python -m unittest test_calculator.TestCalculator.test_add
python -m unittest test_calculator.TestCalculator.test_divide

📊 Test Coverage
The test suite covers:

Unit Tests
✅ Basic arithmetic operations (add, subtract, multiply, divide)

✅ Advanced mathematical functions (power, square root, percentage)

✅ Memory operations (store, recall, clear)

✅ History tracking functionality

✅ Error handling and edge cases

Integration Tests
✅ User menu interaction

✅ Input validation

✅ Screen clearing functionality

✅ Full workflow testing

Special Test Cases
✅ Division by zero handling

✅ Negative square root detection

✅ Memory persistence between operations

✅ History accuracy and ordering

🎯 Usage Examples
Basic Calculator Usage
python
from calculator import Calculator

calc = Calculator()

# Basic operations
result = calc.add(5, 3)        # 8
result = calc.multiply(4, 2.5) # 10.0

# Memory operations
calc.memory_add(10)
calc.memory_subtract(5)
current_memory = calc.memory_recall()  # 5

# View history
calc.show_history()

Running the Interactive Calculator
bash
python calculator.py


🔧 Technical Details
Dependencies
Python 3.6+

Standard library only (no external dependencies)

Key Components
Calculator Class
Memory Management: Persistent storage with operations

History Tracking: Complete operation log

Error Handling: Robust exception management

Type Hints: Full type annotation support

Test Suite
unittest Framework: Python's built-in testing framework

Mock Objects: Simulated user input and system calls

Assertion Methods: Comprehensive result validation

Test Isolation: Independent test execution


🧪 Testing Methodology
Test Types Implemented
Unit Tests

Individual method functionality

Return value verification

Side effect testing (history updates)

Integration Tests

Method interaction

Menu system workflow

User input processing

Edge Case Tests

Boundary conditions

Error scenarios

Invalid input handling


Test Structure
python
def test_method_name(self):
    # Setup
    test_input = ...
    expected_output = ...
    
    # Execution
    actual_output = self.calc.method_name(test_input)
    
    # Verification
    self.assertEqual(actual_output, expected_output)



    📈 Test Results Example
text
test_add (test_calculator.TestCalculator) ... ok
test_divide (test_calculator.TestCalculator) ... ok
test_edge_cases (test_calculator.TestCalculator) ... ok
test_get_valid_number (test_calculator.TestCalculator) ... ok
test_history (test_calculator.TestCalculator) ... ok
test_main_menu_add_operation (test_calculator.TestCalculator) ... ok
test_memory_operations (test_calculator.TestCalculator) ... ok
test_multiply (test_calculator.TestCalculator) ... ok
test_power (test_calculator.TestCalculator) ... ok
test_square_root (test_calculator.TestCalculator) ... ok
test_subtract (test_calculator.TestCalculator) ... ok

----------------------------------------------------------------------
Ran 11 tests in 0.015s

OK



🐛 Bug Reports
If you find any issues, please report them with:

Python version

Operating system

Steps to reproduce

Expected vs actual behavior

🤝 Contributing
Fork the repository

Create a feature branch

Add tests for new functionality

Ensure all tests pass

Submit a pull request

📄 License
This project is open source and available under the MIT License.



🏆 Best Practices Demonstrated
Test-Driven Development: Comprehensive test coverage

Code Quality: Type hints and documentation

Error Handling: Robust exception management

Modular Design: Separated concerns and reusable components

CI/CD Ready: Easy to integrate with automation pipelines

⭐ Star this repository if you find it helpful!

