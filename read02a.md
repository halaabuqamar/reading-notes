# learining Markdown 
## What is Markdown?
**Markdown** is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.

You can use Markdown most places around GitHub:

* Gists 1
* Comments in Issues and Pull Requests 2
* Files with the .md or .markdown extension 3
### Examples
Text Lists Images Headers & Quotes Code Extras
It's very easy to make some words**bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com)
It's very easy to make some words bold and other words italic with Markdown. You can even link to Google!

Syntax guide
Here’s an overview of Markdown syntax that you can use anywhere on GitHub.com or in your own text files.

hlighting:

def foo():
    if not bar:
        return True
Task Lists
- [x] @mentions, #refs, [links](),**formatting**, and<del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
If you include a task list in the first comment of an Issue, you will get a handy progress indicator in your issue list. It also works in Pull Requests!

*Tables*
You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
Would become:

First Header	Second Header
Content from cell 1	Content from cell 2
Content in the first column	Content in the second column
SHA references
Any reference to a commit’s SHA-1 hash will be automatically converted into a link to that commit on GitHub.

16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac
Issue references within a repository
Any number that refers to an Issue or Pull Request will be automatically converted into a link.


Strikethrough
Any word wrapped with two tildes (like ~~this~~) will appear crossed out.

Emoji
GitHub supports emoji!

*To see a list of every image we support, check out the Emoji Cheat Sheet.*