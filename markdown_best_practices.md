# Best Practices for Maintaining Lab Protocols

**Writing/Editing by**: Tiffany Lowe-Power

## Philosophy

* We should have accessible, complete, and clear protocols in order to promote our own research reproducibility
* Platforms: 
    * GitHub provides a useful platform to host a (1) Table of Contents and (2) text-based protocols in markdown format
    * Google Drive can be used, if and only if (1) the files are stored in the lab "Google Drive". (2) permissions are set so anyone can read the file and the file is linked in the GitHub Table of Contents
        * If files are in a personal Google Drive linked to @ucdavis accounts, they will be deleted when you graduate / end employment. 
    * Protocols.io can be used, if and only if (1) the files are stored in the lab organization and (2) permissions are set so anyone can read the file and the file is linked in the GitHub Table of Contents

### Suggestions for maintaining protocols in GitHub

* The formatting is "Markdown", which is a simple and standard language for formatting text. You can google for Markdown guides. 


* **Use a new line for every sentence.** 
This helps with version control -- individually changed sentences will be highlighted upon commits (easy to parse) rather than whole paragraphs (nightmare to parse).
    * This formatting is incompatible with a double space after period. 
    Do a find and replace for ".  " --> ". ". 
    Be careful not to blanket remove all double spaces because tabbed bullets have 3 spaces. 

* ".md" are markdown files.

* Lab convention is to use **underscores (_)** between words and all **lowercase**. 

* Add protocol entries as links to the README.md 

* Add linked content (e.g. images, excel workbooks, etc) to sub-directories

* If you use the `Visual Studio Code` to fork, edit, and commit protocols, you can view the *source code* side-by-side with the *markdown Preview*:
![How to open the preview markdown](images/preview_markdown_screenshot.png)

* When making numbered lists, just use `1. ` for all numbers. 
Markdown will make them sequential automatically.
This is helpful if you go back & add additional entries later. 

* Use "XXX" to indicate an area that needs editing. This will allow the lab to CTRL+F for "XXX" and find areas that need editing.