
# 🚀 Intersect Engine Setup Guide: Using Rider IDE, Git, and .NET SDK to Compile your own build 🎮

Welcome to the **Intersect Engine Setup Guide**! This guide will walk you through the steps to set up **Rider IDE**, **Git**, and **.NET SDK** for developing with **Intersect Engine**. By following these instructions, you'll be able to code, compile, and bring your game vision to life! 🌟

This guide assumes you're working with **Windows 11**. Let’s dive in! 🛠️

---

### 📥 **Required Software**

Before we begin, make sure you have the following tools:

- **[Download .NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)** 💻
- **[Download Git](https://github.com/git-for-windows/git/releases/download/v2.48.1.windows.1/Git-2.48.1-64-bit.exe)** 🔗
- **[Download Rider (IDE)](https://www.jetbrains.com/rider/download/download-thanks.html?platform=windows)** 🧑‍💻
- **GitHub Account** 🧑‍💼
- **Rider Account** (You can link your GitHub account to Rider for easier setup) 🔗

![Install .NET SDK](https://github.com/user-attachments/assets/ff81965a-f1f2-43b8-997d-8f63e17325b8)

---

### 💾 **Step 1: Install Required Programs**

Start by downloading and installing the necessary software:

1. **.NET 8 SDK**: Install this first to ensure you have the required frameworks.
2. **Git**: Download and install Git to enable version control.
3. **Rider IDE**: This is your development environment where all the magic happens.

Once everything is installed, open **Rider IDE**.

![Install Git](https://github.com/user-attachments/assets/0c752354-eb60-4607-ba00-fe6627e227bd)

---

### 🖥️ **Step 2: Launch Rider**

After opening **Rider**, you should see the following screen:

![Rider Welcome Screen](https://github.com/user-attachments/assets/ffb7734c-b980-44ef-a928-badedc70cff9)

1. **Pick the Free Non-Commercial License** and log in:

   ![Non-Commercial License](https://github.com/user-attachments/assets/8c4e79c8-862f-4151-8ee4-a4008380b82e)

2. **Log in with your GitHub Account**:

   ![Github Login](https://github.com/user-attachments/assets/e813c8d1-a773-4f70-a855-47669804258b)

3. **Authorize Rider to Use Your GitHub Account**:

   ![Auth Rider](https://github.com/user-attachments/assets/a093d113-7a8e-4da8-97e4-bae9042a54a0)

   ![Auth Rider 2](https://github.com/user-attachments/assets/a3814025-5c26-459f-9dc4-a8184433d783)

4. **Accept the Terms of Service (TOS)**:

   Don’t forget to accept the **Rider TOS** to continue using the IDE legally! 📜

   ![TOS Acceptance](https://github.com/user-attachments/assets/971a4e3f-c745-4d53-9c9a-d6cf8c7b2f82)

---

### 🔑 **Step 3: Configure Rider**

Now that Rider is installed, let’s configure it for optimal use.

1. **Choose a Theme and Keybind Preset**:

   ![Theme and Keybinds](https://github.com/user-attachments/assets/38e08ab9-4ca8-4347-9b30-792a26898a65)

2. **Plugins**:

   While Rider offers many useful plugins, **I recommend not installing any plugins** for now. It’s better to start with the essentials and add more later if necessary. 🔌

   ![Keybindings Setup](https://github.com/user-attachments/assets/c725e427-2f9b-4f53-97fe-c971746a05c3)

---

### 🌐 **Step 4: Clone the Intersect Engine Repository**

Now that Rider is configured, let's clone the **Intersect Engine** project from **GitHub**.

1. **Clone the Repository**:
   
   Open Rider and click on the **Clone Repository** button to clone the Intersect Engine repository. This will download all the project files to your local machine.

   ![Clone Repo](https://github.com/user-attachments/assets/7d9dafab-3a25-46f0-8703-47a91b2e994f)

2. **Choose Repository URL** -> [https://github.com/AscensionGameDev/Intersect-Engine](https://github.com/AscensionGameDev/Intersect-Engine)

   ![Clone Repo URL](https://github.com/user-attachments/assets/6fd10a0f-90f4-49f8-a717-584d707ce70f)

3. **Click 'Clone'**: The repository should start cloning locally on your device:

   ![Repo Cloning](https://github.com/user-attachments/assets/616c6fef-6f7b-4eb7-b77a-8e78ecedb256)

4. **Click 'Open as Directory'**:

   ![Open as Directory](https://github.com/user-attachments/assets/d3696166-8f90-4a35-961c-219653c390f1)

5. **Trust and Open the Repository**:

   ![Trust and Open](https://github.com/user-attachments/assets/7205effb-44d4-4462-b42e-df3f8c43ad2f)

6. **Exclude the Project Files from Windows Defender**:

   Check your notifications and exclude the project files from Windows Defender:

   ![Windows Defender Exclusion](https://github.com/user-attachments/assets/5f61d945-820e-405e-bd7d-1fd963f5ac20)

7. **Congratulations!** You’ve successfully opened the repository:

   ![Repo Successfully Opened](https://github.com/user-attachments/assets/2d66a630-d63a-45a2-83bc-158a19ec3970)

---


### 🛠️ **Step 5: Build and Compile**

Once you have cloned the Intersect Engine repository into your local environment, it’s time to compile the project.

1. Open Rider's terminal:
![RiderTerminal](https://github.com/user-attachments/assets/c5cc8929-0e21-41f8-ba7e-6e1437437ac8)

2. Run the following command: `git submodule update --init --recursive`
![enter image description here](https://github.com/user-attachments/assets/ccb13043-bf7d-4613-9959-8c50dd5ee421)

3. Compile a Debug build: `dotnet build -p:Configuration=Debug -p:PackageVersion=0.8.0-beta -p:Version=0.8.0`
   * All debug builds will _not_ create single-file binary outputs.

4. Compile a Release build: `dotnet build -p:Configuration=Release -p:PackageVersion=0.8.0-beta -p:Version=0.8.0`
   * Release builds will create single-file binary outputs, but to get a clean output, use `dotnet publish`.

5. Compile a Publish build (Windows x64): `dotnet publish -p:Configuration=Release -p:PackageVersion=0.8.0-beta -p:Version=0.8.0 -r win-x64`
![CompilePublish](https://github.com/user-attachments/assets/99cc4010-5715-4e29-84a6-c642ccfb8536)
   Wait for projects to restore:
![ProjectsRestore](https://github.com/user-attachments/assets/c6350ebf-efe9-416e-a0ce-a8dcf77a0669)

   Wait until `dotnet` finishes building the engine. If you reach this point without failure errors (usually displayed in red text), it means you have successfully built the Intersect Engine!
![CompileDone](https://github.com/user-attachments/assets/f54b03d3-6f12-47f3-87ae-4f1ba320a341)

---

### 🛠️ **Step 6: Build is Complete! Time to Add Assets**

1. Download the latest assets from:
   https://github.com/AscensionGameDev/Intersect-Assets/tree/main_full
![DownloadAssets](https://github.com/user-attachments/assets/161bd9c0-3c63-4690-bacc-9c7224288ecc)  
   Extract your assets to a location that's easy to manage, such as your desktop.

2. In Rider, navigate to your client's publish build, right-click the Client project folder, and select "Open In" -> "Explorer":
![RiderExplorer](https://github.com/user-attachments/assets/8f11ca7a-30d9-4664-9c62-70300e53624d)  
   Then, go to the following path:
   `C:\Users\Windows\RiderProjects\Intersect-Engine\Intersect.Client\bin\Release\net8.0\win-x64\publish`

3. Within the mentioned path, you should find your compiled client:
![PublishFolder](https://github.com/user-attachments/assets/e5987c07-3507-427f-a922-27efd04cb08c)

4. Move the `resources` folder from the previously downloaded assets:
![pasteAssets](https://github.com/user-attachments/assets/8e6e2bb9-951d-4855-8679-fa99e17ecd20)

5. Open the client, but you may get stuck on the updater:
![UpdateStuck](https://github.com/user-attachments/assets/d68196f0-7fd2-40b7-b5bf-d5aa219f0004)

7. If you are stuck on the updater, close the client. Then, go to `resources -> config.json` and delete the following from "UpdateUrl":
![enter image description here](https://github.com/user-attachments/assets/c83541f9-8d0e-4a09-a093-3fa260c2fd67)  
   Leave it like this, then save the file:
![enter image description here](https://github.com/user-attachments/assets/96f1fba0-a4c3-4b12-92d6-49356ea6cdc2)

8. Reopen the game client. Congratulations! You have successfully built your own version!
![enter image description here](https://github.com/user-attachments/assets/9efb5e21-8714-4b43-b6d6-a7c3b6fa3a38)

Good luck, and happy developing! 🙌


