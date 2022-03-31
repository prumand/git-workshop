# Was ist git?

git ist ein 2005 von Linus Torvalds entwickeltes dezentrale Versionskontrollsystem.

## Was heißt Versionskontrolle

Ist ein Verfahren um Änderungen nachvollziehbar zu machen. Man kann sehen was geändert wurde, von wem und wann. Außerdem kann man zu einer alten Version zurückgehen.

## Was heißt dezentral?

Man kann unabähngig von Github, Bitbucket, oder sonst einen Server seine Dateien und Projekte unter Versionskontroller zu stellen.

Also lasst uns beginnen:

```
# in irgendeineinen Folder
git init
git status
# tracken wir die README.md
git add README.md
git commit
# ohne commit message kein commit
# Tipp mit -v|--verbose sieht man die Changes
git commit -v
```
