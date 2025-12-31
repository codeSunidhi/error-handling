<div align="center">

# 🐍 Python Error Handling & Modules 🛡️

### 🎯 Master Exception Handling in Python 🎯

[![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/codeSunidhi/error-handling)

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=28&pause=1000&color=F75C7E&center=true&vCenter=true&width=600&lines=Learn+Error+Handling!+%F0%9F%9A%80;Master+Python+Exceptions!+%E2%9A%A1;Build+Robust+Applications!+%F0%9F%92%AA" alt="Typing SVG" />

</div>

---

## 📚 About This Repository

Welcome to the **Python Error Handling & Modules** repository! This is a comprehensive collection of Python programs demonstrating various types of exceptions, error handling techniques, and module usage. Perfect for students and developers learning to write robust, error-free Python code! 🎓

### 🎯 Learning Objectives

- 🔍 Understand different types of Python exceptions
- 🛠️ Learn proper error handling techniques
- 🧩 Master Python modules and packages
- 💡 Write more reliable and maintainable code
- 🚀 Debug programs effectively

---

## ✨ Features

🎨 **Comprehensive Coverage**
- All major Python exception types
- Real-world error scenarios
- Practical examples and demonstrations

📖 **Educational Focus**
- Clear, commented code
- Each file demonstrates a specific error type
- Learn through practical examples

🔧 **Hands-on Learning**
- Run and experiment with code
- See errors in action
- Understand exception handling flow

---

## 📂 Repository Structure

```
error-handling/
│
├── 🔴 Error Type Demonstrations
│   ├── zerodiv.py              # ZeroDivisionError handling
│   ├── value_error.py          # ValueError examples
│   ├── name_error.py           # NameError demonstrations
│   ├── index_error.py          # IndexError handling
│   ├── key_error.py            # KeyError examples
│   ├── attribute_error.py      # AttributeError cases
│   ├── FOF_error.py            # FileNotFoundError handling
│   ├── module_error.py         # ModuleNotFoundError examples
│   └── multiple_error.py       # Multiple exception handling
│
├── 🧩 Module & Package Examples
│   ├── my_package.py           # Custom package creation
│   ├── call.py                 # Module calling examples
│   ├── m4.py                   # Module demonstration 4
│   └── m5.py                   # Module demonstration 5
│
├── 📦 Data Structure Programs
│   ├── list1.py                # List operations
│   ├── dict3.py                # Dictionary operations
│   └── set2.py                 # Set operations
│
└── 📖 README.md                # This file!
```

---

## 🐛 Exception Types Covered

<div align="center">

| Exception | File | Description |
|-----------|------|-------------|
| 🔢 **ZeroDivisionError** | `zerodiv.py` | Division by zero scenarios |
| 💯 **ValueError** | `value_error.py` | Invalid value conversions |
| 📛 **NameError** | `name_error.py` | Undefined variable references |
| 📍 **IndexError** | `index_error.py` | List/array index out of range |
| 🔑 **KeyError** | `key_error.py` | Dictionary key not found |
| 🏷️ **AttributeError** | `attribute_error.py` | Invalid object attributes |
| 📁 **FileNotFoundError** | `FOF_error.py` | File operations on missing files |
| 📦 **ModuleNotFoundError** | `module_error.py` | Import errors |
| 🎭 **Multiple Exceptions** | `multiple_error.py` | Handling various errors |

</div>

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python installed on your system:

```bash
python --version
```

**Recommended:** Python 3.6 or higher 🐍

### Installation

1️⃣ **Clone the repository**
```bash
git clone https://github.com/codeSunidhi/error-handling.git
```

2️⃣ **Navigate to the directory**
```bash
cd error-handling
```

3️⃣ **You're ready to go!** 🎉

---

## 💻 Usage Examples

### Running Individual Programs

```bash
# Example: Run the ZeroDivisionError demonstration
python zerodiv.py

# Example: Run the ValueError demonstration
python value_error.py

# Example: Run the multiple error handling example
python multiple_error.py
```

### Basic Error Handling Pattern

```python
try:
    # Code that might raise an exception
    result = 10 / 0
except ZeroDivisionError:
    # Handle the specific error
    print("Error: Cannot divide by zero!")
except Exception as e:
    # Catch any other exceptions
    print(f"An error occurred: {e}")
finally:
    # Code that always executes
    print("Execution completed")
```

---

## 📖 Learning Path

### 🟢 Beginner Level
1. Start with `zerodiv.py` - Understand basic try-except
2. Move to `value_error.py` - Learn type conversion errors
3. Try `name_error.py` - Understand variable scope

### 🟡 Intermediate Level
4. Explore `index_error.py` - Master list operations
5. Study `key_error.py` - Handle dictionary errors
6. Check `attribute_error.py` - Object attribute handling

### 🔴 Advanced Level
7. Examine `FOF_error.py` - File handling errors
8. Review `module_error.py` - Import and module errors
9. Master `multiple_error.py` - Complex error scenarios

### 🎓 Module Programming
10. Study `my_package.py` - Create custom packages
11. Practice with `call.py` - Module interactions

---

## 🔍 Code Examples

### Example 1: ZeroDivisionError

```python
try:
    num1 = int(input("Enter first number: "))
    num2 = int(input("Enter second number: "))
    result = num1 / num2
    print(f"Result: {result}")
except ZeroDivisionError:
    print("❌ Error: Cannot divide by zero!")
except ValueError:
    print("❌ Error: Please enter valid numbers!")
```

### Example 2: FileNotFoundError

```python
try:
    with open('data.txt', 'r') as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("❌ Error: File not found!")
except PermissionError:
    print("❌ Error: Permission denied!")
```

### Example 3: Multiple Exception Handling

```python
def safe_divide(a, b):
    try:
        result = a / b
        return result
    except ZeroDivisionError:
        return "Cannot divide by zero"
    except TypeError:
        return "Invalid data types"
    except Exception as e:
        return f"An error occurred: {e}"
```

---

## 🛠️ Best Practices

✅ **DO's**
- Always use specific exception types
- Provide meaningful error messages
- Use `finally` for cleanup code
- Log errors for debugging
- Handle exceptions at appropriate levels

❌ **DON'Ts**
- Don't use bare `except:` clauses
- Don't suppress errors silently
- Don't catch exceptions you can't handle
- Don't use exceptions for flow control

---

## 🎯 Key Concepts

### Try-Except-Finally Block

```python
try:
    # Code that might raise an exception
    risky_operation()
except SpecificError:
    # Handle specific error
    handle_error()
else:
    # Executes if no exception occurred
    success_action()
finally:
    # Always executes
    cleanup()
```

### Custom Exceptions

```python
class CustomError(Exception):
    """Custom exception for specific use cases"""
    pass

try:
    raise CustomError("Something went wrong!")
except CustomError as e:
    print(f"Custom error caught: {e}")
```

---

## 📊 Program Categories

<div align="center">

### 🎯 Error Handling Programs
![Python](https://img.shields.io/badge/Programs-9-blue?style=flat-square)

### 🧩 Module Examples
![Python](https://img.shields.io/badge/Programs-4-green?style=flat-square)

### 📦 Data Structures
![Python](https://img.shields.io/badge/Programs-3-orange?style=flat-square)

</div>

---

## 🤝 Contributing

Contributions are welcome! Help make this learning resource even better! 🌟

### How to Contribute

1. 🍴 Fork the repository
2. 🌱 Create a feature branch
   ```bash
   git checkout -b feature/new-error-example
   ```
3. 💾 Commit your changes
   ```bash
   git commit -m "Add new error handling example"
   ```
4. 📤 Push to the branch
   ```bash
   git push origin feature/new-error-example
   ```
5. 🎉 Open a Pull Request

### Contribution Ideas

- 💡 Add new exception types
- 📝 Improve documentation
- 🐛 Fix bugs or typos
- ✨ Add more real-world examples
- 🎨 Enhance code comments

---

## 📚 Additional Resources

### 📖 Documentation
- [Python Official Docs - Errors and Exceptions](https://docs.python.org/3/tutorial/errors.html)
- [PEP 8 - Style Guide](https://peps.python.org/pep-0008/)
- [Python Exception Hierarchy](https://docs.python.org/3/library/exceptions.html)

### 🎓 Learning Resources
- Python error handling tutorials
- Exception handling best practices
- Debugging techniques in Python

---

## 🏆 Skills Gained

After working through this repository, you'll be able to:

- ✅ Identify and handle different exception types
- ✅ Write robust error-handling code
- ✅ Debug Python programs effectively
- ✅ Create custom exceptions
- ✅ Use try-except-finally blocks properly
- ✅ Work with Python modules and packages
- ✅ Build more reliable applications

---

## 📬 Contact

<div align="center">

**Sunidhi Raturi**

📧 Email: [sunidhiraturi1@gmail.com](mailto:sunidhiraturi1@gmail.com)

💼 LinkedIn: [sunidhi-raturi-08b7b9362](https://www.linkedin.com/in/sunidhi-raturi-08b7b9362/)

🌐 Portfolio: [portfolio-flax-psi-54.vercel.app](https://portfolio-flax-psi-54.vercel.app)

📱 GitHub: [@codeSunidhi](https://github.com/codeSunidhi)

</div>

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- 💙 Thanks to the Python community for excellent documentation
- 📚 Inspired by real-world programming challenges
- 🎓 Created for educational purposes at Doon University

---

## 📊 Repository Stats

<div align="center">

![GitHub repo size](https://img.shields.io/github/repo-size/codeSunidhi/error-handling?style=for-the-badge&color=blue)
![GitHub language count](https://img.shields.io/github/languages/count/codeSunidhi/error-handling?style=for-the-badge&color=green)
![GitHub last commit](https://img.shields.io/github/last-commit/codeSunidhi/error-handling?style=for-the-badge&color=red)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/codeSunidhi/error-handling?style=for-the-badge&color=orange)

</div>

---

## 🎮 Quick Reference

### Common Exception Types Cheatsheet

| Exception | When It Occurs | How to Handle |
|-----------|---------------|---------------|
| `ZeroDivisionError` | Dividing by zero | Check divisor before operation |
| `ValueError` | Invalid value conversion | Validate input before conversion |
| `NameError` | Using undefined variable | Check variable initialization |
| `IndexError` | List index out of range | Check list length |
| `KeyError` | Dictionary key missing | Use `.get()` or check key existence |
| `TypeError` | Wrong data type | Validate type before operation |
| `FileNotFoundError` | File doesn't exist | Check file existence first |
| `ImportError` | Module import fails | Verify module installation |

---

<div align="center">

### 💖 Happy Coding & Learning! 🚀

**⭐ If this repository helped you learn, please star it! ⭐**

<img src="https://raw.githubusercontent.com/BEPb/BEPb/master/assets/Bottom_up.svg" alt="Footer" />

**Made with ❤️ and Python by Sunidhi Raturi** © 2025

</div>
