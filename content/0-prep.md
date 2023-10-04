---
title: Workshop Prep
nav: Prep
topics: GitHub; Optional Software
---

{% capture text %}Note:
This is a sample instructional page on finding articles. {% endcapture %}
{% include alert.html text=text color=secondary %}

Looking for articles, book chapters, conference proceedings, or other research materials? Databases are the best place to search. The library subscribes to over 200 databases, including many discipline-specific options.

This walkthrough provides steps for using **Academic Search Premier**, a multi-disciplinary database, to search for sources related to the sample topic on *why we sometimes get music stuck in our head*. 


1. From the Library webpage, [lib.uidaho.edu](https://lib.uidaho.edu), click **Academic Search Premier** under the catalog search bar and magnifying glass.

{% include figure.html img="navigate.jpg" alt="Navigate to Academic Search Premier" caption="Navigate to Academic Search Premier" width="75%" %}

`Sign in` to your account using your U of I email and password.

{% include figure.html img="signin.jpg" alt="The sign-in screen" caption="The sign-in screen" width="75%" %}

2. Let’s search for articles related to why we sometimes get music stuck in our head. These are often called earworms. We can type **earworms music brain** keywords in the search box. This is the same as using the Boolean phrase **earworms AND music AND brain** because the database automatically puts an AND in all capital letters between each word. Click search after typing the keywords.

{% include figure.html img="searchscreen.jpg" alt="Academic Search Premier search screen" caption="Academic Search Premier search screen" width="75%" %}

3. After searching and seeing the results page, you can scan the article titles to look for relevant articles. If you want to refine your results, you can navigate to the "Refine Results" and "Limit To" sections to add filters to your search results. You can check the box to narrow down your search to "Peer-Reviewed" journals. You can also choose a specific date range.

{% include figure.html img="searchscreen.jpg" alt="Academic Search Premier search screen" caption="Refine results options" width="75%" %}

The icons in the result list help you know what kind of publication the article is from. 
- In Academic Search Premier, periodical means popular magazine. 
- Academic journal means a journal that publishes scholarly articles. Often these articles are reviewed by other experts in the field. This is called “peer review.” 
- News means articles that have been published in a newspaper.

4. Clicking the title of an article, such as "The Classification of Involuntary Musical Imagery," brings up more information, including an abstract or summary as well as other possible keywords you could use in your search. In this example, you can see that we found a more professional term for earworms: involuntary musical imagery. You can use this phrase in your next search by clicking "involuntary musical imagery."

{% include figure.html img="articlepage.jpg" alt="Article page" caption="Article page" width="75%" %}

On the right, you can email the article to yourself or learn how to cite it.
If you find one good article, look at the subject terms used for that article to help you search for more relevant articles. For example, if you click “involuntary musical imagery,” you can pull up all the other articles tagged with that term.
On this new results list, you will see several options for getting the full text article. If you see HTML, PDF or linked full text, you can simply click the icon or link to view the whole article.
If you see a “check for full text availability” link, it means the library may or may not have access to the full text online. For example, when clicking “check for full text availability” on “Singing in the Brain,” you are taken to our library catalog and can see that the full-text is not available immediately from our library’s resources, but it could be ordered for free from Interlibrary Loan.
In this next example, when clicking “check for full text availability” on “Catching Earworms on Twitter...,” you can see a link to the full article under “View Online.”
It’s always a good idea to collect more articles than you think you might need.
If your search was not successful, you can redo your search by changing your search terms or using limiters. For example, you could search for involuntary memory music to see a new list of results.
Searching for articles can be complex, so don't hesitate to contact the Library for additional assistance. Now you are ready to begin searching for articles.






To create your own materials using `workshop-template-b`, please set up a free [GitHub account](https://github.com/join) if you do not have one already.

Basic familiarity with the GitHub web interface will be helpful.
For a quick introduction check out GitHub's [Hello World guide](https://guides.github.com/activities/hello-world/), or the extensive [GitHub Learning Lab](https://lab.github.com/).

This template works great using only GitHub's web interface for editing--you don't have to install anything!
However, for more advanced uses you will want Git, Ruby, and Jekyll installed on your computer to do local development.

{% capture text %}
1. Have a [GitHub](https://github.com) account.
2. *Very Optional:* have [Git](https://git-scm.com/), [Jekyll](https://jekyllrb.com/), and a nice [text editor](https://code.visualstudio.com/) installed.
{% endcapture %}
{% include card.html text=text header="Setup Overview" %}

> *Tip:* for easier editing of your project in your browser, you can click `.` on any GitHub repository to [open the web editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor) (which is a version of [Visual Studio Code](https://code.visualstudio.com/) editor)!
>
> *Tip:* you could also use this template on GitLab or other hosting service. GitHub is handy for easily creating and sharing projects, however, it is not a dependency!

-------------

## Local Jekyll Setup [very optional]

If you want to develop and preview your website project on your local computer (or deploy it some where other than GitHub Pages), you will need to install Git version control and the static site generator [Jekyll](https://jekyllrb.com/).

### Install Git

[Git](https://git-scm.com/) is a [free](https://www.gnu.org/philosophy/free-sw.en.html), [distributed](https://en.wikipedia.org/wiki/Distributed_version_control) version control system. [GitHub](https://github.com/) is a Git repository hosting service, a place to store and sync your work in the cloud.
Your GitHub project will be under Git version control, so you need the software on your machine. 

- **Windows:** Install [Git for Windows](https://git-scm.com/downloads){:target="_blank" rel="noopener"} using the default options, *except* when setup asks you to choose the default editor used by Git, select "Use the Nano editor by default". This will give you Git, Git Bash, and Git GUI. Git Bash is a terminal that lets you use UNIX style commands and utilities on Windows, and will be used as your default terminal when working with Jekyll.
- **Mac:** Mac systems will require the "Xcode Command Line Tools" installed, so open a terminal (to find your terminal search for "terminal" in your Spotlight), type in the command `xcode-select --install`, and follow the prompts. After the install finishes, try typing `git --version`. If you want a newer version of Git, download the official [Mac git installer](https://git-scm.com/downloads){:target="_blank" rel="noopener"}.
- **Linux:** Install from your distribution's software center or package manager (for Ubuntu `sudo apt install git`).

If you are interested in using a visual GUI application integrated with GitHub, Windows and Mac users should also install [GitHub Desktop](https://desktop.github.com/) using the default options.
You can install GitHub Desktop in addition to other versions of Git.
There are other [GUI apps available](https://git-scm.com/downloads/guis) for managing and visualizing Git repositories, including Linux options.

### Install Ruby

[Ruby](https://www.ruby-lang.org/en/){:target="_blank" rel="noopener"} is a open source programming language popular with web applications.
**_You do not need to know anything about Ruby_**, but you do need it to run Jekyll on your system!

Jekyll requires a Ruby version 2.5.0 or greater.
Below are quick start steps, but you may want to refer to Jekyll's official [installation guides](https://jekyllrb.com/docs/installation/) for tips.

- **Windows:** Use [RubyInstaller for Windows](https://rubyinstaller.org/){:target="_blank" rel="noopener"}.
    - First, [download](https://rubyinstaller.org/downloads/) the suggested stable version "WITH DEVKIT" (as of this writing, Ruby+Devkit 3.1.x (x64)) and double click to install. Use the install defaults, but make sure "Add Ruby executables to your PATH" is checked. On the final step, ensure the box to start the MSYS2 DevKit is checked.
    - Second, the installer will open a terminal window with options to install MSYS2 DevKit components. Choose option 3, "MSYS2 and MINGW development toolchain", or simply press ENTER to install all the necessary dependencies. The installer will proceed through a bunch of steps outputting a bunch of text in the terminal window. *Eventually*, this will conclude and you should see a message with the word `success` in it. If the window doesn't close, press `Enter` again or manually close it. (The installer can be restarted by typing `ridk install` into a command prompt).
- **Mac:** OS X has a version of Ruby installed by default. Check the version with `ruby -v`. If it is > 2.5.0 you can use the system Ruby. However, a newer version can be installed using [Homebrew](https://brew.sh/) or a manager such as [rbenv](https://github.com/rbenv/rbenv). Check the official Jekyll [Mac install docs](https://jekyllrb.com/docs/installation/#macOS) for tips.
- **Linux:** Although many distros come with a system Ruby installed or a repository version, we suggest using a version manager such as [rbenv](https://github.com/rbenv/rbenv) or [RVM](http://rvm.io/). This will ensure you have an up to date Ruby version and a clean environment separated from your system Ruby. You will also need the build tools Make and GCC, on Ubuntu get them with `sudo apt install build-essential`. 

### Install Jekyll

Jekyll is a Gem, a software package installed via Ruby's management system called RubyGems (similar to Python's Pip). 
Open a terminal and type:
`gem install jekyll bundler`

This will take a minute as Gem installs all the dependencies and builds extensions. 

### Install Text Editor

When working with code you should have a good text editor.
Windows notepad does not handle UTF-8 encoding or UNIX line endings that are standard for cross platform applications. 
For basic editing, Windows [Notepad++](https://notepad-plus-plus.org/), Mac TextEdit, or Linux Gedit are sufficient.
However, a more complete code editor will be helpful for managing Jekyll projects.
The current most popular open source cross platform option is [Visual Studio Code](https://code.visualstudio.com/).
