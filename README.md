
rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing
$ git init
Initialized empty Git repository in C:/Users/rzamo/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing/.git/

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (master)
$ git checkout -b development
Switched to a new branch 'development'

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (development)
$ git add index
fatal: pathspec 'index' did not match any files

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (development)
$ git add git_landing
fatal: pathspec 'git_landing' did not match any files


rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (development)
$ ls
assets/  index.html.html

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (development)
$ git add index.html.html
warning: in the working copy of 'index.html.html', LF will be replaced by CRLF the next time Git touches it

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (development)
$ git commit -m "Agrego link en imagen"
[development (root-commit) 75e9d23] Agrego link en imagen
 1 file changed, 22 insertions(+)
 create mode 100644 index.html.html

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (development)
$ git checkout -b rama2
Switched to a new branch 'rama2'

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git add index.html
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ ^C

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git commit -m "Agrega link para ir directo a registrarse"
[rama2 db6d2b8] Agrega link para ir directo a registrarse
 1 file changed, 36 insertions(+)
 create mode 100644 index.html

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git checkout master
error: pathspec 'master' did not match any file(s) known to git

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ cat index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Desafío Branching</title>
  <link rel="stylesheet" href="assets/css/style.css">
  <link href="https://fonts.googleapis.com/css?family=Open+Sans|Space+Mono" rel="stylesheet">
</head>
<body>
  <header>

  </header>
  <main>
  <div class="container">
    <h1>Ir a Github</h1>
    <a href="https://github.com/">
      <img src="https://assets-cdn.github.com/images/modules/logos_page/Octocat.png" alt="octocat">
    </a>
    <button type="button" class="btn">
      <a href="https://github.com/" target="_blank">Click aquí para ir a GitHub!</a>
    </button>
  </div>
<section>
  <img src="assets/img/fc7615747bc3cda4372b3fc28f306b53.jpg">
  <button type="button" class="btn">
    <a href="https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home" target="_blank">Click aquí para ir directo a registrarte!</a>
  </button>


</section>
</main>

</body>
</html>
rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git status
On branch rama2
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    index.html.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        assets/

no changes added to commit (use "git add" and/or "git commit -a")

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git add .
warning: in the working copy of 'assets/css/style.css', LF will be replaced by CRLF the next time Git touches it

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git commit -m "Se sube el proyecto"
[rama2 3768618] Se sube el proyecto
 3 files changed, 59 insertions(+), 22 deletions(-)
 create mode 100644 assets/css/style.css
 create mode 100644 assets/img/fc7615747bc3cda4372b3fc28f306b53.jpg
 delete mode 100644 index.html.html

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git config --global user email c.cvdoleyton@gmail.com
error: key does not contain a section: user

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git config --global user.email c.cvdoleyton@gmail.com

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git config --global user.name catalinacevedo13

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git checkout master
error: pathspec 'master' did not match any file(s) known to git

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git config --global user.email c.cvdoleyton@gmail.com

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (rama2)
$ git branch -M main

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (main)
$ git remote add origin https://github.com/catalinacevedo13/git_landing.git     
rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (main)
$ git push -u origin main
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 8 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (13/13), 7.89 KiB | 7.89 MiB/s, done.
Total 13 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/catalinacevedo13/git_landing.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

rzamo@Raimundo MINGW64 ~/Downloads/Apoyo Desafío evaluado - Branching (2)/git_landing (main)
$
