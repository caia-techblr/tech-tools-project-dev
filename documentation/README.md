# 📝 Documentation Best Practices

This guide provides a concise overview of creating professional documentation using **Confluence**, **Markdown**, and tools that generate documentation from code comments like **Javadoc**, **Pydoc**, and **Doxygen**.

---

## 📘 1. Documentation Using Confluence

[Confluence](https://www.atlassian.com/software/confluence) is a popular team collaboration platform by Atlassian used for:

- Creating technical documentation
- Writing how-to guides and SOPs
- Managing project wikis

### Key Features:
- Rich-text editor with macros and templates
- Page versioning and comment threads
- Integration with Jira and other Atlassian tools

### Tips:
- Use templates (e.g., “Product Requirements,” “Project Plan”)
- Organize pages in a tree hierarchy for navigation
- Restrict access for sensitive documentation

---

## 🧾 2. Markdown Syntax for GitHub Documentation

Markdown (`.md` files) is widely used for GitHub wikis, READMEs, and project documentation.

### Common Syntax:

| Feature        | Markdown Syntax                    |
|----------------|-------------------------------------|
| Heading        | `#`, `##`, `###`, etc.             |
| Bold           | `**bold**`                         |
| Italic         | `*italic*`                         |
| Code Block     | ```language ... ```                |
| Link           | `[text](url)`                      |
| Image          | `![alt text](image_url)`           |
| List           | `- item`, `1. item`                |
| Table          | `| Col1 | Col2 | \n |------|------|`  |

### Example README:

```markdown
# MyProject

## Description
A short description of the project.

## Installation
```bash
pip install myproject
```

## Usage
```python
from myproject import start
start()
```
```

---

## 🧠 3. Generate Documentation from Code Comments

Automated tools can generate HTML or PDF documentation directly from annotated source code.

### 🔹 Javadoc (for Java)

```java
/**
 * This is a sample class.
 * @author John
 * @version 1.0
 */
public class Sample {}
```

**Command:**
```bash
javadoc -d docs/ Sample.java
```

### 🔹 Pydoc (for Python)

```python
def add(x, y):
    """
    Adds two numbers.

    :param x: int
    :param y: int
    :return: int
    """
    return x + y
```

**Command:**
```bash
pydoc -w mymodule.py
```

### 🔹 Doxygen (for C, C++, Java, Python, etc.)

```cpp
/**
 * Adds two integers.
 * @param a First integer
 * @param b Second integer
 * @return Sum
 */
int add(int a, int b);
```

**Steps:**
1. Create a `Doxyfile`:
```bash
doxygen -g
```

2. Configure input/output in the `Doxyfile`

3. Run:
```bash
doxygen Doxyfile
```

---

## 📚 References

- [Confluence Documentation](https://support.atlassian.com/confluence/)
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)
- [Javadoc Tool](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javadoc.html)
- [Pydoc](https://docs.python.org/3/library/pydoc.html)
- [Doxygen](https://www.doxygen.nl/)

---

> ✅ Use these tools and formats to maintain clear, maintainable, and professional project documentation.
