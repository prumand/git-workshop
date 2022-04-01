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

# Was ist dann GitHub, GitLab, Bitbucket?

Will man mit mehreren Leuten arbeiten, könnte man sich einfach einen Server mit ssh Zugang aufsetzen. Dann kann jeder mit Zugang Änderungen pushen, bzw. pullen.

Github, GitLab und Bitbucket sind Repomanager die das Anlegen, die Rechteverwaltung, Kommunikation, ... zusätzlich anbieten. Wenn man von einem Repomanager pull kriegt man aber ein einfaches git-repo, wie man das local angelegt hat.
Wir legen mal ein Bitbucket repo an und pushen unser lokales Repo dorthin (open bitbucket)

```
# git@github != git protocol
git remote add origin git@github.com:prumand/testing.git
git push -u origin main
```

# Was wollt ihr noch hören?

1. [Grundkonzepte git: Workspace, Stage, Head, Commit, History, Remote](./Grundkonzepte.md)
1. Branching: local Branches, PRs, pull und "Bitte nicht branchen!!!"
1. Automatisierung: Lokal, Zentral, basierend auf Git-Events, vs. Repomanager-Events
1. Rewrite History: Aktuelle commits bearbeiten, force pushes und git rebase
