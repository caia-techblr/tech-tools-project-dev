
# 🖥️ Visual Studio Code: Download and Install with Python & Java Plugins

This guide helps you **download**, **install**, and **set up Visual Studio Code (VS Code)** with the essential extensions for **Python** and **Java** development.

---

## 📥 1. Download Visual Studio Code

1. Go to the official [Visual Studio Code website](https://code.visualstudio.com/)
2. Click **Download for Windows** (or select your OS: macOS/Linux)
3. Run the installer and follow the steps:
   - Accept the license agreement
   - Choose install location
   - Enable “Add to PATH” and “Open with Code” options
   - Click **Install**

✅ Once installed, launch **VS Code**

---

## 🧩 2. Install Python Plugin in VS Code

1. Open **VS Code**
2. Go to Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for: **Python**
4. Select the extension by **Microsoft**
5. Click **Install**

You will also be prompted to install **Pylance** for better IntelliSense support.

🔹 **Optional but Recommended**:
- Python Extension Pack
- Jupyter (for working with `.ipynb` notebooks)

---

## ☕ 3. Install Java Plugin in VS Code

1. Go to Extensions view (`Ctrl+Shift+X`)
2. Search for: **Extension Pack for Java**
3. Click **Install**

This pack includes:
- Language Support for Java™ by Red Hat
- Debugger for Java
- Java Test Runner
- Maven for Java
- Java Dependency Viewer

🔹 You can also install:
- Spring Boot Extension Pack (for Spring apps)
- Maven Extension (separately, if needed)

---

## ⚙️ 4. Configure Your Environments

### Python Setup

Make sure **Python 3.10+** is installed from:
👉 https://www.python.org/downloads/

- After installing, restart VS Code
- Open Command Palette (`Ctrl+Shift+P`) → `Python: Select Interpreter` → Choose installed Python version
- To run Python files:
  - Open any `.py` file
  - Click **Run Python File in Terminal**

---

### Java Setup

Install the **Java Development Kit (JDK)** from:
👉 https://adoptium.net/

Ensure environment variable `JAVA_HOME` is set.

- After installing, restart VS Code
- Open Command Palette → `Java: Configure Java Runtime` to verify setup
- Create a Java file (e.g., `Main.java`) and run it using the **Run** icon above the `main()` method

---

## 🧪 5. Sample Files to Test

### Python
```python
# hello.py
print("Hello from Python in VS Code!")
```

### Java
```java
// Main.java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello from Java in VS Code!");
    }
}
```

---

## 🧰 6. Troubleshooting Tips

| Issue                        | Fix |
|-----------------------------|-----|
| Python not found            | Install Python and restart VS Code |
| Java not detected           | Install JDK and set JAVA_HOME |
| Extensions not loading      | Reload window or reinstall the extension |
| Code not running            | Use integrated terminal or check interpreter/JDK setup |

---

## 📚 References

- [VS Code Documentation](https://code.visualstudio.com/docs)
- [Python in VS Code](https://code.visualstudio.com/docs/python/python-tutorial)
- [Java in VS Code](https://code.visualstudio.com/docs/java/java-tutorial)

---

> 🎉 You’re all set! Start coding with confidence in Python and Java using VS Code.
