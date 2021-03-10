# [Article Link](https://support.atlassian.com/bitbucket-cloud/docs/configure-your-dvcs-username-for-commits/)
## To set your global username/email configuration:
### 1. Open the command line.
### 2. Set your username: 
git config --global user.name "FIRST_NAME LAST_NAME"
### 3. Set your email address: 
git config --global user.email "MY_NAME@example.com"

## To set repository-specific username/email configuration:

### 1. From the command line, change into the repository directory.
### 2. Set your username:
git config user.name "FIRST_NAME LAST_NAME"

### 3. Set your email address:
git config user.email "MY_NAME@example.com"

## Verify your configuration by displaying your configuration file:
cat .git/config