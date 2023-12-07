# RBKTN-So-03-23-intro-to-git

## FIRST STEPS 
 __NOTE__ - _make sure you have a GitHub account_   
 __NOTE__ Set your name and email in the terminal(Git Bash) by following these
```sh
git config --global user.name YOUR_GUTHUB_NAME
git config --global user.email YOUR_GUTHUB_EMAIL
```
## THIS REPO 
1. Fork this repo.

2. From your Terminal, clone the _forked_ repo to your local Desktop, (you can find it in your Github repositories).
   git clone https://github.com/YourUserName/RepoName

3. From your terminal, Navigate to _the forked repo_.  
   cd RBKTN-So-03-23-intro-to-git OR just open the terminal inside the forked folder.
   
4. Read the questions, solve it, and save.

5. Use git status to check the changed files.
   ```sh
   git status
   ```
6. Stage the changes of the file.
   ```sh
   git add fileName.js
   ```
7. Commit your changes
    ```sh
   git commit -m "YOU_MESSAGE"
   ```
8. Push your code to your GitHub account
    ```sh
   git push origin main
   ```
9. when you execute the command push, you will be instructed to sign in with your account username and password,   
**ON windows** it's only the first time, and the pc will automatically save your credentials for you.  
**ON Linux**, you will need to enter your credentials every time you want to push to your repo 

10. You are all done!(just check your Github Repo to see the last commit)
