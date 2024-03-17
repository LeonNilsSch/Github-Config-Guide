## MY README.File FOR MY GIT CONFIGURATION

Navigiere in dein Home Directory:

	cd ~



Erstelle 2 Shell Scripts, eine für Work und eine für Private Repos:


	touch switch_to_work.sh
	touch switch_to_private.sh


Editiere diese Scripts indem du sie in einem Code Editor deiner Wahl öffnest:

	code switch_to_work.sh


Füge folgenden Code hinzu und füge in den Klammern deine Daten hinzu:

	git config —global user.name “Your Work Name“
	git config —global user.email “Your Work Email“


Save und schliesse die File und mach das selbe mit der Private Config:

	code switch_to_work.sh
	git config —global user.name “Your Private Name“
	git config —global user.email “Your Private Email“


Nun muss man die scripts executable machen damit man sie run kann:

	chmod +x switch_to_work.sh
	chmod +x switch_to_private.sh


Damit wäre das Script komplett konfiguriert und wenn man nun zwischen den configs switchen möchtest run:

	./switch-to-work.sh
	./switch-to-work.sh

__Optional__ kann man noch einen Alias erstellen, QUALITY OF LIFE change:

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
	






