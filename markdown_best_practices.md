# Best Practices for Writing Protocols in Markdown

**Writing/Editing by**: Tiffany Lowe-Power

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