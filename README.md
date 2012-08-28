Overview
--------

This is the source code for my [blog](http://blog.wuzzeb.org), built using
[hakyll](http://jaspervdj.be/hakyll/index.html).  I have tried to keep it as clean code to provide a
base for others looking for a blog in hakyll.  When I initially created this blog, I struggled with
the feed creation since the existing hakyll feed module (in version 3.3) didn't fit my needs.

Changes for your own blog
-------------------------

First, clone the repo.  Next, delete all the posts, images, static files, etc. The files you want to
keep are everything in the css folder, everything in the templates folder, and index.markdown and
posts.html from the toplevel directory.  Lastly, you will need to edit the templates and files to
use your own name and urls.

 * templates/atom.xml : update the title, author, and urls.
 * templates/atom-post.xml: update the url
 * templates/default.html: update the blog name (and perhaps the footer)

 * templates/disqus.html: Update with your disqus id and urls, or delete the template and the only
   change needed to blog.hs is to delete the line near the top which has *applyTemplateCompiler
   "templates/disqus.html"

 * index.markdown: edit to change the homepage

License
-------

The blog.hs code itself and the templates are licensed under the
[BSD3](http://www.opensource.org/licenses/BSD-3-Clause), the same license used by hakyll. The
content of the posts and images (and other content) are published under the [Creative Commons CC
BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)
