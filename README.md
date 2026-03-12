# UpdateAPK Repository

এই রিপোজিটরিটি অ্যাপের **update.json** এবং **APK ফাইল** হোস্ট করার জন্য ব্যবহার করা হয়।
অ্যাপ নতুন আপডেট চেক করার জন্য এখানে থাকা **JSON ফাইল** ব্যবহার করে।

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

# 🚀 সম্পূর্ণ CMD কমান্ড একসাথে

```
cd C:\Users\Nahid\Desktop\updateapk
git add .
git commit -m "update version"
git push origin main
```

---

# ⚠️ যদি Push Error দেখায়

যদি নিচের এরর আসে:

```
Updates were rejected because the remote contains work that you do not have locally
```

তাহলে আগে Pull করুন:

```
git pull origin main --allow-unrelated-histories
```

তারপর আবার Push করুন:

```
git push origin main
```

---

# 🔗 Google Drive Download URL (ID System)

যদি Google Drive থেকে APK ডাউনলোড করতে চান, তাহলে শুধু **File ID** ব্যবহার করুন।

Example:

```
finalUrl = 'https://drive.google.com/uc?export=download&id=$id';
```

এখানে `$id` হবে Google Drive ফাইলের ID।

Example Drive Link:

```
https://drive.google.com/file/d/1ABC123XYZ/view
```

File ID:

```
1ABC123XYZ
```

Final Download URL:

```
https://drive.google.com/uc?export=download&id=1ABC123XYZ
```

---

# ℹ️ নোট

* JSON আপডেট করলে অ্যাপ নতুন আপডেট চেক করতে পারবে
* APK ফাইল আপলোড করার পর `apk_url` আপডেট করতে হবে
* GitHub **Raw URL** ব্যবহার করা ভালো
* Google Drive ব্যবহার করলে **Direct Download URL** ব্যবহার করুন

---

# 👨‍💻 Developer

**N Studio**
Owner: **Md Nahidul Islam**
Location: Bangladesh
