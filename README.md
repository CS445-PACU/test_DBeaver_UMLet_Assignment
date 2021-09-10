# test_DBeaver_UMLet_Assignment

Use this project to pull in a GitHub Classroom assignment, edit a SQL file in DBeaver, and edit an ER diagram in UMLet.

Prior to this: Setup your SSH Keys on GitHub and your VM.

See [Moodle](moodle.pacificu.edu) for videos on SSH Keys (Linux Videos) and this exercise (CS445 Videos).

Basic Script:

1. In the Web Browser - Accept the assignment.
1.1 Go to the repository in your browser.  Green Code button, SSH, copy Git Clone Address

2. Open a Terminator window.

3. mkdir git # might already exist

3. cd git

4. mkdir cs445f21

5. cd cs445f21

6. git clone COPIED_URL_FROM_ABOVE
	
	EXAMPLE:
   git clone git@github.com:will4614/Dbeaver_SQL_TEST.git

7. cd Dbeaver_SQL_TEST # repository name from the end of the URL above

8. ls -l # verify your success

9. Open dbeaver:
	dbeaver & # or click on the icon
	
10. In dbeaver, make a connection to your local DB.
	10.1 plug +
	10.2 MariaDB
	10.3 Next >
	10.4 
		* Database: NAME_test
		* Username: punetid
		* Password: <secret password>
		* X Save Password Locally
		* Test Connection
		* Finish
	10.5 File | Open File | Navigate to git/cs445f21/Dbeaver_SQL_TEST/test.sql
	10.6 Set data source and database at top
	10.7 Write SQL, run SQL, File | Save

11.	In the Terminal:
	* git status
	* git add .  # or git add test.sql
	* git commit -m "useful message"
	* git push
	
12. Refresh repository in the browser to confirm the push was successful.

13. Repeat steps 10.5 - 11 as necessary.

14. UMLet:
	14.1 Open UMLet (slow the first time each session)
	14.2 File | Open | Navigate to git/cs445f21/Dbeaver_SQL_TEST/test.uxf
	14.3 UPDATE DIAGRAM
	14.4 File | Save

15.	In the Terminal:
	* git status
	* git add .  # or git add test.uxf
	* git commit -m "useful message"
	* git push

16. Refresh repository in the browser to confirm the push was successful.

13. Repeat steps 14.3 - 15 as necessary.
