
# 🚀 Intersect Engine Setup Guide: Using Rider IDE, Git, and Dev to Compile 🎮

Welcome to the **Intersect Engine Setup Guide**! This guide is designed to walk you through the steps of setting up **Rider IDE**, **Git**, and **.NET SDK** to start developing with **Intersect Engine**. By following these steps, you’ll be ready to code, compile, and bring your game vision to life! 🌟

This guide assumes you're working on **Windows 11**. Let's get started! 🛠️

---

### 📥 **Required Software**

Before we begin, ensure you have the following tools installed:

- **[Download .NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)** 💻
- **[Download Git](https://github.com/git-for-windows/git/releases/download/v2.48.1.windows.1/Git-2.48.1-64-bit.exe)** 🔗
- **[Download Rider (IDE)](https://www.jetbrains.com/rider/download/download-thanks.html?platform=windows)** 🧑‍💻
- **GitHub Account** 🧑‍💼
- **Rider Account** (you can link your GitHub account to Rider for easier setup) 🔗

### 🔧 **Suggested Tools**

These tools can make your workflow smoother:
- **Notepad++** 📝
- **Aseprite** (for sprite creation) 🎨

---

### 💾 **Step 1: Install Required Programs**

Start by downloading and installing the required software:

1. **.NET 8 SDK**: Install this first to get the necessary frameworks.
2. **Git**: Download and install Git to enable version control.
3. **Rider IDE**: This is your development environment where all the magic happens. 

Here’s what each installation should look like:

**1. Install .NET SDK**
   
   ![Install .NET SDK](https://github.com/user-attachments/assets/ff81965a-f1f2-43b8-997d-8f63e17325b8)

**2. Install Git** 

   ![Install Git](https://github.com/user-attachments/assets/0c752354-eb60-4607-ba00-fe6627e227bd)

After you have installed everything, open **Rider IDE**.

---

### 🖥️ **Step 2: Launch Rider**

Once you open **Rider**, you should see the following screen:

![Rider Welcome Screen](https://github.com/user-attachments/assets/ffb7734c-b980-44ef-a928-badedc70cff9)

1. **Pick the Free Non-Commercial License**:
   
   Select the **Free Non-Commercial Use** option to proceed. 

![Non-Commercial License](https://github.com/user-attachments/assets/8c4e79c8-862f-4151-8ee4-a4008380b82e)

Then press the following (WIP...):

<img width="187" alt="{F6CC5EE0-CF58-4739-8FFC-B348C9441CEB}" src="https://github.com/user-attachments/assets/8c4e79c8-862f-4151-8ee4-a4008380b82e" />

<img width="334" alt="{060E6AAB-4C79-4C29-B35A-D42F966CB36C}" src="https://github.com/user-attachments/assets/e813c8d1-a773-4f70-a855-47669804258b" />

<img width="429" alt="{B71072F3-E078-4807-89EE-B53B67114BF5}" src="https://github.com/user-attachments/assets/a093d113-7a8e-4da8-97e4-bae9042a54a0" />

<img width="374" alt="{2510EBCF-2F03-43DC-8A16-B42060394946}" src="https://github.com/user-attachments/assets/a3814025-5c26-459f-9dc4-a8184433d783" />

Accept the TOS
<img width="457" alt="{D01CF7FE-E68F-4514-BBBC-444172908D49}" src="https://github.com/user-attachments/assets/971a4e3f-c745-4d53-9c9a-d6cf8c7b2f82" />

<img width="525" alt="{31399A39-D50E-4DF2-B5C2-749A44BADF79}" src="https://github.com/user-attachments/assets/38e08ab9-4ca8-4347-9b30-792a26898a65" />

2. **Accept the Terms of Service (TOS)**:

   Don't forget to accept the Rider **TOS** to continue using the IDE legally! 📜

   ![TOS Acceptance](https://github.com/user-attachments/assets/971a4e3f-c745-4d53-9c9a-d6cf8c7b2f82)

---

### 🔑 **Step 3: Rider Configuration**

Now that you’ve got Rider installed, it's time to configure your settings.

1. **Set Keybinds**:
   
   Customize your keybinds based on your preference for a smooth workflow.

   ![Keybindings Setup](https://github.com/user-attachments/assets/c725e427-2f9b-4f53-97fe-c971746a05c3)

2. **Plugins**:
   
   While there are a ton of useful plugins, **I don't recommend installing any plugins** at this stage. It's best to start with the essentials and only add more if you find you need them later on. 🔌

---

### 🌐 **Step 4: Clone the Intersect Engine Repository**

Now that Rider is set up, let's get the **Intersect Engine** project from **GitHub**.

1. **Clone the repository**:
   
   Open Rider and choose the **Clone Repository** button to clone the Intersect Engine repository. This is where you'll get all the project files to start working on.

	 ![CloneRepo](https://github.com/user-attachments/assets/7d9dafab-3a25-46f0-8703-47a91b2e994f)

2. **Choose repository URL** -> [https://github.com/AscensionGameDev/Intersect-Engine](https://github.com/AscensionGameDev/Intersect-Engine)

   ![CloneRepoURL](https://github.com/user-attachments/assets/6fd10a0f-90f4-49f8-a717-584d707ce70f)

3. **Click Clone**, the repo should start cloning locally on your device:

   ![Repo Cloning](https://github.com/user-attachments/assets/616c6fef-6f7b-4eb7-b77a-8e78ecedb256)

4. **Click "Open as Directory"**:

   ![Open as Directory](https://github.com/user-attachments/assets/d3696166-8f90-4a35-961c-219653c390f1)

5. **Trust and Open the Repository**:

   ![Trust and Open](https://github.com/user-attachments/assets/7205effb-44d4-4462-b42e-df3f8c43ad2f)

6. **Check your notifications**, exclude the project files from Windows Defender:

   ![Windows Defender Exclusion](https://github.com/user-attachments/assets/5f61d945-820e-405e-bd7d-1fd963f5ac20)

7. **Congratulations**, you have successfully opened the repo:

   ![Repo Successfully Opened](https://github.com/user-attachments/assets/2d66a630-d63a-45a2-83bc-158a19ec3970)

---

### 🛠️ **Step 5: Build and Compile**

Once you have the Intersect Engine repository cloned into your local environment, it’s time to compile the project.

1. Open Rider and go to **File > Open** to open your cloned repository.
2. (wip.. explain here how to build using rider's terminal and dotnet build commands....)

Good luck, and happy developing! 🙌
