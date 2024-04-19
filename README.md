# Setting Up Visual Studio Code (The IQSS Way)

***IMPORT PROFILE LINK***: https://vscode.dev/profile/github/2f5c3eb559798c7c449adac706742807.

With its Copilot integration and a marketplace full of extensions, we recommend using **Visual Studio Code (VSCode)** for your coding IDE. It is especially useful if you are in academia, and need to write in R[^1], Python, LaTeX, etc. 

Here we'll teach you how to download VSCode, as well as the extensions, settings, and shortcuts that we like to make this a more robust text editor. Of course, you may not have the same preferences! Once you have these downloaded, you can customize your VSCode with the extensions, settings, and shortcuts that you like. We'd love to hear feedback from you and incorporate your suggestions into our recommended profile![^2] 

## Table of Contents
1. [Instructions for Downloading VSCode](#1-instructions-for-downloading-vscode)
2. [Importing Our Recommended Profile](#2-importing-our-recommended-profile)
   
   2.1 [Extensions](#extensions)
   
   2.2 [Settings](#settings)
   
   2.3 [Keyboard Shortcuts](#keyboard-shortcuts)
   
3. [Recommended Dependencies](#3-recommended-dependencies)
4. [Customizing Your Own VSCode](#4-customizing-your-own-vscode)
   
   4.1 [Adding Your Own Extensions](#adding-your-own-extensions)

   4.2 [Adding Your Own Settings](#adding-your-own-settings)
   
   4.3 [Adding Your Own Keyboard Shortcuts](#adding-your-own-keyboard-shortcuts)
   
5. [Managing Profiles](#5-managing-profiles)

   5.1 [Creating Your Own Profile](#creating-your-own-profile)

   5.2 [Exporting Your Own Profile](#exporting-your-own-profile)

   5.3 [Deleting Profiles](#deleting-profiles)

## 1. Instructions for Downloading VSCode:
Visual Studio Code has [instructions](https://code.visualstudio.com/learn/get-started/basics) for getting started.

You can download VSCode directly from their [website](https://code.visualstudio.com/download) for your operating system.

Unzip the download (mine was called "VSCode-darwin-universal.zip"), and then click on the new application (Visual Studio Code). A pop-up will ask you if you want to open an app downloaded from the internet. Click open.

Congrats, you've downloaded VSCode!

## 2. Importing Our Recommended Profile
* Inside VSCode, click on the settings icon in the bottom-left corner (it looks like a gear!)
* Select "Profiles (*Name of your current profile*)" &#8592; this should be "Profiles (Default)" if you are doing this for the first time
* Select "Import Profile"
* Copy and paste the following URL into the search bar pop-up that says "Provide Profile Template URL": https://vscode.dev/profile/github/2f5c3eb559798c7c449adac706742807.
  * If you were to follow this link in a browser, it would bring you to VSCode's Preview in a browser. More information about their browser version [here](https://code.visualstudio.com/blogs/2021/10/20/vscode-dev).
* A pane on the left will pop up. Leave everything checked off, and select the blue "Create Profile" button
* Enter a name for this profile in the text pop-up, such as "IQSS Recs"
* Leave everything checked off, and select the blue "Create" button

Now the settings icon should have a short descriptor bubble attached, e.g. "IQ", and if you click on it, you should see that it now says "Profiles (*Profile Name*)", such as "Profiles (IQSS Rec)"

Congrats, you've imported our recommended profile!

This includes:
* **extensions**, which will automatically install for you. You can access these by clicking the extensions icon on the left-hand toolbar, which has three squares in an L shape with an additional square that is separated at the top right corner.
* **settings.json**, which you can access by clicking the settings icon, selecting Settings, and then clicking the "Open Setting (JSON)" icon in the file toolbar, which looks like a piece of paper with a curved arrow.
* **keybindings.json**, which you can access by clicking the settings icon, selecting Keyboard Shortcuts, and then clicking the "Open Keyboard Shortcuts (JSON)" icon in the file toolbar, which looks like a piece of paper with a curved arrow.

### Extensions:
* **Azure Repos**:
  * Dependency for GitHub extensions.
* **Better Comments**:
  * Color codes types of comments with symbols at the beginning of each. For example, there are:
    * "*" for highlighting a comment (green)
    * "!" for an alert (red)
    * "?" for a question (blue)
    * "TODO" for a to-do (orange)
    * "//" for a strikethrough
  * You can also customize your own.
* **GitHub Copilot**:
  * In-line suggestions: Copilot will anticipate what you are about to type. You can accept these suggestions, or keep typing.
* **GitHub Copilot Chat**:
  * In-line chat: You can use Cmd+I to start an inline chat, where you can ask Copilot to do something for you. One of my favorites is to ask Copilot "Can you write me the outline of a LaTeX document?"
  * Side chat: You can open up a side-pane for a continuous chat with Copilot, much like Chat-GPT. You can ask Copilot to explain things to you, or to make suggestions.
* **GitHub Pull Requests and Issues**:
  * Allows for a smoother integration of GitHub into VSCode.
* **GitHub Repositories**:
  * Another extension which helps to integrate your repositories into VSCode.
* **indent-rainbow**:
  * Highlights vertically along indents, allowing you to see the different levels of structure in your code.
* **LaTeX Utilities**:
  * Extension pack for LaTeX Workshop. Includes quicker paste options, live snippets, and word count.
* **LaTeX Workshop**:
  * Includes many features, including snippets, shortcuts, and pdf-viewing.
* **Live Preview**:
  * Allows you to see HTML previews inside VSCode.
* **LTeX - LanguageTool grammar/spell checking**:
  * Underlines potential spelling and grammar mistakes.
* **Path Autocomplete**:
  * Autocompletes paths for files inside your repository.
* **R**:
  * Allows you to use R in VSCode, with snippets and various viewer options.
* **R Debugger**:
  * Integrates the debugging process for R into VSCode.
* **Rainbow CSV**:
  * If you view a CSV file inside VSCode, each variable will be color-coded (for easier viewing)
* **Remote Repositories**:
  * Dependency for GitHub extensions.
* **Settings Cycler**:
  * Necessary for using special keyboard shortcuts to toggle settings on/off.
* **Toggle**:
  * Necessary for using special keyboard shortcuts to toggle settings on/off.
* **vscode-icons**:
  * Includes additional graphic icons for file types, etc., inside VSCode.
* **Word Count**:
  * Provides additional word count support for markdown documents.
* **Zotero LaTeX**:
  * Allows for more smooth integration for Zotero in LaTeX documents.
 
### Settings
We've added quite a few non-default settings, which will be automatically configured with this profile. Again, you might not like all of these — feel free to remove these from your settings.json file. Here is a list of some of these settings:
* Additional LaTeX recipes:
  * xelatex+ and pdflatex+ will actually build the accompanying files many times underneath the hood in order to make sure that your bibliography citations correspond correctly.
* LaTeX outline view will include the sections: part, chapter, section, subsection, subsubsection, and paragraph.
* Word wrapping

### Keyboard Shortcuts
We've also added a few keyboard shortcuts. You can remove these from your keybindings.json file if you do not like them. 
* "Option+Command+y": Will show you all of your built-in LaTeX recipes.
* "Shift+Option+b": When you are inside a .tex file, this will open the accompanying output PDF in an external viewer. We recommend using Skim, which you can set up with sync so that it will refresh whenever you save/build the .tex file.
* "Option+Command+f": When you are typing, this will toggle on/off whether inline suggestons will appear. Once you toggle on/off, you need to continue typing to see the change take effect.
* "Option+Command+h": When you have text highlighted, this will toggle on/off whether repeat occurrences of that word will also be highlighted.
* "Option+Command+q": When you are typing, this will toggle on/off whether dropdown spelling suggestions will appear. 

## 3. Recommended Dependencies
* GitHub:
  * We recommend using GitHub. If you do not already have a GitHub account, we recommend following the [instructions from GitHub](https://docs.github.com/en/get-started).
* Copilot:
  * One of the main benefits of VSCode is its integration with GitHub Copilot, an AI pair programmer which helps you to more effectively and quickly write code.
  * Please use [these instructions](https://docs.github.com/en/copilot/quickstart) for setting up your GitHub Copilot account.
* Skim:
  * Skim is a PDF viewer, which you can [download from the internet](https://skim-app.sourceforge.io/). We recommend setting this as your default PDF viewer.
  * Once Skim is open, go to the top toolbar menu. Select Skim > Settings.
  * In the settings pane that opens, click Sync on the top right.
  * Check off the boxes for "Check for file changes" and "Reload automatically"
  * In the PDF-TeX Sync support section, set the "Preset" to Visual Studio Code
* MikTex:
  * MikTex is a TeX distribution which you can [download from the internet](https://miktex.org/download).
  * If you already have a TeX distribution installed on your computer, you do not need to install MiKTeX as well.
* Pandoc:
  * Pandoc allows you to knit .Rmd files to PDF files. You can [install the latest release from the internet](https://pandoc.org/installing.html).

## 4. Customizing Your Own VSCode

### Adding Your Own Extensions

Adding your own extensions is easy. Simply locate the extensions icon on the left-hand toolbar (it looks like three squares in an L, with one separated square to the top right). You can search for any extension available! When you've found an extension that you like, all you need to do is click the "Install" button!

### Adding Your Own Settings

You may want different default settings. Click the settings icon in the bottom-right, and click Settings. This will open up all of your VSCode settings available. Search for what you want to do. Most settings have dropdowns or checkboxes. Simply select whichever options you like. (Underneath the hood, VSCode will also write these to your settings.json file, which you can see by clicking the Open File icon (paper with an arrow) on the top right toolbar.)

### Adding Your Own Keyboard Shortcuts

You can also add your own keyboard shortcuts by clicking the settings icon, selecting Keyboard Shortcuts and then searching for the command which you'd like to add. Then, click the pencil icon to the left of the command, and then enter in the keys you'd like to use for your shortcut.

You should then be able to see these in the Keyboard Shortcuts menu or if you click the Open File icon (paper with an arrow) in the top right of the toolbar, you can see your customized keyboard shortcuts.

## 5. Managing Profiles

Profiles allow you to build custom configurations in VSCode! You can set up multiple profiles, and you can customize each one.

### Creating Your Own Profile
* Click the settings menu
* Click Profiles
* Click Create Profile
* Give it a name, click enter

### Exporting Your Own Profile

Once you have made your own personalized settings, you can export your own profile to share with others.
* Click the settings menu
* Click Profiles
* Click Export Profile
* Click the blue "Export" button
* Give it a name, click enter
* Select the GitHub gist option
* Copy the link to share!

### Deleting Profiles
* Click the settings menu
* Click Profiles
* Click Delete Profile
* Check off the profiles that you would like to delete
* Click OK

## Contact Us:
This is a work in progress! If you like to use VSCode for other languages (Python, etc.), let us know which extensions and settings you like! If you have additional extensions, settings, or keybindings you'd like to share, please do so!

You can use the "Issues" section in this repository to add feedback.

[^1]: My personal opinion: RStudio also has Copilot integration now, so that is still a great alternative if you are just writing .R or .Rmd files. Some may even prefer it! I suggest taking a look at Matt Blackwell's instructions for [Getting Started with R, R Studio, Git, and GitHub](https://gov51.mattblackwell.org/assignments/00-r-intro/), as well as Posit's [R Studio User Guide for GitHub Copilot](https://docs.posit.co/ide/user/ide/guide/tools/copilot.html).
[^2]: See the "Contact Us" section above. Please use the "Issues" section in this repository to add feedback.
