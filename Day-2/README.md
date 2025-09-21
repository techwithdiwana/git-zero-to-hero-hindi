# 📘 Git Zero to Hero – Day 2  

![Made with Love](https://img.shields.io/badge/Made%20with-❤-red) ![Powered by Git](https://img.shields.io/badge/Powered%20by-Git-orange) ![Level Beginner](https://img.shields.io/badge/Level-Beginner-brightgreen) ![Brand Tech With Diwana](https://img.shields.io/badge/Brand-Tech%20With%20Diwana-orange)  

## 🔥 Topics Covered  

- What is Git?  
- Difference between Git and GitHub  
- Git Architecture  
- Git clone, commit, push  
- Hands-on Git commands for beginners  

---

## 📌 What is Git?  

- Git ek **Distributed Version Control System (DVCS)** hai jo developers ko code ka **history track karne**, **collaborate karne** aur **parallel changes manage karne** ka option deta hai.  
- Har developer ke paas apna **local repository + full history** hoti hai.  
- **Key Benefits**: Fast, secure, offline work possible, aur branching/merging bahut powerful hai.  

---

## 📌 Difference between Git and GitHub  

| Feature            | Git 🚀 | GitHub 🌐 |
|--------------------|--------|-----------|
| **Definition**     | Local DVCS tool | Cloud-based hosting service |
| **Where it works** | Local system (offline bhi) | Online, internet required |
| **Usage**          | Code track, branch, merge | Remote repo host, collaboration |
| **Scope**          | Tool/software | Platform/service |
| **Example**        | `git commit`, `git push` | Pull Request, Issues, Actions |

👉 Simple words me: **Git = Tool, GitHub = Hosting Service**.  

---

## 📌 Git Architecture  

Git ke andar 3 main areas hote hain:  

1. **Working Directory**  
   - Ye aapke project files ka area hai.  
   - Yahan aap code edit karte ho.  

2. **Staging Area (Index)**  
   - Ye ek temporary storage hai jahan aap decide karte ho ki kaunse changes commit karne hain.  
   - Command:  
     ```bash
     git add file.txt
     ```

3. **Repository (.git directory)**  
   - Yahan par commits permanently store hote hain.  
   - Command:  
     ```bash
     git commit -m "message"
     ```

4. **Remote Repository (GitHub, GitLab, etc.)**  
   - Ye ek centralized location hai jahan multiple developers collaborate karte hain.  
   - Command:  
     ```bash
     git push origin main
     ```

⚡ **Workflow**:  
Working Directory → `git add` → Staging Area → `git commit` → Local Repo → `git push` → Remote Repo  

---

## 📌 Git Basic Workflow (Clone → Commit → Push)  

1. **Clone** (repo ko local system me copy karna):  
   ```bash
   git clone https://github.com/username/repo.git
   ```

2. **Commit** (local changes save karna):  
   ```bash
   git add .
   git commit -m "Your commit message"
   ```

3. **Push** (local commits ko remote repo pe bhejna):  
   ```bash
   git push origin main
   ```

---

## 📌 Hands-on Git Commands for Beginners  

- Check Git version:  
  ```bash
  git --version
  ```

- Initialize repo:  
  ```bash
  git init
  ```

- Check repo status:  
  ```bash
  git status
  ```

- View commit history:  
  ```bash
  git log --oneline
  ```

- Create new branch:  
  ```bash
  git checkout -b feature-branch
  ```

---

## 🌐 Connect with Me  

- 🎥 **YouTube**: [Tech With Diwana](https://www.youtube.com/@TechWithDiwana)  
- 💻 **GitHub**: [techwithdiwana](https://github.com/techwithdiwana)  
- 🔗 **LinkedIn**: [Tech With Diwana](https://www.linkedin.com/in/techwithdiwana)  

---

✍️ **Prepared By:** *Tech With Diwana*  
