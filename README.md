practicasGit
============

practicasGit como su nombre indica son diversas practicas para llegar a dominar git ;-)



Comienzo por crear un repositorio aqui en github. En local tengo [git estandar](http://git-scm.com/) (no la [aplicacion de github](http://windows.github.com/)).



-primer clone
	$ git clone https://github.com/fmanaya/practicasGit
	
	
	fmanaya@FMANAYAW7 /d/DEV/gitest
	$ git clone https://github.com/fmanaya/practicasGit
	Cloning into 'practicasGit'...
	remote: Counting objects: 9, done.
	remote: Compressing objects: 100% (6/6), done.
	remote: Total 9 (delta 1), reused 3 (delta 0)
	Unpacking objects: 100% (9/9), done.

-Estado
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
	
-Ver que ramas (branch) tengo en local
	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git branch
	* master

-Modifico Readme.md, comit y subo al repo central
	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
	$ git commit -a -m 'Primer commit, completo guia'
	[master b5ae7b7] Primer commit, completo guia
	 1 file changed, 22 insertions(+), 1 deletion(-)

	fmanaya@FMANAYAW7 /d/DEV/gitest/practicasGit (master)
$


