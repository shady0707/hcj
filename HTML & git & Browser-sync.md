# HTML & git & Browser-sync

1. commit local files to remote git:

   $ git add .     *. means everything, or substitute it with file name, this mark the files need to be committed later*

   $ git commit -m "*some notes*".     *commit files to github (remote site)*

   $ git push     *update the remote site with local site files*

   $ git status    *check the status to see if everything committed*

   $ git config --get remote.origin.url *look for the original url of this repo*
2. browser-sync 

   $browser-sync start --server --files "*"    *"\*"is the file you wanna keep updated*

   then go to localhost:3000/* ,it will keep updated while you edit.

3. pseudo-class selector:

   selector : pseudo-class {}

4. alwasy escape: <, >, &, 
   use **&lt;**, **&gt;**, **&amp;** instead

5. \<section>: a generic secion of a document, typically with a heading. An introduction, content, or contact information can be a section.  
    \<div>: no special meaning. When no other oelement is suitable, choose this one (poor accessibility).  
    \<article>: indipendent item section of content, **must have \<h1> tag as title**. Such as a blog post, newspaper article, etc. It's an independent content.  
    \<nav>: navigation links.  
    \<p>: a paragraph, automatically add a single blank line before and after each \<p> element.
    >