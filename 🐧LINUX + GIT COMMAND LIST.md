# 🐧 LINUX + GIT COMMAND LIST (DAY 1)

---

## 🔹 1. NAVIGATION

```bash
pwd
ls
ls -l
ls -a

cd ~
cd /
cd ..
cd folder_name
```

---

## 🔹 2. FILE & DIRECTORY OPERATIONS

```bash
mkdir folder_name
mkdir -p a/b/c

touch file.txt

cp file.txt folder/
mv file.txt newname.txt
mv file.txt folder/

rm file.txt
rm -r folder/
```

---

## 🔹 3. FILE VIEW & EDIT

```bash
cat file.txt
nano file.txt
vim file.txt
```

---

## 🔹 4. PERMISSIONS

```bash
ls -l
chmod +x file.txt
chmod 777 file.txt
```

---

## 🔹 5. SYSTEM / UTILITIES

```bash
tree
clear
whoami
```

---

## 🔹 6. PACKAGE MANAGEMENT

```bash
sudo apt update
sudo apt upgrade
sudo apt install tree
```

---

## 🔹 7. GIT (BASIC)

```bash
git init
git status
git add .
git commit -m "message"

git config --global user.name "Your Name"
git config --global user.email "your@email.com"

git branch -m main
```

---

## 🔹 8. WORKSPACE SETUP

```bash
cd ~
mkdir vlsi_workspace
cd vlsi_workspace

mkdir linux digital verilog projects notes
tree
```

---

## 🔹 9. VS CODE (WSL)

```bash
code .
```

---

## 🔹 10. OPTIONAL (AUTO OPEN WORKSPACE)

```bash
echo "cd ~/vlsi_workspace" >> ~/.bashrc
source ~/.bashrc
```

---

## 🔹 11. TROUBLESHOOTING

```bash
ls ~
find / -type d -name "vlsi_workspace" 2>/dev/null
```

---

# 🔥 MOST IMPORTANT COMMANDS (REMEMBER FIRST)

```bash
cd
ls
mkdir
touch
rm
cp
mv
nano
git add
git commit
```

---

# 🎯 GOAL

✔ Navigate Linux without fear
✔ Manage files confidently
✔ Start using Git daily
✔ Build habit of terminal usage
