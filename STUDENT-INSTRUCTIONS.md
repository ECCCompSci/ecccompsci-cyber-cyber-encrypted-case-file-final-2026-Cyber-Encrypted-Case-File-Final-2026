# 📋 Student Instructions — Encrypted Case File Final

## Overview
You will work inside your **GitHub Classroom assignment** and build your own **Encrypted Case File** — both solving the provided mystery *and* creating your own encrypted evidence for a peer to solve. This project covers cryptography (Unit 4.1) and digital forensics basics (Unit 4.2).

---

## 💻 Setting Up VS Code

You will use **Visual Studio Code (VS Code)** to open, edit, and submit your work. Follow these steps to get started:

### Step 1 — Accept the Assignment
1. Click the **GitHub Classroom assignment link** provided by your teacher.
2. Click **Accept this assignment**.
3. GitHub will create a personal repo for you automatically — wait for it to finish, then click your repo link.

### Step 2 — Clone Your Repo into VS Code
1. On your GitHub repo page, click the green **Code** button.
2. Make sure **HTTPS** is selected and copy the URL.
3. Open **VS Code** on your computer.
4. Press **Ctrl + Shift + P** (Windows) or **Cmd + Shift + P** (Mac) to open the Command Palette.
5. Type **Git: Clone** and press Enter.
6. Paste your repo URL and press Enter.
7. Choose a folder to save it (e.g., `Documents/GitHub`).
8. When prompted, click **Open** to open the cloned repo in VS Code.

### Step 3 — Make Sure Git Is Set Up
If VS Code asks you to configure Git, open the built-in terminal (**Terminal → New Terminal**) and run:
```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### Step 4 — Committing and Pushing Your Work
After making changes to any file:
1. Click the **Source Control** icon on the left sidebar (looks like a branch).
2. You will see your changed files listed.
3. Hover over a file and click **+** to stage it.
4. Type a **meaningful commit message** in the box (e.g., `Add decryption notes for message 1`).
5. Click the **✓ Commit** button.
6. Click **Sync Changes** (or the cloud/arrow icon) to push to GitHub.

> ✅ Do this after every major section — your commit history is part of your grade!

---

## Part 1 — Solve the Case (Provided Materials)

### Step 1: Decrypt the Messages
- Open `crypto/message1_encrypted.txt` and `crypto/message2_encrypted.txt` in VS Code.
- Read `crypto/crypto_notes.md` to understand what cipher types were used (but NOT the key — you must figure that out!).
- Decrypt both messages by hand or with a tool. Document your method.
- Create a new file in VS Code called `crypto/my_decryption.md` and explain:
  - What cipher was used for each message
  - What steps you took to break it
  - The plaintext result

### Step 2: Analyze the Forensic Evidence
- Open and review all three files in the `/forensics/` folder in VS Code:
  - `server_log.txt` — What was accessed? By whom? When?
  - `email_header.txt` — Where did the email originate? Is anything suspicious?
  - `file_metadata.txt` — What do the timestamps tell you?
- Answer every question in `forensics/investigation_questions.md`.
- Create a new file: `forensics/my_answers.md` with your answers.

---

## Part 2 — Build Your Own Encrypted Case

Create a **second scenario** inside a new folder called `/my_case/`. In VS Code, right-click in the Explorer panel and select **New Folder** to create it. Your case must include:

### Required Files
| File | Description |
|---|---|
| `my_case/README.md` | Your scenario backstory (who, what, when, where) |
| `my_case/message_encrypted.txt` | At least ONE message you encrypted |
| `my_case/cipher_explanation.md` | What cipher you used, why it's weak or strong, and how frequency analysis applies |
| `my_case/evidence.txt` | Made-up log, email header, or metadata as your forensic clue |
| `my_case/questions.md` | 3–5 questions a peer investigator must answer |

### Cipher Requirements
- You must use **at least one** of the following: Caesar cipher, Vigenère cipher, or substitution cipher.
- Optionally include symmetric or asymmetric encryption concepts in your written explanation even if your actual message uses a classical cipher.
- Do NOT include your decryption key in the same folder — create a separate `my_case/TEACHER_KEY.md` file.

---

## Commit Requirements
You must have **at least 5 meaningful commits** with clear messages. Examples:
```
Add decryption notes for message 1
Complete forensics investigation answers
Create my_case scenario and encrypted message
Add cipher explanation for my case
Finish all investigation questions
```

Vague messages like `stuff`, `done`, or `update` will lose points.

---

## Submission
- Your work is automatically saved to your **GitHub Classroom repo** every time you push.
- Make sure all required files are present and your latest changes are pushed before the due date.
- You do **not** need to submit a link — your teacher can see your repo through GitHub Classroom.
- **Due Date:** ___________________________
