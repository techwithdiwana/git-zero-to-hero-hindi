# 📘 Git Zero to Hero – Day 5  

![Made with Love](https://img.shields.io/badge/Made%20with-❤-red) ![Powered by Git](https://img.shields.io/badge/Powered%20by-Git-orange) ![Level Advanced](https://img.shields.io/badge/Level-Advanced-blue) ![Brand Tech With Diwana](https://img.shields.io/badge/Brand-Tech%20With%20Diwana-orange)  

## 🔥 Topics Covered  

- Git Parse क्या है और इसका इस्तेमाल कब करना चाहिए  
- Git Reflog से Git history को कैसे recover करें  
- Git Squash का इस्तेमाल करके commits को combine कैसे करें  
- Step-by-step hands-on demo  
- Real-life use cases & pro tips  

---

## 📌 Git Parse क्या है और इसका इस्तेमाल कब करना चाहिए  

- `git rev-parse` (Git Parse) ek **plumbing command** hai jo commit IDs, branch names, aur references ko parse karta hai.  
- Example:  
  ```bash
  git rev-parse HEAD
  ```  
  Ye current commit ka hash dikhata hai.  

- Use cases:  
  - Scripts me automation ke liye  
  - Branch ya commit ka exact reference nikalne ke liye  
  - Low-level Git debugging  

---

## 📌 Git Reflog se Git history recover karna  

- Reflog ek tarah ka **safety net** hai jo batata hai ki `HEAD` aur branches pehle kaha point kar rahe the.  
- Example:  
  ```bash
  git reflog
  ```  

- Agar galti se branch delete ho jaye ya commit reset ho jaye, toh aap Reflog se commit hash nikal kar recover kar sakte ho:  
  ```bash
  git checkout -b recovery-branch <commit-hash>
  ```  

---

## 📌 Git Squash – Multiple commits ko combine karna  

- Squash ek tarika hai multiple commits ko **ek single commit** me combine karne ka.  
- Useful jab aapke paas chhote-chhote commits ho aur aap clean history banana chahte ho.  

Example:  

```bash
git rebase -i HEAD~3
```

- Editor open hoga, aap `pick` ko `squash` me change karo:  

```
pick 1234 Add login button
squash 5678 Fix button color
squash 9abc Finalize login UI
```

- Result: ek single commit banega.  

---

## 📌 Step-by-step Hands-on Demo  

1. Create test commits:  
   ```bash
   git checkout -b feature-demo
   echo "line1" >> demo.txt
   git add demo.txt
   git commit -m "Commit 1"

   echo "line2" >> demo.txt
   git commit -am "Commit 2"

   echo "line3" >> demo.txt
   git commit -am "Commit 3"
   ```

2. Squash last 3 commits:  
   ```bash
   git rebase -i HEAD~3
   ```

3. Recover accidentally deleted commit via reflog:  
   ```bash
   git reflog
   git checkout -b recovery <commit-hash>
   ```

---

## 📌 Real-life Use Cases & Pro Tips  

- **Git Parse**: Automation scripts aur CI/CD pipelines me use hota hai.  
- **Git Reflog**: Jab bhi commit/branch delete ho jaye, aapko “time travel” karne ka option deta hai.  
- **Git Squash**: Clean history maintain karne ke liye use karo — open-source projects me highly recommended.  

---

## 🌐 Connect with Me  

- 🎥 **YouTube**: [Tech With Diwana](https://www.youtube.com/@TechWithDiwana)  
- 💻 **GitHub**: [techwithdiwana](https://github.com/techwithdiwana)  
- 🔗 **LinkedIn**: [Tech With Diwana](https://www.linkedin.com/in/techwithdiwana)  

---

✍️ **Prepared By:** *Tech With Diwana*  
