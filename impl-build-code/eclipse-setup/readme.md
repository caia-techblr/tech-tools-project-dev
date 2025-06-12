
# 🌟 Installing Eclipse IDE with Java and Python Plugins

This guide will help you **download**, **install**, and **configure Eclipse IDE** for both **Java** and **Python** development.

---

## 📥 1. Download and Install Eclipse

1. Go to: [https://www.eclipse.org/downloads/](https://www.eclipse.org/downloads/)
2. Click **Download** for "Eclipse IDE for Java Developers"
3. Run the installer:
   - Choose **Eclipse IDE for Java Developers**
   - Follow prompts and install to default location
   - Launch Eclipse after installation

---

## ☕ 2. Java Plugin (Built-In)

The Eclipse IDE for Java Developers already includes Java support:

### Create a Java Project
1. Go to **File** → **New** → **Java Project**
2. Name your project (e.g., `MyJavaProject`)
3. Add a class: `File → New → Class`
4. Write your code and click **Run**

### Sample Java Code
```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello from Java in Eclipse!");
  }
}
```

---

## 🐍 3. Add Python Support (PyDev Plugin)

### Install PyDev Plugin
1. Go to **Help** → **Eclipse Marketplace**
2. Search for **PyDev**
3. Click **Install** → Accept license → Restart Eclipse when prompted

### Configure Python Interpreter
1. Go to **Window** → **Preferences**
2. Navigate to **PyDev** → **Interpreters** → **Python Interpreter**
3. Click **New** and browse to your Python executable (`python.exe` or `/usr/bin/python3`)
4. Apply and Close

---

## 🐍 Create a Python Project

1. Go to **File** → **New** → **Project**
2. Choose **PyDev Project** under **PyDev**
3. Set project name and interpreter
4. Add a new Python file: `right-click → New → PyDev Module`

### Sample Python Code
```python
print("Hello from Python in Eclipse!")
```

---

## 🧰 4. Troubleshooting

| Issue                     | Fix |
|--------------------------|-----|
| PyDev not visible        | Ensure plugin was installed from Eclipse Marketplace |
| Interpreter not found    | Manually add Python in Preferences |
| Java errors              | Check JDK installation and build path configuration |

---

## 📚 References

- [Eclipse Downloads](https://www.eclipse.org/downloads/)
- [PyDev Website](http://www.pydev.org/)
- [Eclipse Marketplace](https://marketplace.eclipse.org/)

---

> ✅ You are now ready to develop Java and Python applications using Eclipse IDE!
