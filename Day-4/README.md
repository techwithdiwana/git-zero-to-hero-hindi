# 📘 Git Zero to Hero – Day 4  

![Made with Love](https://img.shields.io/badge/Made%20with-❤-red) ![Powered by Git](https://img.shields.io/badge/Powered%20by-Git-orange) ![Level Intermediate](https://img.shields.io/badge/Level-Intermediate-yellow) ![Brand Tech With Diwana](https://img.shields.io/badge/Brand-Tech%20With%20Diwana-orange)  

## 🔥 Topics Covered  

- ✅ Git Merge  
- ✅ Git Rebase  
- ✅ Git Stash  
- ✅ Git Cherry-pick  
- ✅ Git Branching  
- ✅ Git Workflow  
- ✅ Git Tag & Release Creation  

---

## 📌 Git Merge  

- Merge ek branch ke changes ko dusre branch me integrate karta hai.  
- Example:  
  ```bash
  git checkout main
  git merge feature-branch
  ```  
- **Advantage**: History safe rehta hai.  
- **Limitation**: Extra merge commits create ho jate hain.  

---

## 📌 Git Rebase  

- Rebase ek branch ke commits ko dusre branch ke upar re-apply karta hai.  
- Example:  
  ```bash
  git checkout feature-branch
  git rebase main
  ```  
- **Advantage**: Clean & linear history.  
- **Limitation**: History rewrite hota hai, toh shared branches pe carefully use karein.  

---

## 📌 Git Stash  

- Stash temporary changes ko save karta hai bina commit kiye.  
- Example:  
  ```bash
  git stash save "WIP: half-done feature"
  git stash list
  git stash apply
  ```  
- Useful jab aapko branch switch karni ho aur kaam adhura ho.  

---

## 📌 Git Cherry-pick  

- Cherry-pick ek specific commit ko current branch me apply karta hai.  
- Example:  
  ```bash
  git checkout main
  git cherry-pick <commit-hash>
  ```  
- Useful for **hotfixes**.  

---

## 📌 Git Branching (Recap)  

- Branch = independent line of development.  
- Example:  
  ```bash
  git checkout -b feature-payment
  ```  
- Git branching ko merge + rebase ke sath use karke ek powerful workflow banaya jata hai.  

---

## 📌 Git Workflow  

- Common workflows:  
  - **Feature Branch Workflow** – har feature ek alag branch.  
  - **Gitflow Workflow** – `main`, `develop`, `feature/*`, `release/*`, `hotfix/*`.  
  - **Forking Workflow** – open source contribution ke liye.  

---

## 📌 Git Tag & Release Creation  

- **Lightweight Tag**: sirf ek pointer.  
  ```bash
  git tag v1.0
  ```

- **Annotated Tag**: details ke sath.  
  ```bash
  git tag -a v1.0 -m "Release version 1.0"
  ```

- Push tags to remote:  
  ```bash
  git push origin v1.0
  ```

- Push all tags:  
  ```bash
  git push origin --tags
  ```

---

## 🌐 Connect with Me  

- 🎥 **YouTube**: [Tech With Diwana](https://www.youtube.com/@TechWithDiwana)  
- 💻 **GitHub**: [techwithdiwana](https://github.com/techwithdiwana)  
- 🔗 **LinkedIn**: [Tech With Diwana](https://www.linkedin.com/in/techwithdiwana)  

---

✍️ **Prepared By:** *Tech With Diwana*  
