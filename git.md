#=================================================
#Basic Git Commands (to upload a folder to GitHub)
#=================================================

# 1️⃣ Initialize Git in your current folder
git init

# 2️⃣ (Optional) Check the status of your files
git status

# 3️⃣ Add all files to the staging area
git add .

# 4️⃣ Create your first commit with a descriptive message
git commit -m "Initial commit"

# 5️⃣ Connect your local folder to the remote GitHub repository
# (Copy the HTTPS URL from your GitHub repo)
git remote add origin https://github.com/your-username/your-repository.git

# 6️⃣ Push your files to the main branch (main or master)
git branch -M main
git push -u origin main

# 7️⃣ (Optional) If you already have changes in GitHub, pull them first
git pull origin main

# 8️⃣ (Optional) For future updates
git add .
git commit -m "Description of changes"
git push

#============================================
#Initial Git Configuration (only needed once)
#============================================
# Set your username
git config --global user.name "Your Name"

# Set your email (same one you use for GitHub)
git config --global user.email "youremail@example.com"