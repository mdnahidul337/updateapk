# UpdateAPK Repository

এই রিপোজিটরিটি অ্যাপের **update.json** এবং **APK ফাইল** হোস্ট করার জন্য ব্যবহার করা হয়।
অ্যাপ নতুন আপডেট চেক করার জন্য এখানে থাকা JSON ফাইল ব্যবহার করে।

---

# 📂 ফাইল স্ট্রাকচার

```
updateapk
│
├── BDBLA
│   └── update.json
│
└── bdbla.apk
```

* **update.json** → অ্যাপের আপডেট তথ্য
* **bdbla.apk** → নতুন APK ফাইল

---

# ⚙️ update.json Example

```json
{
  "version": "1.0.5",
  "update_required": true,
  "title": "New Update Available",
  "message": "Please update the app to continue using the latest features.",
  "whats_new": [
    "Improved app performance",
    "Faster download system",
    "Stable version with bug fixes"
  ],
  "apk_url": "https://github.com/mdnahidul337/updateapk/raw/main/bdbla.apk"
}
```

---

# 🔗 Direct Download URL Example

APK ডাউনলোড করার জন্য একটি সরাসরি লিংক ব্যবহার করতে পারেন।

Example:

```
https://drive.usercontent.google.com/download?id=1hg4Fu3QqRQgCXcTgE6Hp5XeW20-GJAPp&export=download
```

App এর কোডে উদাহরণ:

```
finalUrl = 'https://drive.usercontent.google.com/download?id=1hg4Fu3QqRQgCXcTgE6Hp5XeW20-GJAPp&export=download';
```

---

# 📤 CMD দিয়ে ফাইল আপলোড করার নিয়ম

### 1️⃣ Project Folder এ যান

CMD খুলে লিখুন:

```
cd C:\Users\Nahid\Desktop\updateapk
```

---

### 2️⃣ ফাইল পরিবর্তন হয়েছে কিনা দেখুন

```
git status
```

---

### 3️⃣ সব ফাইল Add করুন

```
git add .
```

অথবা নির্দিষ্ট ফাইল:

```
git add BDBLA/update.json
```

---

### 4️⃣ Commit করুন

```
git commit -m "update json version"
```

---

### 5️⃣ GitHub এ Push করুন

```
git push origin main
```

---

# ⚠️ Push Error Fix (If Rejected)

যদি এই ধরনের error আসে:

```
! [rejected] main -> main (fetch first)
```

তাহলে আগে pull করুন:

```
git pull origin main --allow-unrelated-histories
```

তারপর আবার push করুন:

```
git push origin main
```

---

# 🚀 সম্পূর্ণ CMD কমান্ড একসাথে

```
cd C:\Users\Nahid\Desktop\updateapk
git pull origin main
git add .
git commit -m "update version"
git push origin main
```

---

# ℹ️ নোট

* JSON আপডেট করলে অ্যাপ নতুন আপডেট চেক করতে পারবে
* APK ফাইল আপলোড করার পর `apk_url` আপডেট করতে হবে
* GitHub Raw URL ব্যবহার করা ভালো

Example:

```
https://github.com/mdnahidul337/updateapk/raw/main/bdbla.apk
```

---

# 📢 Update Message Example

নতুন আপডেট রিলিজ হলে ব্যবহারকারীদের জন্য উদাহরণ মেসেজ:

```
New Update Available!

✔ Improved app performance  
✔ Faster download system  
✔ More stable version with bug fixes  

Please update the app to enjoy the latest improvements.
```

---

# 👨‍💻 Developer

**N Studio**
Owner: **Md Nahidul Islam**
Location: Bangladesh
