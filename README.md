1️⃣ Go to Your Project Folder

Open Command Prompt and move to the repo folder.

cd path\to\your\updateapk

Example:

cd C:\Users\Nahid\Desktop\updateapk
2️⃣ Check Repo Status
git status

This shows which files changed (like update.json).

3️⃣ Add Files to Commit

Add all changed files:

git add .

Or only add the JSON file:

git add BDBLA/update.json
4️⃣ Commit Changes
git commit -m "update version 1.0.5 json"
5️⃣ Push to GitHub
git push origin main

If your branch is master, use:

git push origin master

✅ Complete CMD Flow

cd C:\Users\Nahid\Desktop\updateapk
git status
git add .
git commit -m "update json version"
git push origin main
⚠️ If Repo Not Connected Yet

Run once:

git remote add origin https://github.com/mdnahidul337/updateapk.git
git branch -M main
git push -u origin main
