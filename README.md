# TicketMaker Repository

This repository contains the code for the TicketMaker project. Follow the steps below to clone, set up, and contribute to the repository, including generating an HTTPS access token for secure access.

---
## **Prerequisites**

1. Install Python
	1.	Download Python from Company Portal.
	•	Open Command Prompt and type:
    ```python
    python --version
    ```

2. Depedencies
    ### You can run this command:
    ```python 
    pip install -r requirements.txt # requirements.txt should be into the main directory
    ```
    You can also install the depedencies one by one
    ### Some of the required Python modules are:
    ```python
    ## Requests
    pip install requests

    ## Pillow
    pip install pillow

    ## pyinstaller
    pip install pyinstaller

    ```
## **Step 1: Getting Jira Credentials**

Access: https://id.atlassian.com/manage-profile/security/

Click on create and manage API tokens

![1735836507929](image/readme/1735836507929.png)


Then click on Create API Token

![1735840050050](image/readme/1735840050050.png)

Give it a name and copy it. It will be needed because we will set it once in our code.


## **Step 2: Generate an HTTPS Token**

To securely interact with this repository using HTTPS, follow these steps:

1. Log in to your Bitbucket account.
2. Go to **Personal Settings**.
3. Navigate to **HTTP Access Tokens**.
4. Click **Create token**.
5. Add a token name (e.g., `TicketMakerToken`) and ensure it has the necessary repository permissions (read/write).
6. Copy the generated token and save it securely (you will not be able to see it again).

---

## **Step 3: Clone the Repository**

To clone the repository using your HTTPS token and set it up, follow the commands below:

```bash
# Clone the repository
git clone https://<username>:<your-https-token>@git.rdisoftware.com:8443/scm/~jpedro/ticketmaker.git

# Replace <username> with your Bitbucket username (e.g., jpedro)
# Replace <your-https-token> with the token generated in Step 2

# Example:
git clone https://user:account-https-token@git.rdisoftware.com:8443/scm/isct/jiraticketmaker.git


# Navigate into the repository
cd jiraticketmaker


```

## Step 4: Set up Jira credentials

When you run the ticketApp.py for the first time, it will ask for both email and Jira API Token

![credentialsSetup](image/readme/credentialsSetup.png)
Make sure to fill email using @rdisoftware.com.
""
Click on "Save and Continue"

As you fill it, the home screen will load.

![home](image/readme/home.png)

It may take some time to load, as it fetches thousands of data fields.

Click on "Ok"

![saved](image/readme/saved.png)


After no longer than one minute, the home page shows up.
![home](image/readme/home.png)

Hepful git commands:

```bash
# Create a new branch
git checkout -b <branch-name>

# Example:
git checkout -b reviewApp

# Add all files
git add --all

# Commit your changes with a message
git commit -m "Your commit message"

# Example:
git commit -m "Add initial implementation for ticket creation feature"

# Push the branch to the remote repository
git push -u origin <branch-name>

# Example:
git push -u origin reviewApp

# Check repository status at any time
git status

# Pull the latest changes from the remote repository
git pull

# View all remote URLs
git remote -v
```

