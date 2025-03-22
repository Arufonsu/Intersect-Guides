# 🔐 Git Commit Signing with GPG

## 📥 Prerequisites
You will need the following programs installed:

- [Git for Windows](https://gitforwindows.org/)
- [GPG4Win](https://gpg4win.org/thanks-for-download.html)

![imagen](https://github.com/user-attachments/assets/57f887d8-1b1f-44e3-a68d-788dc75df0ca)

## 🖥️ Setup GPG

### 1️⃣ Check GPG Configuration
Open Git Bash and run:

```sh
gpgconf
```

![imagen](https://github.com/user-attachments/assets/ca87915a-78fa-43b5-8de5-6145cdce00d4)

### 2️⃣ Ensure GUI Prompt for Pinentry
Run the following command to check if `pinentry` shows a GUI prompt:

```sh
echo GETPIN | pinentry
```

![imagen](https://github.com/user-attachments/assets/51227a45-3c82-4f75-8dba-24ba237a09bc)

---

## 🛠️ Configure Git to Use GPG

Run:

```sh
git config --global gpg.program "C:\Program Files (x86)\GnuPG\bin\gpg.exe"
```

Then, generate a new GPG key:

```sh
gpg --full-generate-key
```

![{C8DD9027-1A50-43BE-A070-9F6FB0CD2CEE}](https://github.com/user-attachments/assets/e574dd0f-1877-4562-8830-5854d14311e8)

### 🔢 Select Key Type

Type `4`, then press **Enter**:

![{D732D00F-D7CD-46A8-AD83-F06A807F75DA}](https://github.com/user-attachments/assets/e0c8bc8e-d65f-4fa7-9931-73bcbf813a9c)

Type `4096`, then press **Enter**:

![{55EC6264-78C1-4790-8A9B-02A44C4B05FA}](https://github.com/user-attachments/assets/8b92949a-243a-4041-a77f-4b494cfad0b9)

Type `0` (for a key that never expires), then press **Enter**:

![{01AEB613-1C02-4506-A76D-2DE89276E82F}](https://github.com/user-attachments/assets/27f4a1d9-1dbb-4833-82db-d130aed478ae)

Enter your **GitHub username** and **email**:

![{6E0395BF-AB0B-4377-89E7-06E3A323DD68}](https://github.com/user-attachments/assets/3f7d112a-2f20-4e8f-b9c9-0dd04b914298)

Set a **passphrase**, then confirm it:

![{8BE1C3DE-B009-4BCA-BC71-F32390BB8D76}](https://github.com/user-attachments/assets/af39f62f-807e-46c0-885f-5bbdbdb7362e)

✅ **GPG key generated successfully!**

![{30092BC8-0533-433F-A190-F3CF062D9A62}](https://github.com/user-attachments/assets/80ba10f8-aadc-4398-a27c-5306e7ac5c65)

---

## 🔍 Verify Your GPG Key

Run:

```sh
gpg --list-secret-keys --keyid-format=long
```

You should see your GPG key:

![{289684BF-3817-49FE-ABE4-C09C75E3816B}](https://github.com/user-attachments/assets/a2d044e1-892b-42a3-93df-e8da0e4ab617)

Export your GPG key:

```sh
gpg --armor --export B0EEC08E5A242F28
```

![{71C04B71-FC0D-4D99-9EBB-D3BE59718799}](https://github.com/user-attachments/assets/ef606433-a1e5-4be3-8963-473aa79da09c)

Copy your GPG key (from `-----BEGIN PGP PUBLIC KEY BLOCK-----` to `-----END PGP PUBLIC KEY BLOCK-----`) and add it to [your GitHub account](https://github.com/settings/keys).

---

## 🏗️ Configure GPG in JetBrains Rider

Go to **Settings** ➝ **Version Control** ➝ **Git** ➝ **Configure GPG**.

![{59026275-D1E1-45AC-B70B-C0B1F09B9E82}](https://github.com/user-attachments/assets/00f3aa5f-e97c-4c36-ae9d-cf5046cf6284)

Enable **"Sign commits with GPG key"**, select your key, then click **OK** and **Save**:

![{A7DE1CA5-5D6A-4C60-A129-F79EE1985902}](https://github.com/user-attachments/assets/a9d25be4-b2c5-4bc2-9460-da8262291bc5)

---

## 🎉 Commit with GPG Signing

Now, every time you commit, you will be prompted to enter your passphrase!

![{91823011-CA44-492E-A1C5-92F6CD9FB532}](https://github.com/user-attachments/assets/53a43dee-9d27-4d14-9ec6-44aebd0e5887)

🚀 **You're all set! Your commits are now signed with GPG!** 🔐
