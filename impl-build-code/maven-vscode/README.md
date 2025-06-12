
# ⚙️ Integrating Apache Maven with Visual Studio Code

This guide explains how to set up and use **Apache Maven** with **Visual Studio Code** for Java development.

---

## 📥 1. Prerequisites

Before integrating Maven with VS Code, make sure the following are installed:

### ✅ Java Development Kit (JDK)
- Recommended: JDK 17 or newer
- Download from: https://adoptium.net/
- Set the environment variable `JAVA_HOME` properly

### ✅ Apache Maven
- Download from: https://maven.apache.org/download.cgi
- Extract and add the `bin` directory to your system `PATH`

To verify:
```bash
mvn -version
```

---

## 🖥️ 2. Download & Install Visual Studio Code

- Download: https://code.visualstudio.com/
- Install and launch

---

## 🧩 3. Install Maven Extension in VS Code

1. Open **VS Code**
2. Go to Extensions (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for **Maven for Java**
4. Install the extension by **Microsoft**

---

## 🛠️ 4. Create or Open a Maven Project

### Option A: Create using Maven CLI
```bash
mvn archetype:generate -DgroupId=com.example -DartifactId=myapp -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

Then open the folder in VS Code.

### Option B: Use VS Code Maven Project Explorer
- Open Command Palette → `Maven: Create Maven Project`
- Follow prompts to generate a project

---

## 📁 5. Recommended Project Structure

```
myapp/
├── pom.xml
└── src/
    ├── main/
    │   └── java/
    │       └── com/example/App.java
    └── test/
        └── java/
            └── com/example/AppTest.java
```

---

## 🚀 6. Building and Running

### Use Maven Commands in Terminal
```bash
mvn clean install
mvn compile
mvn exec:java -Dexec.mainClass="com.example.App"
```

### Or Use Maven Extension
- Open **Maven Projects** sidebar
- Right-click lifecycle goals: `clean`, `install`, `package`, etc.

---

## 🧪 7. Sample `pom.xml`

```xml
<project xmlns="http://maven.apache.org/POM/4.0.0" ...>
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

## 🧰 8. Troubleshooting Tips

| Issue                        | Fix |
|-----------------------------|-----|
| Maven not found             | Ensure `mvn` is in your PATH |
| Java not detected           | Check JAVA_HOME and reinstall JDK |
| Project not detected        | Open the root folder with `pom.xml` |
| Maven goals not working     | Use the integrated terminal or reinstall extension |

---

## 📚 Resources

- [Maven Official Site](https://maven.apache.org/)
- [VS Code Java Guide](https://code.visualstudio.com/docs/java/java-project)
- [VS Code Maven Extension](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-maven)

---

> 🎉 You're now ready to build and manage Java projects with Maven in VS Code!
