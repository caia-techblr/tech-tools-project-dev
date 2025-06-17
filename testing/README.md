
# ✅ Testing in VS Code and Eclipse

This guide covers how to write and run tests for **Java (using Maven & JUnit)** and **Python (using pytest)** in both **VS Code** and **Eclipse**.

---

## ☕ Java Testing with Maven (JUnit)

### 📁 Maven Directory Structure

```
my-java-app/
├── pom.xml
└── src/
    ├── main/java/
    │   └── com/example/App.java
    └── test/java/
        └── com/example/AppTest.java
```

### 📦 Add JUnit to `pom.xml`

```xml
<dependencies>
  <dependency>
    <groupId>org.junit.jupiter</groupId>
    <artifactId>junit-jupiter</artifactId>
    <version>5.9.2</version>
    <scope>test</scope>
  </dependency>
</dependencies>
```

### 🧪 Example JUnit Test

```java
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.assertEquals;

public class AppTest {
    @Test
    void testAdd() {
        assertEquals(4, 2 + 2);
    }
}
```

### ▶ Run Tests

- **VS Code**:
  - Right-click on test → Run Test
  - Or run `mvn test` in the terminal

- **Eclipse**:
  - Right-click → Run As → JUnit Test
  - Or project → Run As → Maven test

---

## 🐍 Python Testing with pytest

### 📁 Python Directory Structure

```
my-python-app/
├── main.py
├── app/
│   └── utils.py
└── tests/
    └── test_utils.py
```

### 🧪 Sample Test File (`tests/test_utils.py`)

```python
def add(x, y):
    return x + y

def test_add():
    assert add(2, 3) == 5
```

### ▶ Install and Run pytest

```bash
pip install pytest
pytest
```

### 📌 VS Code Setup for Python Testing

1. Install **Python** and **pytest** via pip
2. Open Command Palette → `Python: Configure Tests`
3. Choose `pytest` as the framework
4. Use the **Testing Sidebar** to run and debug tests

---

## 🧩 Eclipse with PyDev (Optional for Python)

1. Install **PyDev** via Eclipse Marketplace
2. Configure Python Interpreter: Preferences → PyDev → Interpreters
3. Create test files with `test_*.py` naming
4. Right-click test file → Run As → Python unit-test

---

## 📚 References

- [JUnit 5 Guide](https://junit.org/junit5/docs/current/user-guide/)
- [pytest Docs](https://docs.pytest.org/)
- [VS Code Java Testing](https://code.visualstudio.com/docs/java/java-testing)
- [VS Code Python Testing](https://code.visualstudio.com/docs/python/testing)

---

> ✅ You’re now ready to write, run, and automate unit tests in both Java and Python projects using industry-standard tools!
