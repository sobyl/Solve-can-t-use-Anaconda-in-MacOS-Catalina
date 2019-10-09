# Solve can't use Anaconda in MacOS Catalina

- 1. Activate bash: $ chsh -s /bin/bash
- 2. Reopen Terminal
- 3. Move folder from ‘Users/Shared/Relocated\ Items/Security/anaconda3’ to ‘/User/my_user/anaconda3’: 
 $ mv Users/Shared/Relocated\ Items/Security/anaconda3/* /User/my_user/anaconda3
- 4. $ export PATH=“/Users/my_user/anaconda3/bin:$PATH”
- 5. Edit file: /Users/my_user/anaconda3/bin/conda :

Edit the first line like: #!/Users/my_user/anaconda3/bin/python

Save changes
- 6. $ /Users/my_user/anaconda3/bin/conda init bash

You have to change my_user to your account name.
