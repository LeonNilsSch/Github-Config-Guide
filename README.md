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

Optional kann man noch einen Alias erstellen, QUALITY OF LIFE change:

	alias switch_to_work=“~/switch_to_work.sh“
	alias switch_to_private=“~/switch_to_private.sh“


## THATS IT HAVE FUN WITH IT !!!!!
	






