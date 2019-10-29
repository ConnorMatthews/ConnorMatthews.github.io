# How to Format a Resume using Markdown and Host it Online For Free.
By Connor Matthews

## Introduction 
This is a tutorial intended for those with no experience with Markdown and Jekyll and some knowledge of Github. It shows how these tools can be used to format a resume and host it on a themed webpage. An example of the finished product can be found [here](https://connormatthews.github.io/). The expected experience level for this tutorial is no experience in Markdown and Jekyll, and some experience in GitHub.
## Prerequisites 
For this tutorial you should already have a resume made in a word processor. Your resume should be logically divided into sections such as work experience, education and technical skills. You will also need to have a GitHub account, and Git installed on your computer. Some parts will require you to use Git Bash. It is assumed that you know (or can figure out how) to do basic terminal tasks like navigating through file hierarchies. This Tutorial was done on a Windows 10 computer so step details may vary on different operating systems.

## Part 1: Formatting a resume with Markdown
Markdown is a markup language. That means it uses certain symbols to format a text document. Markdown features a very simple syntax and is widely supported and extended. You will see how Github and Jekyll interact with Markdown shortly.
### Markdown Syntax
Here is all of the Markdown you will need to know to format your resume.

| Syntax     | Result                                                         |
| ------------ | ------------------------------------------------------------ |
| # Header     | The text 'Header' is formatted as a page header.             |
|	- List Item: | The text ‘List Item’ is formatted as an unordered list item. |
|	1. List Item:| The text ‘List Item’ is formatted as a numbered list item.   |
|	\_\_Bold Text__| The text ‘Bold Text’ is formatted as __bold text__.        |
|	\_Italic Text_| The text ‘Italic Text’ is formatted as _italic text_.      |
- Note: There are six different types of page headers. One '#' is reffered to as a top level header, and ###### is the smallest header.

That’s it! You are now ready to convert your resume to Markdown. Here are the step-by-step instructions for doing so.
1.	Download the Atom installer here (https://atom.io/). Atom is a free to use text editor with excellent support for writing markdown documents.
2.	Install Atom by following the installer instructions.
3.	Open Atom. You can close the welcome screens that appear on start up.
4.	(Optional) Change from the default theme to a light theme. The light theme may seem more natural when working with your resume
a.	Click the settings option under the file dropdown menu.
b.	Select Themes from the menu on the left.
c.	Change the UI and syntax theme to a light one.
5.	Create a new file, use the keyboard shortcut Ctrl+N
6.	Open your resume in whatever word processor you used to make it (e.g. Microsoft Word).
7.	Copy the text of your resume into the new file in Atom.
8.	Save your Atom file as a .md file.
9.	Open the Markdown preview screen in Atom by opening the ‘Packages’ dropdown, navigating to the ‘Markdown Preview’ option and clicking ‘Toggle Markdown Preview’. A new window will appear on the right side of the editor which will show the formatted version of your resume for easier editing.
10.	Format your name with a top level header (one ‘#’). 
11.	Format the titles of the segments of your resume with lower level headers. Second or third level headers work well here.
12.	Use even lower level headers for any further titles under the segments. For example, you might want to use headers for job names and titles.
13.	Use list formatting for any writing that describes a part of your resume in more detail. For example, the descriptions of your accomplishments at a certain job.

Pro Tip: You should avoid indenting any of your lists, GitHub will do this automatically once your resumed has been copied over there later on.  
At this point, all aspects of your resume should be formatted in Markdown. You can verify this by looking at the preview window.

## Part 2: Putting a resume online with GitHub Pages
Now that you have a markdown formatted resume file, it is time to host it online. For this exercise, you will learn how to do this with GitHub Pages. Github pages is a feature tied to a Github repository that allows you to host files from the repository as web pages that can be view online by anyone. A Github account gets one Github pages repository to use for free. Here is how it is done.
1.	Log in to your Github account.
2.	Create a new public repository. The Repositories name must be your account name, followed by ‘github.io’
3.	Create a folder on your computer. This will be used to hold a local version of the repository you just created
4.	Navigate to the folder in Git Bash
5.	Type ‘git clone https://repo_name’ where ‘repo_name’ is the name of the repository you created in step 2. You will now have a local copy of the repository in this folder.
6.	Copy your resume .md file and paste it into the folder. Rename it to index.md. The ‘index’ file is the file GitHub will serve when someone goes to your site  address).
7.	Add your file to the local repository with the command ‘git add index.md’ using Bash.
8.	Commit your change with the command ‘git commit -m <message>’ using Bash. For the message, choose something relevant like ‘Added resumes as index file’.
9.	Push your changes to the central repository with the command ‘git push -u origin-master’ using Bash.
10.	Check your repository on the GitHub site and verify that the index.md file has been added.
11.	Enter the address ‘https://repo_name’ into the web browser of your choice, where ’repo_name’ is the name of your repository in step 2. You should see your markdown formatted resume in all of its glory. 
  
## Part 3: Using a Jekyll Theme 
The last thing left to do is give your resume website a fancy theme. Github supports applying themes to markdown formatted text documents using a static site generator called Jekyll. For this exercise you will use one of the default themes that GitHub offers. However, with Jekyll you can create your own themes or customize one created by other people if you are so inclined. 
1.	Navigate to the settings page of your Github Pages repository.
2.	Under the ‘GitHub Pages’ selection click the button to choose a theme. This will take you to a new page showcasing the different options.
3.	Choose one of the themes with the green ‘Select Theme’ button.
4.	View your site. It should now have the chosen theme. It may take a few moments for the changes to take place.

## Concluding remarks
You should now know everything you need to format a resume with markdown and host it online with GitHub pages. If you want to go further with this topic, an interesting thing to do would be to use a custom Jekyll theme for your site rather than one of the Github defaults. 

## Further Resources
- A good Markdown Tutorial: https://www.markdowntutorial.com/
- The official Jekyll tutorial: https://jekyllrb.com/docs/step-by-step/01-setup/

## Frequently Asked Questions
__Q.__ Do I really have to download a new text editor just for writing in Markdown? 
__A.__ No, there are websites that work in much the same way as Atom does. some examples are markdownlivepreview.com and dillinger.io

# Acknowledgements 
Big thanks to the Group 18 crew (Kyle Boch and Jonathan Kuz) for ideas and editing.
Thank you to Bill Gates for inventing the computer.
