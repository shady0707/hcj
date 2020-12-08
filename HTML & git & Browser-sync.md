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