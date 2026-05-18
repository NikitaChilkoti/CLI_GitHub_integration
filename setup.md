## Hands-on setup (Step-by-step)

You'll get the feeling when you would have successfully connected CLI to GitHub. Trust me, though very easy, it gives feelig of authority and a sense of knowledge.
---
### 1. Check git version
Before anything, make sure Git exists on your system.

`git --version`

If not, then install git
`sudo apt install git`

---
### 2. Tell CLI who you are
`git config --global user.name "Your Name"`

`git config --global user.email "your-email@example.com"`

---
### 3. Generate SSH Key
Create a secure key to authenticate with GitHub.

`ssh-keygen -t ed25519 -C "your-email@example.com"`

Print the generated Public key
`cat ~/.ssh/id_ed25519.pub`

Copy this.

---
### 4. Add this key to GitHub
Go to GitHub --> Settings --> SSH and GPG Keys --> New SSH Key

Paste the key here, and Save.

---
### 5. Test your connection
This will check and show whether you've authenticated rightly or not.

`ssh -T git@github.com`

---

## ⭐ You'll see a successful authentication message.

## Remember
You can connect to your GitHub but cannot be inside it.

## Refer [the next file](Initialising_&_Pushing_a_repo.ssh) to initialize a local repository and to push it to GitHub.
