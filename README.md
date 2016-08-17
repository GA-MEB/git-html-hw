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

## Directions

Create a new directory on your computer called `example-git-project`, and run
`git init` inside it to turn that directory into a repo.

In this directory, you are going to make a simple storefront website,
piece by piece, and you will need to make a commit (following the "Commit
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

Rule Number 1 is to not use `commit -m`; it doesn't let you give a detailed
commit message. Instead, just write `git commit` and write your message in the
text editor that pops up (e.g. Atom, Sublime Text, Vim).

Every commit message must have a **subject line** that gives a high-level
description of the commit, followed by a **message body** that goes into more
detail.

Additionally, each commit message should adhere to the seven rules
below, which lay out some widely-accepted best practices. A detailed analysis
of these rules can be found
[here](http://chris.beams.io/posts/git-commit/#seven-rules).

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
you'll commonly see people write things like `Resolves #73`

## Submission

Since you created a repo as part of this assignment, just create a new empty
repo on your GitHub account and add it as a remote repo to `example-git-project`
by typing the command `git remote add origin ...`,  where `...` is the SSH
URL that shows up on GitHub
(e.g. `git@github.com:YourGitHubUsername/example-git-project.git`).

Then, push up your code to GitHub by typing `git push origin master`.

Finally, create an issue on the `wdi-remote-...` repo, with the title
"YourGitHubUsername -- Week XX Day XX".
Add a link to the body of the issue that points to your new repo on Github,
include any other comments or notes you want, and click 'Submit new issue'.
