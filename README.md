## MY README.File FOR MY GIT CONFIGURATION

Navigate to your Home directory:

	cd ~



Create 2 shell scripts, one for Work and one for Private Repos:


	touch switch_to_work.sh
	touch switch_to_private.sh


Editiere diese Scripts indem du sie in einem Code Editor deiner Wahl öffnest:

	code switch_to_work.sh


Edit these scripts by opening them in a code editor of your choice:

	git config —global user.name “Your Work Name“
	git config —global user.email “Your Work Email“


Save and close the file and do the same with the Private Config:

	code switch_to_work.sh
	git config —global user.name “Your Private Name“
	git config —global user.email “Your Private Email“


Now you have to make the scripts executable so that you can run them:

	chmod +x switch_to_work.sh
	chmod +x switch_to_private.sh


Now the script is completely configured and if you want to switch between the configs run:

	./switch-to-work.sh
	./switch-to-work.sh

__Optional__: you can create an alias, QUALITY OF LIFE change:

Here's how you can do it:

1. **Open your shell configuration file:**
   - Depending on which shell you're using, open the appropriate configuration file. For example, if you're using Bash, you'll typically edit `~/.bashrc`. If you're using Zsh, you'd edit `~/.zshrc`.
   - You can open the file in a text editor like VSCode:
     - For Zsh:
       ```
       code ~/.zshrc
       ```

2. **Add alias definitions:**
   - Inside the file, add the alias definitions for `switch_to_work` and `switch_to_private` at the end:
     ```bash
     alias switch_to_work="/Users/blank/switch_to_work.sh"
     alias switch_to_private="/Users/blank/switch_to_private.sh"
     ```
   - Replace `/User/blank/` with the actual path to your scripts.

3. **Save and exit the editor:**
   - In nano, you can save the changes by pressing `Ctrl + O` (to write out) and then `Enter`, and then exit VSCode by pressing `Ctrl + X`.

4. **Apply changes:**
   - After saving the file, you need to apply the changes to your current shell session. You can do this by running:
     - For Zsh:
       ```
       source ~/.zshrc
       ```
   - This command reloads the configuration file, making the aliases available in your current session.
   
Now, the aliases should persist across terminal sessions, and you should be able to use `switch_to_work` and `switch_to_private` commands without any issues, even after restarting the terminal.







## THATS IT HAVE FUN WITH IT !!!!!
	






