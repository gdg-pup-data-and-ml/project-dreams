# Data Review Notebooks (`data-review-ipynbs`)

[![DataCamp Data Connector](https://img.shields.io/badge/-DataCamp%20Data%20Connector-005BBB?style=flat-square&logo=datacamp&logoColor=white)](https://enterprise-docs.datacamp.com/)

## Introduction

Welcome to the `data-review-ipynbs` folder of **Project DREAMS: DataCamp Resources & Engagement Analytics Monitoring System**! This folder is where contributors will submit their Google Colab notebooks containing the 5 research questions and analyses as outlined in the **Project DREAMS: Data Analysis Assignment**. The dataset for this assignment is sourced from the DataCamp Data Connector (see shield above for documentation). This README provides step-by-step instructions to help you submit your work, even if you're new to Git and GitHub.

### Important Note on Repository Access and Branch Permissions
As a member of the GDG On Campus PUP organization, you do not automatically have access or permission to commit to this repository. Access depends on:
- **Organization base permissions**: Check if the organization grants "Write" access to all members.
- **Repository-specific permissions**: You must be explicitly granted "Write" or higher access to this repository, either individually or through a team.
- **Team membership**: If you're part of a team with access to this repository, your permissions align with the team's settings.

**Branch Restrictions**:
- Contributors are **only allowed to push changes to the `data-review` branch**.
- Direct pushes to the `main` branch are **not permitted**. All changes to `main` must be submitted via pull requests (PRs) and approved by maintainers.
- Branch protection rules are enforced to ensure this workflow. If you attempt to push to `main`, you will receive an error.

If you cannot commit or push to the `data-review` branch, contact the project lead (John Paul Curada) or an organization owner to verify your permissions. For more details, refer to GitHub's documentation on [organization permissions](https://docs.github.com/en/organizations/managing-access-to-your-organizations-repositories).

---

## Assignment Overview

Your task is to:
1. Review the [DataCamp Data Connector documentation](https://enterprise-docs.datacamp.com/data-connector/explore-data-model/data-model).
2. Formulate **5 research questions** that provide valuable insights for tracking and improving DataCamp scholar engagement.
3. For each question:
   - Explain its relevance to Project DREAMS objectives.
   - Identify the tables and columns needed to answer the question.
   - Describe any joins, aggregations, or calculations required.
   - Explain how the insights could improve scholar management.

---

## Submission Guidelines

Follow these steps to submit your work to the `data-review-ipynbs` folder. Ensure you adhere to the file naming, formatting, and commit message conventions. **All submissions must be pushed to the `data-review` branch, not `main`.**

### 1. Prepare Your Google Colab Notebook
- Create a Google Colab notebook for your assignment.
- Use the filename format: `SURNAME_DataReview.ipynb` (e.g., `CURADA_DataReview.ipynb`).
- Structure your notebook with the following sections using Markdown cells:
  - **Introduction**: Brief overview of your approach.
  - **Research Questions**: Your 5 research questions, each including:
    - The question itself.
    - Relevance to Project DREAMS objectives.
    - Tables and columns required from the DataCamp Data Connector.
    - Methodology (joins, aggregations, calculations).
    - Potential insights and actions.
  - **Conclusion**: Summarize how your insights would benefit Project DREAMS.
- Ensure your notebook uses proper Markdown formatting for readability.

### 2. Download Your Notebook
- Download your Google Colab notebook as an `.ipynb` file:
  - Go to `File > Download > Download .ipynb`.
  - Save the file with the correct filename (e.g., `SURNAME_DataReview.ipynb`).

### 3. Check Your Repository Setup
- **If you have already forked and cloned the repository** (i.e., you completed these steps for a previous submission):
  - Skip to **Step 4 (Update Your Local Repository)**.
- **If you have NOT previously forked and cloned the repository**:
  - Follow **Steps 4-6** to set up your repository, then proceed to **Step 7**.

### 4. Fork the Repository (First-Time Setup Only)
- Go to the main repository page on GitHub.
- Click the **Fork** button in the top-right corner to create a copy of the repository under your GitHub account.
- This fork will allow you to make changes and submit pull requests.

### 5. Clone the Repository (First-Time Setup Only)
- Clone your forked repository to your local machine:
  ```bash
  git clone <your-forked-repo-url>
  ```
  - Replace `<your-forked-repo-url>` with the URL of your forked repository (found on GitHub under "Code").
- Navigate to the repository folder:
  ```bash
  cd <repository-name>
  ```

### 6. Set Up the Upstream Remote (First-Time Setup Only)
- Add the original repository as an upstream remote to keep your fork updated:
  ```bash
  git remote add upstream <original-repo-url>
  ```
  - Replace `<original-repo-url>` with the URL of the main repository (e.g., `https://github.com/<org-name>/<repo-name>.git`).

### 7. Update Your Local Repository (For Returning Contributors)
- If you already have the repository cloned, ensure your local copy is up-to-date with the main repository:
  ```bash
  git fetch upstream
  git checkout main
  git merge upstream/main
  ```
- Push the updates to your fork:
  ```bash
  git push origin main
  ```

### 8. Switch to the `data-review` Branch
- Switch to the `data-review` branch in your local repository:
  ```bash
  git checkout data-review
  ```
- If the `data-review` branch does not exist locally, pull it from the upstream repository:
  ```bash
  git checkout -b data-review
  git pull upstream data-review
  ```

### 9. Add Your Notebook to the Repository
- Copy your downloaded `.ipynb` file (e.g., `SURNAME_DataReview.ipynb`) into the `data-review-ipynbs` folder in your local repository.
- Stage the file for commit:
  ```bash
  git add data-review-ipynbs/SURNAME_DataReview.ipynb
  ```

### 10. Commit Your Changes
- Commit your changes with a clear and descriptive commit message:
  ```bash
  git commit -m "Add data review notebook for <Your Surname>"
  ```
  - Example: `git commit -m "Add data review notebook for Curada"`.

### 11. Push Your Changes to the `data-review` Branch
- Push your changes to the `data-review` branch in your forked repository:
  ```bash
  git push origin data-review
  ```
- **Note**: You cannot push directly to the `main` branch due to branch protection rules. If you attempt to push to `main`, you will receive an error.

### 12. Create a Pull Request (PR)
- Go to your forked repository on GitHub.
- You should see a banner indicating that you recently pushed to the `data-review` branch.
- Click **Compare & pull request**.
- In the pull request:
  - Use the title: `Data Review Submission - <Your Surname>` (e.g., `Data Review Submission - Curada`).
  - Add a description:
    ```
    - Submitted data review notebook: <SURNAME_DataReview.ipynb>
    - Contains 5 research questions and analyses for Project DREAMS.
    - Ready for review.
    ```
- Ensure the PR is targeting the `main` branch of the original repository.
- Submit the pull request.

---

## Due Date
- **Submission Deadline**: March 14, 2025.
- Be prepared to discuss your research questions in the next team meeting.

---

## Evaluation Criteria
Your submission will be evaluated based on:
- Relevance to Project DREAMS objectives.
- Clarity and specificity of research questions.
- Appropriate identification of data tables and columns.
- Creativity and insight in proposed analyses.
- Actionability of potential insights.
- Proper use of Markdown formatting in the notebook.

---

## Troubleshooting
- **Cannot push to `data-review` branch**: Verify your permissions with the project lead or organization owner.
- **Cannot push to `main` branch**: This is expected due to branch protection rules. Ensure you are pushing to the `data-review` branch.
- **Merge conflicts**: If your PR has conflicts, resolve them locally by pulling the latest changes from `upstream/main`, merging them into your `data-review` branch, and pushing the updated branch.
- **Need help with Git/GitHub**: Reach out to the project lead or refer to GitHub's documentation.

---

## Questions?
If you have any questions or need assistance, contact the project lead (John Paul Curada) or open an issue in the repository.

Happy analyzing, and thank you for contributing to Project DREAMS! 🚀

