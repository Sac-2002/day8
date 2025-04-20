# day8
🚀 Jenkins CI/CD Pipeline with Maven: Build and Test Setup
📌 Overview
This project demonstrates how to set up a basic Jenkins pipeline that uses Maven to build and test a Java application. It covers integration of Jenkins with a Git repository and automates the clean, test, and package phases of the Maven lifecycle.

🧰 Tools & Technologies
Jenkins

Maven

Java (Sample App)

GitHub (for source code)

🛠️ Jenkins Job Configuration
1. Create a Freestyle Project
Go to Jenkins dashboard → New Item → Freestyle project → Name your job → Click OK

2. Configure Source Code Management (SCM)
Select Git

Enter your repository URL (e.g., https://github.com/your-username/your-repo.git)

Add credentials if needed

3. Add Build Step
Go to the Build section

Click Add build step → Invoke top-level Maven targets

In the Goals field, enter:

bash
Copy
Edit
clean test package
4. Save and Build
Click Save

Then click Build Now

Monitor the Console Output to ensure everything runs smoothly

✅ Expected Output
Jenkins will clone the repo

Run Maven commands:

clean: Cleans old compiled files

test: Runs all unit tests

package: Creates a .jar or .war file

Console output should show all green if successful ✅

📁 Project Structure (Example)
css
Copy
Edit
your-project/
├── src/
│   └── main/
│       └── java/
│   └── test/
│       └── java/
├── pom.xml
