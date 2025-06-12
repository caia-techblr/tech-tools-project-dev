
# ⚙️ Integrating Apache Maven with Installed Eclipse IDE

If you already have **Eclipse IDE** installed, this guide helps you set up and use **Apache Maven** for Java project development.

---

## 🔍 1. Verify Maven Plugin (M2E) in Eclipse

Maven support (via **M2E plugin**) is usually pre-installed.

### To Check:
1. Open Eclipse
2. Go to **File** → **New** → **Other**
3. Search for **Maven Project**

If **Maven** options appear, you're good to go!

> ❗ If not available:
- Go to **Help** → **Eclipse Marketplace**
- Search for: **Maven Integration for Eclipse (m2e)**
- Click **Install** → Restart Eclipse

---

## 📁 2. Create a New Maven Project

1. Go to **File** → **New** → **Other**
2. Select **Maven** → **Maven Project**
3. Click **Next**
4. You can either:
   - Select an archetype (like `maven-archetype-quickstart`)
   - Or check **Create a simple project (skip archetype selection)**
5. Fill in:
   - **Group Id**: com.example
   - **Artifact Id**: myapp
6. Click **Finish**

---

## 🧾 3. Example Project Structure

```
myapp/
├── pom.xml
└── src/
    ├── main/
    │   └── java/
    │       └── com/example/App.java
    └── test/
        └── java/
```

---

## 🧾 4. Sample `pom.xml`

```xml
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0
         http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>myapp</artifactId>
    <version>1.0-SNAPSHOT</version>

    <dependencies>
        <dependency>
            <groupId>org.apache.commons</groupId>
            <artifactId>commons-lang3</artifactId>
            <version>3.12.0</version>
        </dependency>
    </dependencies>
</project>
```

---

## 🚀 5. Build and Run the Maven Project

### Build the project:
- Right-click the project → **Run As** → **Maven build...**
- Enter goal: `clean install`

### Run the Java application:
- Right-click `App.java` → **Run As** → **Java Application**

---

## 🔄 6. Update Maven Dependencies

After editing `pom.xml`:

- Right-click the project
- Select **Maven** → **Update Project**
- Click **OK**

---

## 🧰 7. Troubleshooting

| Issue                          | Fix |
|-------------------------------|-----|
| Maven not available            | Install M2E plugin from Eclipse Marketplace |
| Dependencies not resolving     | Use "Update Project" under Maven menu |
| Build errors                   | Clean project: `Project` → `Clean...` |
| Java class not running         | Ensure correct class has a `main()` method |

---

## 📚 Resources

- [Apache Maven](https://maven.apache.org/)
- [Eclipse IDE](https://www.eclipse.org/)
- [M2E Plugin Documentation](https://www.eclipse.org/m2e/)

---

> ✅ Maven is now integrated with Eclipse. You're ready to develop and manage Java projects efficiently!
