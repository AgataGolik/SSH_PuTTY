# 🔹 How to Create an SSH Key with PuTTY and Connect to Vast.ai

## 🔸 Step 1: Generate SSH Keys with PuTTYgen

1. Open **PuTTYgen** (it comes bundled with PuTTY).  
2. Under **Type of key to generate**, choose **RSA** (the most common and secure option).  
3. Click **Generate** and move your mouse around the blank area until the progress bar completes.  
4. Once the key is generated:
   - You’ll see your **public key** in the field labeled **Public key for pasting into OpenSSH authorized_keys file** ->`⚠️ **Copy this – you’ll need it for Vast.ai.**`

   - Set a **key passphrase** if you want extra security and **confirm key passphrase** .
    (When you create your key in PuTTYgen, you can set a passphrase – it’s basically a password that keeps your private key safe.
Each time you restart your computer and open the key file (for example, by double-clicking the CodeAssist.ppk icon on your desktop), PuTTY will ask you to type this passphrase.
You should always enter it before using the key to connect).

![image](https://github.com/AgataGolik/images/blob/main/Projekt%20bez%20nazwy%20(33).png)
![image](https://github.com/AgataGolik/images/blob/main/Zrzut%20ekranu%202025-11-08%20163858.jpg)

6. Then click:
   - **Save private key** → save it as something like `CodeAssist` – this is the file you’ll use in PuTTY.  
   - (You can also click **Save public key**, but copying the text from the box is usually enough.)

---

## 🔸 Step 2: Upload the Public Key to Vast.ai

1. Log in to [https://vast.ai/console](https://vast.ai/console).  
2. Go to **🔑Keys**.  
3. Click `SSH Key` and `+New`
4. Paste your **public key** from PuTTYgen – it should look something like this:

   `ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQ...`

## 🔸 Step 3: CREATE VPS on Vast.ai
