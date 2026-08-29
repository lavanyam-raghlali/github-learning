# How to Upload Files to the Repository

This guide explains how to add and upload files to this GitHub repository using both the web interface and command-line tools.

## Method 1: Using GitHub Web Interface

### Steps:
1. **Navigate to the repository** on GitHub.com
2. **Click the "Add file" button** (usually near the top-right of the file list)
3. **Select "Upload files"** from the dropdown menu
4. **Drag and drop files** or click "choose your files" to browse
5. **Add a commit message** describing what you're uploading
6. **Click "Commit changes"** to upload the files

### When to Use:
- Quick uploads of one or two files
- When you don't have git installed
- For adding files from a web browser

---

## Method 2: Using Git Command Line

### Prerequisites:
- Git installed on your computer
- Repository cloned locally
- Basic terminal/command-line knowledge

### Steps:

#### 1. Clone the Repository (if you haven't already)
```bash
git clone https://github.com/lavanyam-raghlali/github-learning.git
cd github-learning
```

#### 2. Add Your Files
Copy or move your files to the repository folder.

#### 3. Stage the Files
```bash
# Add a specific file
git add filename.txt

# Add all new files
git add .
```

#### 4. Commit the Changes
```bash
git commit -m "Add filename: brief description of what you added"
```

Example:
```bash
git commit -m "Add file upload guide documentation"
```

#### 5. Push to GitHub
```bash
git push origin main
```

If you're working on a different branch, replace `main` with your branch name.

---

## Method 3: Using Git in Visual Studio Code

### Steps:
1. **Open the repository folder** in VS Code
2. **Click the Source Control icon** (left sidebar)
3. **Drag and drop files** into the project folder
4. **Stage changes** by clicking the "+" button next to files
5. **Enter a commit message** in the text box
6. **Click the checkmark** to commit
7. **Click the sync button** to push to GitHub

---

## Best Practices

✅ **Do:**
- Write clear, descriptive commit messages
- Organize files into appropriate folders
- Review changes before committing
- Pull latest changes before pushing

❌ **Don't:**
- Upload sensitive files (passwords, API keys, personal data)
- Commit large binary files without permission
- Push directly to `main` if working in a team (use branches)

---

## Common Issues & Solutions

### Issue: "fatal: not a git repository"
**Solution:** Make sure you're in the repository folder:
```bash
cd path/to/github-learning
```

### Issue: "Permission denied" or authentication error
**Solution:** 
- Set up SSH keys or use GitHub personal access tokens
- Use `git config` to set your GitHub credentials

### Issue: Large file upload fails
**Solution:** 
- Use Git Large File Storage (LFS) for files > 100 MB
- Install and configure: `git lfs install`

---

## Need More Help?

- [GitHub Documentation - Adding files](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [Git Official Documentation](https://git-scm.com/doc)
- Ask a question by creating a new issue!
