[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Homework : Using Git

<!-- MATERIALS METADATA -->
<!--
  title: 'Using Git'
  type: homework
  duration: ??
  creators: Matt Brendzel
  competencies: git, html
-->

## A Note About Git Commits

For this assignment (and the one tomorrow as well), you **must** use
`git commit` rather than `git commit -m` to make your commits. Why?
When using the `-m` version, you can only write a single line of text in your
commit message. This makes it hard for your commit message to have much detail.

What kinds of details are important? Things like

-   High-level descriptions of groups of changes;

-   Explanations of why a particular change or group of changes got made;

-   References to external code, both for providiing attribution and for
    linking to relevant documentation; and, most commonly...

-   References to the issue (or issues) that your commit is addressing (a very
    important part of managing workflow).

Opening up a text editor also gives you an opportunity to make your commit
message thoughtful, rather than just `"Pushed code"`. In fact, for this
assignment and the next one, every commit message you write must have a
**subject line** that gives a high-level description of the commit, followed by
a **message body** that goes into more detail.

## Setup

The terminal's default text editor is, perhaps unsurprisingly, an editor which
runs inside the terminal -- it's called [`Vim`](http://www.vim.org/)

Vim is a tool that many serious developers use for working with text, but it
can sometimes be intimidating to a beginner. If you're interested in learning to
use Vim, there are a variety of [cheatsheets](http://vim.rtorr.com/)
available online.
However, we would recommend instead that you use **Atom** as the text editor.

To set Atom as the terminal's default editor, run the following Bash commands:

1.  `echo "export VISUAL='atom --wait'" >> ~/.bash_profile`
2.  `echo "export EDITOR='atom --wait'" >> ~/.bash_profile`
3.  `source ~/.bash_profile`

> Watch out for backticks ( ` ) when you copy and paste! They're part of the
> README's formatting code, and should not be included in the commands.

## Directions

You are going to make a simple storefront website, piece by piece, inside this
directory. As you do, you will need to make a commit (following the "Commit
Guidelines" below) after completing each step.

1.  Create a new file called `index.html`, filled with HTML boilerplate.
    Give the page a header, a 'main' section, and a footer.

    > For context, the header will show the company's logo and hold navigation.
    > The main section of `index.html` will display the company's most
    > popular product and show a link to where you can purchase one.
    > The footer will hold links to other, less well-traveled parts of the site
    > (e.g. `Warranty and Returns`).

2.  Add a heading (with the text "ExampleCompany") and a nav bar to the header.

3.  Create a new file called `about.html`, also filled with standard HTML
    boilerplate. The body should contain a header, followed by a heading with
    the text "About Us".

4.  Add an article to the body of `about.html`, with two paragraphs of text
    inside. Since this is just a mock site, fill the paragraphs with
    'lorem ipsum' text (or equivalent).

5.  Add a link with the text "< Back" to the bottom of `about.html`.
    Have this link take the user back to `index.html`.
    Then, add a link to the nav bar of `index.html` with the text 'About Us',
    and have that link direct the user to `about.html`.

6.  In the main section of `index.html`, add a box containing the name of the
    the product ('PopularProduct'), a short description (just use lorem ipsum
    for now), and a link with the text "Buy Now".

7.  Create a new file called `product-page-01.html`, and again fill it with
    HTML boilerplate. Have the "Buy Now" link from the previous step point to
    this page. Then, add a header and a 'main' section to the body.

8.  Inside the 'main' section of `product-page-01.html`, add a heading
    ('PopularProduct'), a longer description (lorem ipsum again), a form
    for placing an order, and a 'Back' link similar to the one in `about.html`.

9.  Inside the order form, add a set of checkboxes (to selectively
    include/exclude Features A, B, C, D, and E), and create labels to match up
    with each checkbox. Fill each label with the appropriate text ('Feature A',
    'Feature B', etc). Make sure that all checkboxes have the same value for
    'name', so that their results will get grouped together by the form.

10. Also inside the order form, add a drop-down menu to choose the delivery
    speed : Standard Delivery, Expedited Delivery, or Overnight Delivery.
    Then add a 'submit' button to the order form, with the text "Buy Now" inside
    of it.

You will probably need to use a reference to figure out exactly how to
implement those steps in HTML.
The [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML)
and [W3Schools](http://www.w3schools.com/html/default.asp)
are two good ones.

### Commit Guidelines

In addition to having a subject line and a commit body,
each commit message should adhere to the seven guidelines below,
which lay out some widely-accepted best practices.
A detailed analysis and discussion of these guidelines can be found [here](http://chris.beams.io/posts/git-commit/#seven-rules).

1.  Separate your subject line from your body with a blank line.

2.  Limit the subject line to 50 characters (some say 40).

3.  Capitalize the subject line.

4.  Do not end your subject line in a period.

5.  Use the imperative mood in the subject line. This means to write
    it as if you were giving someone a command, e.g. "Create a new directory"

6.  Wrap the body at 72 characters.

7.  Use the body to explain _what_ and _why_ rather than _how_.

Here's an example commit message.

```markdown
Refactor parsing function

Starting to refactor the parsing function in order to make it more DRY.

See: #112
```

That last bit (`See #112`) is a reference to an issue on the repo.
GitHub recognizes those notes, and this allows you to quickly see which commits
are tied to which issues. If a commit completely solves an issue,
you'll commonly see people write something like `Resolves #73`

## Submission

Push up your code to GitHub by typing `git push origin master`.

Then, create an issue on the `wdi-remote-r2d2` repo, with the title
"YourGitHubUsername -- Week XX Day XX". Add a link to the body of the issue that
points to your fork on Github, and a 'comfort' score, from 1 to 5, based on your
understanding of the material (where 5 is "I feel very comfortable with this
material", and 1 is "I feel very uncomfortable with this material"). Feel free
to give more context to this score if you like.

e.g. For an issue named "GA-MEB -- Week 01 Day 02"

```plaintext
link : https://www.github.com/GA-MEB/wdi-remote-r2d2/unit_01/w01d02/homework
comfort: 3

Feeling mostly ok with things. My commit messages are getting better.
```

Finally, click 'Submit new issue'.
