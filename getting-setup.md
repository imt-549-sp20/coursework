# Getting setup tutorial

<iframe width="725" height="408" src="https://www.youtube.com/embed/rfK1kauUNBA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Before you get started with this course, you need to install a few tools and create a few accounts. All of these things are free and available on all major platforms (Windows, OS X, and Linux).

Most screenshots and examples will be on a Mac OS machine.

## Sign up

- [GitHub](https://github.com) - We will store all code in GitHub. There is also a [Student Developer Pack](https://education.github.com/pack) which gives you unlimited private repositories and other useful resources.

### Join the GitHut classroom

Follow the link in the [Week 1 - Managing files challenge](https://canvas.uw.edu/courses/1375712/assignments/5284439) to join the IMT 549 organization on GitHub. Once you join, it should make a copy of the initial files and put them in the location `github.com/imt-549-sp20/challanges-{your username}`. 

This is repository you will be working out of for the quarter, it will part of the GitHub classroom but only Nick and Ilesha will have access to it.

## Desktop tools

- [GitHub Desktop](https://desktop.github.com/) - This tool makes working with GIT visual.
- [Visual Studio Code](https://code.visualstudio.com/) - Code editor we will be using throughout the course.
- [Google Chrome](https://www.google.com/chrome/) - Web browser with developer tools that will allow us to inspect Web pages and javascript.

## Install GIT (optional)

If GitHub Desktop of VS Code show an error that "git cannot be found". You will have to [download git](https://git-scm.com/downloads) and install it.

On a Mac, if you get an error when trying to open the file because it could not identify the developer.

![Git error](./images/getting-setup/git-error.png)

Open System Preferences -> Security and click the "Open Anyways" button at the bottom of the window:

![System preferences](./images/getting-setup/system-preferences.png)

## Command line tools

- [Node JS and NPM](https://nodejs.org/en/download/) - These tools will help us build modern Web pages.
These tools can be downloaded from the website.

### Homebrew (optional)

If you are comfortable using the command line, [Homebrew](https://brew.sh/) (MacOS only) can be used to manage applications on your computer, the software is available to install by using the following commands:

```
# Install Homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install the desktop applications
brew cask install google-chrome
brew cask install visual-studio-code
brew cask install github

# Install Node and NPM
brew install node
```

## Troubleshooting

GIT username or email address error

If you get this error when pushing to GitHub Desktop

![Git username error](./images/getting-setup/github-auth-error.png)

[Open a Terminal](https://www.wikihow.com/Open-a-Terminal-Window-in-Mac) or [Command Prompt](https://www.digitalcitizen.life/7-ways-launch-command-prompt-windows-7-windows-8) and type the following commands. Replace `{Firstname}`, `{Lastname}`, `{Email}` with your name and email address you use to sign up for GitHub.com.

```
git config --global user.email "{Email}"
git config --global user.name "{Firstname} {Lastname}"
```

## Customizing VS Code

These extensions will help you as a developer get the most out of Visual Studio Code.

- [StyleLint](https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
- [IntelliSense for CSS class names](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
- [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek)
- [Auto close tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
- [Auto rename tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
- [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)
- [Spelling Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
- [Indenticator](https://marketplace.visualstudio.com/items?itemName=SirTori.indenticator)

## Chrome extensions

- [Web Developer Toolbar](https://chrispederick.com/work/web-developer/)
- [aXe Accessibility Tester](https://chrome.google.com/webstore/detail/axe/lhdoppojpmngadmnindnejefpokejbdd?hl=en-US)