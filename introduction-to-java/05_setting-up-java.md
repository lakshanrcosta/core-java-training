# 🚀 Setting up the Java Development Environment (JDK, JRE, JVM)

Java requires a proper development environment to write, compile, and run Java programs. The **Java Development Kit (JDK)** includes everything needed for Java development, including the **Java Runtime Environment (JRE)** and the **Java Virtual Machine (JVM)**.

---

## 📌 **Understanding Java Components**
Before installation, let's clarify the key Java components:

- **JDK (Java Development Kit)** → Contains the **JRE, JVM, and Java Compiler (`javac`)**. Required for **developing and running** Java applications.
- **JRE (Java Runtime Environment)** → Contains the **JVM and standard Java libraries**. Required **only to run** Java applications.
- **JVM (Java Virtual Machine)** → Executes **compiled Java bytecode (`.class` files)** and makes Java **platform-independent**.

✅ **If you're a developer, install the JDK** (it includes the JRE).  
✅ **If you only need to run Java applications, install the JRE**.

---

## 🖥️ **1. Installing Java on Windows**

### ✅ **Step 1: Download the Oracle JDK**
1. Go to the **official Oracle JDK download page**:  
   👉 [Oracle JDK Downloads](https://www.oracle.com/java/technologies/javase-downloads.html)
2. Select the **latest JDK version** for **Windows** (`.exe` installer).
3. Download the installer.

### ✅ **Step 2: Install Java**
1. Run the downloaded **`.exe`** file.
2. Follow the installation wizard **(Keep default settings)**.
3. Click **Next → Install** and wait for the installation to complete.

### ✅ **Step 3: Configure Environment Variables**
1. Open **File Explorer**, right-click **This PC** → **Properties** → **Advanced system settings**.
2. Click **Environment Variables**.
3. Under **System Variables**, find **`Path`** and click **Edit**.
4. Add the JDK installation path (`C:\Program Files\Java\jdk-XX.X.X\bin`).
5. Click **OK** to save.

### ✅ **Step 4: Verify Installation**
Open **Command Prompt (`cmd`)** and run:

```sh
java -version
javac -version

---

## 🍏 2. **Installing Java on macOS**

### ✅ **Step 1: Download the Oracle JDK**
1. Visit 👉 [Oracle JDK Downloads](https://www.oracle.com/java/technologies/javase-downloads.html).
2. Select **macOS** and download the **`.dmg`** installer.

### ✅ **Step 2: Install Java**
1. Open the downloaded **`.dmg`** file.
2. Follow the installation steps.
3. Java will be installed in **`/Library/Java/JavaVirtualMachines/`**.

### ✅ **Step 3: Verify Installation**
Open **Terminal** and run:

```sh
java -version
javac -version

---

## 🐧 3. **Installing Java on Linux (Ubuntu & Debian-based Distros)**

### ✅ **Step 1: Download the Oracle JDK**
1. Go to 👉 [Oracle JDK Downloads](https://www.oracle.com/java/technologies/javase-downloads.html).
2. Download the **Linux `.tar.gz` package**.


### ✅ **Step 2: Extract and Install Java**
Open **Terminal** and run the following commands:

```sh
sudo mkdir -p /usr/lib/jvm
cd ~/Downloads
sudo tar -xvf jdk-XX.X.X_linux-x64_bin.tar.gz -C /usr/lib/jvm/

### ✅ **Step 3: Set Up Java Environment Variables**
Run the following commands to set Java as the default:

```sh
sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-XX.X.X/bin/java 1
sudo update-alternatives --install /usr/bin/javac javac /usr/lib/jvm/jdk-XX.X.X/bin/javac 1
sudo update-alternatives --config java

### ✅ **Step 4: Verify Installation**
Run the following commands to check if Java is installed correctly:

```sh
java -version
javac -version
