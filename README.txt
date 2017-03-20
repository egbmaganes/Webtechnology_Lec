========================================================================================================================================
Setting up the site:
========================================================================================================================================

Access website locally:
	1. Unzip the file that contains the entire course website.
	2. Open the course website folder and double click on index.html to open the website.
	
========================================================================================================================================

Through firebase:
Important: Make sure to have an Internet Connection.
	1. Go to "firebase.google.com" then create a user.
	2. After creating a user, click on "Console" then select "Create New Project".
	3. After filling the requirements, you will have your project.
	4. In order to host your website, you have to install "node.js" which is available at "nodejs.org". Make sure to download the current or latest version.
	5. After downloading and installing "node.js", go to command prompt.
	6. Type the following in the command prompt:

		nmp install -g firebase-tools <enter>
		firebase login <enter>
		You'll see a question "Allow Firebase to collect anonymous CLI usage information? <Y/n>" Type "Y" <enter>

	7. You'll be prompt by a Request for Permission. Just select "Allow", then you'll be successfully log in.
	8. Now create a public folder (which firebase will be looking for). Just name the folder "public".
	9. Move the files needed for your website to the public folder. Make sure that the main page of your website should named "index.html", otherwise firebase will not recognize it.
	10. Open the command prompt and go to the directory where the public folder is located (e.g C:\Users\John\Desktop>) and type the following:
		
		firebase init <enter>

		When it asked you the following questions...
		"Are you ready to proceed? <Y/n>" Type "Y" <enter>
		"What Firebase CLI features you want to setup for this folder?" Choose "Hosting" <enter>
		"What do you want to use as your public directoy?" Type "public" <enter>
		"Configure as a single-page app (rewrite all urls to /index.html)?" Type "N" <enter>
		"File public/index.html already exists. Overwrite?" Type "N" <enter>
		"What Firebase project do you want to associate as default?" Choose the project that you created on firebase.google.com 		<enter>
		
		firebase deploy <enter>

	11. Copy the URL beside "Hosting Site" then open a browser and paste it on the URL bar.
	12. The website will be available online via the URL given by Firebase.


