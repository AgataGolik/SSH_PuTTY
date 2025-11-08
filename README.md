# 🔹 How to Create an SSH Key with PuTTY and Connect to Vast.ai

## 🔸 Step 1: Generate SSH Keys with PuTTYgen

1. Open **PuTTYgen** (it comes bundled with PuTTY).  
2. Under **Type of key to generate**, choose **RSA** (the most common and secure option).  
3. Click **Generate** and move your mouse around the blank area until the progress bar completes.  
4. Once the key is generated:
   - You’ll see your **public key** in the field labeled **Public key for pasting into OpenSSH authorized_keys file** – copy this, you’ll need it for Vast.ai.
   - Set a **key passphrase** if you want extra security and **confirm key passphrase** .
     (When generating your key in PuTTYgen, you can set a key passphrase - a password that protects your private key file. Each time you start your computer and open the key file (for example, by double-clicking the CodeAssist.ppk (if you name the file like this) icon on your desktop, PuTTY will ask you to enter this passphrase)
5. Then click:
   - **Save private key** → save it as something like `CodeAssist` – this is the file you’ll use in PuTTY.  
   - (You can also click **Save public key**, but copying the text from the box is usually enough.)

---

## 🔸 Step 2: Upload the Public Key to Vast.ai

1. Log in to [https://vast.ai/console](https://vast.ai/console).  
2. Go to **Account → SSH Keys**.  
3. Click **Add SSH Key**.  
4. Paste your **public key** from PuTTYgen – it should look something like this:

   `ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQ... user@vast-ai-key`
