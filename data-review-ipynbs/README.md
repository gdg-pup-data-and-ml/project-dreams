# Data Review Notebooks (`data-review-ipynbs`)

[![DataCamp Data Connector](https://img.shields.io/badge/-DataCamp%20Data%20Connector-005BBB?style=flat-square&logo=datacamp&logoColor=white)](https://enterprise-docs.datacamp.com/)

## Introduction

Welcome to the `data-review-ipynbs` folder of **Project DREAMS: DataCamp Resources & Engagement Analytics Monitoring System**! This folder is where contributors will submit their Google Colab notebooks containing the 5 research questions and analyses as outlined in the **Project DREAMS: Data Analysis Assignment**. The dataset for this assignment is sourced from the DataCamp Data Connector (see shield above for documentation). This README provides step-by-step instructions to help you submit your work, even if you're new to Git and GitHub.

## Purpose
The `data-review-ipynbs` folder is dedicated to storing Google Colab notebooks (`.ipynb` files) with your research questions and insights for Project DREAMS. Your submissions here will help us build a robust analytics platform for tracking DataCamp scholar engagement.

## Submission Guidelines
1. **File Name Format**: Name your notebook file as `SURNAME_DataReview.ipynb` (e.g., `CURADA_DataReview.ipynb`).
   - Use your surname in ALL CAPS, followed by `_DataReview`.
   - Ensure the file is a `.ipynb` file downloaded from Google Colab.
2. **Notebook Content**: Your notebook must include:
   - **Introduction**: A brief overview of your approach.
   - **Research Questions**: 5 questions with explanations, tables/columns, methodology, and potential insights (see assignment details).
   - **Conclusion**: How your insights benefit Project DREAMS.
   - Use Markdown cells for formatting.
3. **Due Date**: Submit by **March 14, 2025**.
4. **Commit Message**: Use a clear commit message like:  
   `"Add SURNAME_DataReview.ipynb with 5 research questions"`

## Prerequisites
- You need **Git** installed on your computer to collaborate via GitHub.
- You must be a contributor to the `gdg-pup-data-and-ml` organization with **write access** to this repository.

## Step-by-Step Instructions
Follow these steps to submit your work. These are written for beginners, so don’t worry if you’re new to Git!

### 1. Check if Git is Installed
- Open your **Command Prompt** (Windows) or **Terminal** (Mac/Linux).
- Type the following command and press Enter:
  ```
  git --version
  ```
- If you see a version number (e.g., `git version 2.39.2`), Git is installed. Move to Step 2.
- If you get an error like "command not found," download and install Git from [git-scm.com](https://git-scm.com/downloads), then repeat this step.

### 2. Clone the Repository
- Clone the Project DREAMS repository to your computer:
  ```
  git clone https://github.com/gdg-pup-data-and-ml/project-dreams
  ```
- This creates a `project-dreams` folder on your computer with all the repo contents.

### 3. Navigate to the Repository
- Move into the `project-dreams` folder:
  ```
  cd project-dreams
  ```

### 4. Set Up Your Git Identity
- Configure your name and email (only need to do this once on your computer):
  ```
  git config --global user.name "Your Full Name"
  git config --global user.email "your.email@example.com"
  ```
  - Replace `"Your Full Name"` with your name and `"your.email@example.com"` with the email tied to your GitHub account.

### 5. Set Up Authentication
- GitHub requires a Personal Access Token (PAT) instead of a password. Set this up once:
  1. Go to [github.com/settings/tokens](https://github.com/settings/tokens).
  2. Click **Generate new token** > **Generate new token (classic)**.
  3. Name it (e.g., "Project DREAMS"), set expiration (e.g., 30 days), check the **repo** scope, and click **Generate token**.
  4. Copy the token (e.g., `ghp_xxxxxxxxxxxxxxxxxx`).
- Store your credentials so you don’t have to enter them repeatedly:
  ```
  git config --global credential.helper store
  ```
  - The first time you push, you’ll enter your GitHub username and PAT. Git will save them for future use.

### 6. Switch to the `data-review` Branch
- Move to the `data-review` branch where we’ll submit work:
  ```
  git checkout data-review
  ```
- **Note**: If you see an error like "error: pathspec 'data-review' did not match any file(s) known to git," the branch doesn’t exist yet. Create it with:
  ```
  git checkout -b data-review
  ```
  - This creates and switches to the `data-review` branch.

### 7. Go to the `data-review-ipynbs` Folder
- Move into the `data-review-ipynbs` folder:
  ```
  cd data-review-ipynbs
  ```

### 8. Add Your Notebook
- After completing your assignment in Google Colab, download your notebook as a `.ipynb` file (File > Download > Download .ipynb).
- Copy or move your `SURNAME_DataReview.ipynb` file into the `data-review-ipynbs` folder using your file explorer.

### 9. Update Your Local Branch
- Before committing, pull any updates from the `data-review` branch on GitHub:
  ```
  git pull origin data-review
  ```
- If you see "Already up to date," proceed. If there are conflicts, ask for help.

### 10. Check the Status
- Check what’s changed:
  ```
  git status
  ```
- You should see your file listed under "Untracked files" or "Changes not staged for commit."

### 11. Add Your File to Git
- Tell Git to track your file:
  ```
  git add SURNAME_DataReview.ipynb
  ```
  - Replace `SURNAME` with your surname (e.g., `git add CURADA_DataReview.ipynb`).

### 12. Commit Your Changes
- Save your changes with a descriptive message:
  ```
  git commit -m "Add SURNAME_DataReview.ipynb with 5 research questions"
  ```
  - Replace `SURNAME` with your surname (e.g., `git commit -m "Add CURADA_DataReview.ipynb with 5 research questions"`).

### 13. Push Your Work to GitHub
- Send your changes to the `data-review` branch on GitHub:
  ```
  git push origin data-review
  ```
- The first time, enter your GitHub username and paste your PAT when prompted. After that, Git should remember them.

### 14. Verify Your Submission
- Visit [https://github.com/gdg-pup-data-and-ml/project-dreams/tree/data-review/data-review-ipynbs](https://github.com/gdg-pup-data-and-ml/project-dreams/tree/data-review/data-review-ipynbs) in your browser.
- Check that your `SURNAME_DataReview.ipynb` file appears in the folder.

## Tips for Beginners
- **Branch Issue?** If `git checkout data-review` fails and you created it with `git checkout -b data-review`, your push will set it up on GitHub.
- **Push Failed?** If you get "rejected" or "non-fast-forward," run `git pull origin data-review`, resolve conflicts (ask for help if needed), then push again.
- **Made a Mistake?** Before pushing:
  - Unstage a file: `git restore --staged SURNAME_DataReview.ipynb`
  - Discard changes: `git restore SURNAME_DataReview.ipynb` (careful—this deletes unsaved changes!).
- **Authentication Issues?** If prompted repeatedly for credentials, ensure you ran `git config --global credential.helper store` and used your PAT correctly.

## Need Help?
- Contact **John Paul Curada** or **Jen Patrick Nataba** via the GDG PUP communication channel.
- Post your question in our team chat—someone will assist you!

## Next Steps
- Be ready to discuss your research questions in our next team meeting after submission.
- Your work here will directly contribute to Project DREAMS’ analytics platform!

Happy coding, and thank you for contributing to **Project DREAMS**!

