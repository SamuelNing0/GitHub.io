# Hosting a Markdown Formatted Resume on Github Pages
![resume](assets/resume.gif)
## Purpose
This README tutorial goes over the practical steps of hosting a markdown formatted resume on a GitHub page. Meanwhile these steps will showcase the key principles explained in the book *Modern Technical Writing* by Andrew Etter, including using lightweight markup languages, employing a static site generator, and hosting documents on a distributed version control system.

---
## Prerequisites
1. Make sure you have an **up-to-date resume properly formatted in markdown**. We need a markdown formatted resume to generate a static website. Markdown is a popular lightweight markup language to write your document. You can learn about markdown [here](https://www.markdowntutorial.com/) or check out [More Resources](#more-resources) if you are not familiar with markdown.
2. You must have a **GitHub account**. If you don't have one, [create a github account here](https://github.com).
3. Have a text editor installed on your computer (such as [Visual Studio code](https://code.visualstudio.com)).
4. Have [GitHub Desktop](https://desktop.github.com) installed on your computer. 
---
## Instructions
### Step 1: Create a personal repository on GitHub
> GitHub is a distributed version control system (DVCS) using Git behind the scenes. You can imagine GitHub as a folder that everyone can access and copy to their local machine. Git is your assistant that keeps every change you make in the folder. As discussed in Modern Technical Writing, 'all sorts of people have extolled the virtues of distributed version control systems (DVCS) like Git.' Etter believes that technical writers can benefit from using DVCS as it is widely used by developers. Using DVCS makes it easier for everyone to contribute to the documentation. Moreover, GitHub keeps track of all the changes to your resume, and your readers can always see your most up-to-date resume.
1. Sign in to your [GitHub](https://github.com) account.
2. Click the plus sign on the top right corner to create a new repository.![newrepo](assets/newrepo.gif)
3. Name your repository "yourUserName.github.io"(yourUserName is your actual GitHub account name).![name](assets/name.gif)
4. Choose "Public" option for your repository.![public](assets/public.png)
5. Select "Add a README file".![readme](assets/readme.png)
   > According to Etter's book, all repositories should have a "README" file containing summary, instructions on how to contribute etc. We are not using it here but it's good practice to include one.
6. Click "Create Repository" to create your personal repository.![create](assets/create.gif)

### Step 2: Clone the repository to your local machine.
> According to Etter's book, DVCS allow people to clone the repository to their local machine and work on it offline. 
1. Sign in to GithHub desktop with your GitHub account. 
2. Click "File" on the top left corner to clone the repository.![file](assets/file.gif)
3. Choose a folder that you want to save the repository to.![path](assets/path.png)
4. Select the repository you created in step 1.3 \(yourUserName.github.io).
5. Click "Clone" to finish cloning the repository from GitHub to your local machine. ![clone](assets/clone.gif)
6. Select "main" for your current branch.![branch](assets/branch.png)

### Step 3: Add your resume to your local repository.
> Your resume must be formatted in Markdown, a popular lightweight markup language mentioned in Etter's book. Markdown is easy to learn, much shorter than XML-based languages, and has broad compatibility with many platforms. It can be converted to a variety of formats, including HTML and PDF.
1. Go to the Repository folder \(yourUserName.github.io) you saved in Step 2.4.
2. Put your \"resume.md\" in this folder. 
3. Rename your resume to \"index.md\".

### Step 4. Configure theme for your resume.
> Etter recommends using a customized theme when building a static webpage to make it stand out. We are using GitHub's default jekyll theme here for simplicity. Check out [resources](#more-resources) for using remote themes.
1. Go to [this website](https://pages.github.com/themes/) to choose a theme you like. 
2. Open Visual Studio Code or any other text editor.
3. Create a file named "_config.yml" in your local repository folder from Step 2.4. ![config](assets/config.gif)
4. Put "theme: jekyll-theme-cayman" in your "_config.yml" file (you can replace the "cayman" with the theme of your choice).![theme](assets/theme.png)
5. Save the file "_config.yml".

### Step 5. Push your changes to GitHub.
> "Catalog the diff":Etter recommends recording changes to a product. GitHub keeps track of these changes for you and allows you to document the changes you make.
1. Open GitHub Desktop. 
2. Set your current repository to \"yourUserName.github.io\" if it is not selected.
3. Select "main" for your current branch if it is not selected.
4. Select \"index.md\" and "_config.yml" for the files you want to push.![change](assets/change.png)
5. Write a summary for your changes.![commit](assets/commit.gif)
6. Click "Commit to main" button on the bottome left corner.
7. Click "Push origin" to push your changes to the remote repository on GitHub. ![push](assets/push.gif)

### Step 6. Publish your static page on GitHub. 
> Etter recommends hosting documentation on a website instead of using PDFs or Word documents since websites do not become outdated. Etter also mentioned several advantages of using a static webpage:
> 1. Static webpage does not depend on server. We easily migrate our resume webpage from GitHub to other hosts.
> 2. Static webpage can be easily generated from markdown, using Jekyll. 
> 3. We can generate webpage and test it locally. In this tutorial we can using Github's built in Jekyll to generate a webpage for simplicity. You can check out [resources](#more-resources) for building and testing a webpage locally.
1. Sign in to your [GitHub](https://github.com) account.
2. Click the hamburger button on the top left corder to go to your repository \"yourName.github.io\".![menu](assets/hamburger.gif)
3. Go to your repository setting on the top right corner.![setting](assets/setting.gif)
4. Navigate to "Pages" section on the left sidebar.
5. Select "Deploy from a branch" as your webpage source.
6. Select "main" as the branch to deploy your webpage from.
7. Click the "Save" button. ![page](assets/page.gif)
8. Naviage to "Action" tab where you can see your static website is being deployed.![action](assets/action.gif)
9.  Click "pages build and deployment" and you can see your static website link once it is ready.![deploy](assets/deploy.gif)

___
# FAQs
### Why is my resume not showing up?
* You need to ensure your resume file is named as \"index.md\" for GitHub to use it as the homepage. 

### Why is Markdown better than a word processor?
* Markdown is better than a word processor because it is more widely supported across platforms, portable, and easy to learn. Moreover, Markdown is compatible with version control systems like Git, allowing for tracking changes.

---
## More Resources
- [Markdown Tutorial](https://www.markdowntutorial.com): A step-by-step markdown tutorial that covers common syntax in Markdown, along with examples and practices.
- [Markdown Guide](https://www.markdownguide.org/getting-started/): An overview of Markdown, how it works, and what you can do with it.
- [Geekflare](https://geekflare.com/best-markdown-editors/): A list of several good markdown editors.
- ["Modern Technical Writing" by Andrew Etter](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS): This book discusses some key principles in technical documentation that we follow in this tutorial.
- [Jekyll Quick Start Guide](https://jekyllrb.com/docs/): A quick tutorial for installing Jekyll locally and generating a static webpage from markdown file on your own machine.
- [Beautiful Jekyll](https://beautifuljekyll.com/getstarted/#install-steps-hard): A tutorial for using remote themes.
___
## Authors and Acknowledgements 
### Author
* [Samuel Ning](https://github.com/SamuelNing0/samuelning0.github.io)
### Acknowledgements:

This tutorial follows documentation principles from Andrew Etter's book Modern Technical Writing. Thanks to my group members Yuelang Zhang and Kim Wills for editting my Readme file. 
