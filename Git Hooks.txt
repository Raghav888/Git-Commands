1. Git hooks are inbuilt features in git.
2. Two groups in git hook
   - Server side hook ->  runs on remote repo
   - Client side hook -> runs on local repo
3. Server side hooks are executed before or after certain action happens on remote repo.
4. Client side hooks are executed before or after certain actions happens on local repo

NOTE: In .git/hooks folder, we can get all client side hooks.
In those files we can create rules for hooks and enable the required hook.

Few Client side hooks
5. Pre-commit hook -> will be executed before commit happens. If it fails, commit wont happen. Ex: check lint before commit
6. Post-commit hook -> will be executed after commit happens. Can be used to run UT,etc, before pushing the code to remote repo.

Few Server side hook
7. Once code is pushed to remote, pre-receive hook is executed before updating the remote repo with new changes. If this hook fails, the push is rejected.
8. post-receive hook -> Once code is succesfully updated with push, then this hook will run. It can be used to send notification, run deployment, execute any script,etc 
after code is updated.

Why to use Githooks?
1. Increases productivity
2. Helps to automate to run custom script.
3. Saves developer time
4. Reduces failure of build on remote, by checking lint/UT issues before commit
