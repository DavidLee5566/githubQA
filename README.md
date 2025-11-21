# GitHub Actions Assessment
## Objective

Create a simple CI pipeline using GitHub Actions that:
- Sets up Python environment on Ubuntu
- Installs dependencies from requirements.txt
- Runs pytest on a Flask application
- Sends Discord notifications on workflow completion
---

## Download Required Files

Download and place these files in your repository:

1. **app.py** - Flask application with multiple endpoints
2. **test_app.py** - Pytest test suite for the Flask app
3. **requirements.txt** - Python dependencies
4. **workflow-template.yml** - Workflow starter template (rename and place in `.github/workflows/`)

---

## Repository Structure

```
your-repository/
├── app.py
├── test_app.py
├── requirements.txt
└── .github/
    └── workflows/
        └── ci.yml  (your completed workflow)
```

---

## Tasks

### Task 1: Setup Python Environment
In your workflow file, add steps to:
- Checkout the code
- Set up Python 3.9 or 3.10

### Task 2: Install Dependencies
- Install packages from requirements.txt

### Task 3: Run Tests
- Execute pytest on test_app.py
- Show verbose output
- Ensure the job fails if tests fail

### Task 4: Discord Webhook Integration
- Create a notification job that always runs (even if tests fail)
- Send a message to Discord with:
  - Workflow status (passed/failed)
  - Repository name
  - Branch name
  - Link to workflow run

---

## Setup Instructions

### Step 1: Discord Webhook
1. A Discord Webhook will be provided. 

### Step 2: Add GitHub Secret
1. Go to your repository Settings
2. Navigate to Secrets and variables → Actions
3. Click "New repository secret"
4. Name: `DISCORD_WEBHOOK_URL`
5. Value: Paste your Discord webhook URL
6. Click "Add secret"

### Step 3: Complete the Workflow
- Use the provided template as a starting point
- Add the required steps for each task
- Test by pushing to your main branch

---

## Testing Your Workflow

1. **GitHub Actions Testing**:
   - Push your code to the main branch
   - Go to the "Actions" tab in your repository
   - Watch the workflow run
   - Discord notification should happen
   - Take a screenshot of the flow

---

## Helpful Resources

- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [GitHub Actions - Python Setup](https://github.com/actions/setup-python)
- [Discord Webhooks Guide](https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks)
- [Pytest Documentation](https://docs.pytest.org/)

---

## Submission
Push your completed workflow to your GitHub repository with all provided files.
You should have the following completed:
1. The workflow runs successfully
2. All tests pass
3. Discord notification is received

Submit screenshots and/or your git url into brightspace as a record.

