# Hello Java Maven - Jenkins Build

## Task Overview
This project is part of the DevOps Internship Task 8: Run a Simple Java Maven Build Job in Jenkins.  
The goal was to create a basic Java Maven project and build it using Jenkins.

---

## Project Structure
```

hello-java-maven/
├── pom.xml
└── src/
└── main/java/HelloWorld.java

````
## Steps Performed

1. Created a **HelloWorld Java program**.
2. Created a **Maven `pom.xml`** file to compile and package the Java code.
3. Configured Jenkins:

   * Installed Maven via **Global Tool Configuration**.
   * Added a Freestyle project: `HelloJavaMaven`.
4. Added **Build Step → Invoke top-level Maven targets**:

   * Maven Version: `Maven 3.8.11` (or your version)
   * Root POM: `pom.xml`
   * Goals: `clean package`
5. Copied local project files (`pom.xml` + `src/`) into Jenkins **workspace**.
6. Clicked **Build Now** → Verified `BUILD SUCCESS` in Console Output.
7. Optional: Archived `target/*.jar` as a build artifact.

---

## Outcome

* Successfully built a Java Maven project using Jenkins.
* Learned:

  * How to configure Maven in Jenkins
  * How to create a Freestyle Jenkins job
  * How to debug Maven build errors
  * How to archive artifacts after a successful build

---

## Screenshot
(/jenkin.png)

---

## Notes

* Local files need to be available in Jenkins workspace for Maven builds.
* Using **custom workspace** or **copying files** are both valid approaches.

```

---

If you want, I can also **prepare a folder structure with this README, pom.xml, src/** fully ready to push to GitHub so you can submit immediately. Do you want me to do that?
```
