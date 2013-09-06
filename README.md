practicasGit
============

*practicasGit* como su nombre indica son diversas practicas para llegar a dominar git ;-)

Comienzo por crear un repositorio aqui en github. En local tengo [git estandar](http://git-scm.com/) (no la [aplicacion de github](http://windows.github.com/)).

## Primer repositorio local

**git clone https://github.com/fmanaya/practicasGit**

	fmanaya@FMANAYAW7 /d/DEV/gitest
	$ git clone https://github.com/fmanaya/practicasGit
	Cloning into 'practicasGit'...
	remote: Counting objects: 9, done.
	remote: Compressing objects: 100% (6/6), done.
	remote: Total 9 (delta 1), reused 3 (delta 0)
	Unpacking objects: 100% (9/9), done.

## Estado

**git status**

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git status
	# On branch master
	# Changes not staged for commit:
	#   (use "git add <file>..." to update what will be committed)
	#   (use "git checkout -- <file>..." to discard changes in working directory)
	#
	#       modified:   README.md
	#
	no changes added to commit (use "git add" and/or "git commit -a")
	
## Ver que ramas (branch) tengo en local

**git branch**

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git branch
	* master

## Modifico Readme.md, comit y subo al repo central

**git commit -a -m 'msg'**

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git commit -a -m 'Primer commit, completo guia'
	[master b5ae7b7] Primer commit, completo guia
	 1 file changed, 22 insertions(+), 1 deletion(-)

**git push**
	
	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git push
	warning: push.default is unset; its implicit value is changing in
	Git 2.0 from 'matching' to 'simple'. To squelch this message
	and maintain the current behavior after the default changes, use:

	  git config --global push.default matching

	To squelch this message and adopt the new behavior now, use:

	  git config --global push.default simple

	See 'git help config' and search for 'push.default' for further information.
	(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
	'current' instead of 'simple' if you sometimes use older versions of Git)

	Username for 'https://github.com': fmanaya
	Password for 'https://fmanaya@github.com':
	Counting objects: 5, done.
	Delta compression using up to 4 threads.
	Compressing objects: 100% (3/3), done.
	Writing objects: 100% (3/3), 453 bytes | 0 bytes/s, done.
	Total 3 (delta 1), reused 0 (delta 0)
	To https://github.com/fmanaya/practicasGit
	   07ee8f1..3c167fc  master -> master

## Nuevos ficheros

**git status**

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git status
	# On branch master
	# Untracked files:
	#   (use "git add <file>..." to include in what will be committed)
	#
	#       recursos.txt
	nothing added to commit but untracked files present (use "git add" to track)

**git add recursos.txt**
**git commit**
**git push**

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git add recursos.txt

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git status
	# On branch master
	# Changes to be committed:
	#   (use "git reset HEAD <file>..." to unstage)
	#
	#       new file:   recursos.txt
	#
	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git commit -a -m 'recursos'
	[master e8a89bc] recursos
	 1 file changed, 10 insertions(+)
	 create mode 100644 recursos.txt	

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git push
	warning: push.default is unset; its implicit value is changing in
	Git 2.0 from 'matching' to 'simple'. To squelch this message
	and maintain the current behavior after the default changes, use:

	  git config --global push.default matching

	To squelch this message and adopt the new behavior now, use:

	  git config --global push.default simple

	See 'git help config' and search for 'push.default' for further information.
	(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
	'current' instead of 'simple' if you sometimes use older versions of Git)

	Username for 'https://github.com': fmanaya
	Password for 'https://fmanaya@github.com':
	Counting objects: 4, done.
	Delta compression using up to 4 threads.
	Compressing objects: 100% (3/3), done.
	Writing objects: 100% (3/3), 477 bytes | 0 bytes/s, done.
	Total 3 (delta 0), reused 0 (delta 0)
	To https://github.com/fmanaya/practicasGit
	   fc1526f..e8a89bc  master -> master
	
	
	
## Actualizo local con las modificaciones en el repo remoto

**git pull**

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git pull
	remote: Counting objects: 14, done.
	remote: Compressing objects: 100% (12/12), done.
	remote: Total 12 (delta 4), reused 0 (delta 0)
	Unpacking objects: 100% (12/12), done.
	From https://github.com/fmanaya/practicasGit
	   e3e749a..bc1c7fb  master     -> origin/master
	Updating e3e749a..bc1c7fb
	Fast-forward
	 README.md | 30 ++++++++++++++++++------------
	 1 file changed, 18 insertions(+), 12 deletions(-)
