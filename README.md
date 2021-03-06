# Haiku Inc. website

This repository contains the source code for the website for
[Haiku, Inc.](https://www.haiku-inc.org/about/), the non-profit
organization registered in New York that supports the development
of the Haiku operating system.

## How to test locally

This site uses Hugo to generate the site from a theme and Markdown files.

Please install Hugo either from [its website](https://gohugo.io/) or using a
package manager.

Unfortunately due to the state of the Go port in Haiku, it is unlikely that recent
versions of Hugo can be used there. But otherwise Hugo can be used on most other
operating systems.

Once Hugo is installed, run the following command within this repo:

    hugo server -D

This will run the local Hugo server and include any drafts (`-D` does this) and
usually it can be found on http://localhost:1313.

Any changes made should be picked up by the server.

## Adding new content

To add new content, simply clone the repository, make a fork, open it in your file explorer, and add pages under the "content" folder. 
The content folder is divided into several smaller folders, namely:
- about
- documents
- donate
- trademarks

You might notice that these folders reflect the drop-down menus on the live site - this makes it easier to know where to put pages.
Pages put under folders will appear as links in the drop-down menus on the live site. 

**Pages must be saved as .md (Markdown) files to work - this means that you should be using Markdown when writing new content as well.**
Markdown is relatively easy to learn, and if you've used MediaWiki syntax before, Markdown is quite similar. A syntax guide is available [here](https://www.markdownguide.org/basic-syntax/): 
If you want to start writing immediately, there is an online Markdown editor [here](https://markdown-editor.github.io/). **Note that this editor does not save anything, so ensure you have your work copied into your preferred text editor just in case.

After you have finished writing, save the file as an .md file. **Just to keep things consistent, the name of the page should be entirely lowercase, and any spaces in between the name separated by a "_".** Then select which folder you wish the page to be grouped under. 
When you're finished, commit the changes and submit a pull request to merge your changes from your personal fork of the website to the master branch.

## Adding files, such as documents and images
If you wish to add files:
- Images can be placed into the images folder at "static" > "images". 
- Documents can be placed into the docs folder at "static" > "docs". 
- Javascript files can be placed into the js folder at "static" > "js". 

**Please ensure any files you insert into the website are relevant to Haiku Inc. and that any file licenses permit re-use of the file online.**

If you wish to insert files into pages:
- Images can be added into pages by adding `<img src="/images/image.png">`, replacing `image.png` with the filename and file extension of the image you want.

