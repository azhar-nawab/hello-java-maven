
---

## 🔧 Prerequisites

- Java (JDK 8+)
- Maven (e.g., Maven 3.x)
- Git
- Jenkins server installed

---

## 🚀 Jenkins Setup (Freestyle Project)

1. **Create New Job**:  
   - Jenkins Dashboard → `New Item` → Enter name `hello-java-maven` → Choose `Freestyle project`

2. **Configure Source Code Management**:  
   - Git Repository URL: `https://github.com/azhar-nawab/hello-java-maven.git`

3. **Build Environment**:  
   - Add `Delete workspace before build starts` (optional but recommended)

4. **Build Configuration**:  
   - Add build step: `Invoke top-level Maven targets`
   - Goals: `clean package`

5. **Post-build Actions**:  
   - Publish JUnit test result report
   - Test report XMLs: `**/target/surefire-reports/*.xml`

---

## ✅ Example Output

**Screenshot of successful Jenkins build console output:**

> 📸 _Include your console output screenshot here_

---
## 📁 Project Structure

<pre lang="markdown"> ## 🗂️ Project Structure ``` hello-java-maven/ ├── pom.xml └── src/ ├── main/ │ └── java/ │ └── com/ │ └── example/ │ └── HelloWorld.java └── test/ └── java/ └── com/ └── example/ └── HelloTest.java ``` </pre>
