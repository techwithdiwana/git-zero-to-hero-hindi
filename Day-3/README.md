# 📘 Git Zero to Hero – Day 3  

![Made with Love](https://img.shields.io/badge/Made%20with-❤-red) ![Powered by Git](https://img.shields.io/badge/Powered%20by-Git-orange) ![Level Beginner](https://img.shields.io/badge/Level-Beginner-brightgreen) ![Brand Tech With Diwana](https://img.shields.io/badge/Brand-Tech%20With%20Diwana-orange)  

## 🔥 Topics Covered  

- Git Branch Kya Hota Hai?  
- Branch Create Karna (`git branch`)  
- Switch Branch (`git checkout`)  
- Branch Rename  
- Merge Branch  
- Real Project Hands-On  
- Tips & Best Practices  

---

## 📌 Git Branch Kya Hota Hai?  

- Git me **branch ek pointer hota hai ek commit ke upar**.  
- Default branch ka naam hota hai `main` (pehle `master`).  
- Branch ka main purpose hai **parallel development without disturbing main code**.  
- Example: ek branch **feature-login**, doosra branch **bugfix-101**.  

---

## 📌 Branch Create Karna  

```bash
git branch feature-login
```

👉 Ye ek nayi branch banata hai jiska naam `feature-login` hoga.  

---

## 📌 Switch Branch  

```bash
git checkout feature-login
```

👉 Ab aapka HEAD `feature-login` branch par chala jayega.  
👉 Naya Git (2.23+) me shortcut:  

```bash
git switch feature-login
```

---

## 📌 Branch Rename  

```bash
# Old Git versions
git branch -m old-branch-name new-branch-name

# Example
git branch -m feature-login feature-auth
```

👉 Current branch ka naam change ho jayega.  

---

## 📌 Merge Branch  

```bash
# Pehle main branch me jao
git checkout main

# Fir feature branch ko merge karo
git merge feature-login
```

👉 Ab `feature-login` ka code `main` branch me merge ho gaya.  

---

## 📌 Real Project Hands-On Flow  

1. Repo clone karo:  
   ```bash
   git clone https://github.com/username/repo.git
   cd repo
   ```

2. Nayi feature branch banao aur usme switch karo:  
   ```bash
   git checkout -b feature-login
   ```

3. Code update karo aur commit banao:  
   ```bash
   git add .
   git commit -m "🚀 Added login feature"
   ```

4. Wapas `main` branch me aao aur merge karo:  
   ```bash
   git checkout main
   git merge feature-login
   ```

5. Remote pe push karo:  
   ```bash
   git push origin main
   ```

---

## 📌 Tips & Best Practices  

- Always meaningful branch names use karo (e.g., `feature-login`, `bugfix-db-connection`).  
- Ek branch = ek feature/fix (avoid mixing multiple changes).  
- Merge karne se pehle hamesha `git pull origin main` run karo taaki conflicts kam ho.  
- Large projects me **Pull Requests (PR)** prefer karo direct merge ki jagah.  

---

## 🌐 Connect with Me  

- 🎥 **YouTube**: [Tech With Diwana](https://www.youtube.com/@TechWithDiwana)  
- 💻 **GitHub**: [techwithdiwana](https://github.com/techwithdiwana)  
- 🔗 **LinkedIn**: [Tech With Diwana](https://www.linkedin.com/in/techwithdiwana)  

---

✍️ **Prepared By:** *Tech With Diwana*  
