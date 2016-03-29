
# Assignment 1

Publish to GitHub by Thursday __April 7th, 11:55pm__.

It's dangerous to go alone! Take these [Git Notes].

[Git Notes]: https://github.com/2016-ucdavis-sts98/notes/blob/master/git_guide.pdf

Start early so that you can get help on Piazza and in office hours. Now is the
time to work out any problems you have with submitting assignments via git.

## Part A: About You :smiley:

If you're reading this on GitHub, clone this repository to get started. Cloning
is explained in the [Git Notes].

For this part of the assignment, you'll create a short description of yourself
and publish it to the web. The goal is to get comfortable with text editors,
git, and the command line.

1.  Get a text editor. Since we'll be using R a lot in this class, the best
    choice is [RStudio]. Some other options are [Atom], [Notepad++][]
    (Windows), and [TextWrangler][] (Mac OS X). If you want a challenge,
    [Emacs] and [Neovim] are more advanced, but much less beginner-friendly.
    Microsoft Word and other office suites are designed to edit formatted text
    files, not plain text files, so they are not a good substitute for a text
    editor.
    
[RStudio]: https://www.rstudio.com/products/rstudio/download/
[Atom]: https://atom.io/
[Notepad++]: https://notepad-plus-plus.org/
[TextWrangler]: http://www.barebones.com/products/textwrangler/
[Emacs]: https://www.gnu.org/software/emacs/
[Neovim]: https://neovim.io/

2.  Open your text editor. Create a new text document and write a 5-6 sentence
    description of yourself, which should include:

    * Your first and last name
    * Your year and major
    * What you want to learn in STS 98
    * A little about you (this can be anything you want to tell)

    While writing, keep in mind that you'll be publishing this information
    publicly online. Save the file in your assignment repository as
    `description.txt`.

    __(optional)__ Format the file with [Markdown], and save it as
    `description.md` instead.

[Markdown]: https://guides.github.com/features/mastering-markdown/

3.  Copy a clear photo of your face. Keep it appropriate and under 1 MB. Name
    the file `photo`, but keep the original extension. For example: if the
    original file is `IMG2351.jpg`, name the copy `photo.jpg`.

Now you need to publish your work.

1.  Open the command line and change the working directory to your assignment
    repository.
    
2.  Use the `git add` command to stage your description and photo. Remember,
    you can check which files you've added with the `git status` command. You
    can unstage a file with the `git reset HEAD` command.

3.  Once your files are staged, use `git commit -m` to create a commit. Write a
    one-sentence commit message that describes your work. Make sure to surround
    the commit message in quotes. For example,

        git commit -m "Wrote a totally awesome bio!"

4.  Push your commits to GitHub with the `git push` command. Git will ask you
    for your GitHub username and password. You'll need an internet connection
    for this step. 

5.  Open [GitHub](https://github.com/) in your web browser and double-check
    that your files are now online.

## Part B: Data Detective :mag:

For this part of the assignment, you'll investigate an unfamiliar R function
and a mystery data set. The goal is to take your first few steps as an R user.

Helpful R commands: `?`, `??`, `dim`, `nrow`, `ncol`, `length`, `names`,
`rownames`, `colnames`, `head`, `tail`, `typeof`, `class`, `readRDS`

1.  R includes a function called `which.max`.

    1. How many parameters does the function have? Describe each of them.
    2. What does it do?
    3. Give an example of what it does with the vector `c(3, -1, 4, 2.5)`.
    4. What happens if there's a tie? How did you figure this out?

2.  Load the data set `mystery.rds`.

    1.  What's the type of this data? What's the class?
    2.  How big is the data?
    3.  Briefly describe five of the columns.
    4.  What do you think this data represents? Explain your reasoning.
    5.  Searching the web is a good way to get more information (but always be
        skeptical). Search the web to verify your guess about what the data
        represents. Were you correct? Did you find any new information?
    6.  There are many variables this data set doesn't include. For example, it
        doesn't include each person's hair color. Suggest two variables that
        aren't included. For each variable, write a paragraph that gives a
        description and a discussion of why you think the variable is
        meaningful. It might help to imagine you're someone from 1912. What
        would you want to know?
    7.  Do you think this data set is accurate? In a paragraph, discuss how and
        why there might be inaccuracies or errors.

Save your answers to a PDF file named `partB.pdf` and your code to a text file
named `partB.R`, both in your assignment repository. Add, commit, and push the
files to GitHub following the same steps you used to publish Part A. Please do
not commit any `.docx` or `.odt` files.

Microsoft Word, [Libre Office], [RStudio][RMarkdown], and others can export to
PDF. 

[Libre Office]: https://www.libreoffice.org/
[RMarkdown]: http://rmarkdown.rstudio.com/authoring_quick_tour.html

