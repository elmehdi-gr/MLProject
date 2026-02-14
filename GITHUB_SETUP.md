# GitHub Setup Instructions

Follow these steps to push your project to a new GitHub repository after creating one on [github.com/new](https://github.com/new).

### 1. Initialize Git Repository
Open your terminal in the project folder (`MLProject`) and run:
```bash
git init
```

### 2. Configure Your Identity (If not already set)
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### 3. Add and Commit Files
Add all files to the staging area and commit them:
```bash
git add .
git commit -m "Initial commit of HAR project"
```

### 4. Connect to Remote Repository
Replace `<your-repo-url>` with the URL of the repository you created on GitHub (e.g., `https://github.com/aliahmed/HAR-Project.git`):
```bash
git remote add origin <your-repo-url>
git branch -M main
```

### 5. Push to GitHub
Upload your local commits to the remote repository:
```bash
git push -u origin main
```
