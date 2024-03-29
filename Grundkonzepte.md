# Grundkonzepte git
## Workspace

Wenn man etwas geänder wird will man das auch sehen (VS-Code auf der Seite ;)), oder

```bash
git status
git diff
```

Hier sieht man die Aenderungen, die man gemacht hat.

## Stage

Bevor wir etwas commiten, muessen wir die Aenderungen erst stagen, dh fuer einen Commit vormerken. Wir muessen nicht alles Files commiten.

```
git add Grundkonzepte.md
git status
git commit
# ohne commit message bricht es ab
# mit --verbose|-v sieht man im Editor alle die Aenderungen bevor
# man commited
git commit --verbose
```

## HEAD

Das ist der aktuelle Stand, des commited REPOS.

```
git diff
# ist das gleiche wie
git diff HEAD
```

## Commits & History

Jede Aenderungen generiert einen Commit und man kann sich diese auch in der History anschauen. Bzw. Unterschiede zwischen zwei Commits anschauen.

```
git log
# mit Aenderungen
git log -p
# Aenderungen eines spezifischen Commits
git diff 533e5a5
# Aenderunge mehrer Commits
git diff 533e5a5 f517144
```

# Git push, bzw. pull und fetch

Wir haben ja die Moeglichkeit auf ein neues Repos zu pushen. Was wir bei git status sehen, ist allerdings nur der letzte Stand den wir uns geholt haben. Dh wenn wir remote Aenderungen machen, sehen wir die erst im `git status`, wenn wir auch ein `git fetch` machen.
Erst wenn wir pullen, aktualisieren wir unseren HEAD.

```bash
git status
!! Kurze Aenderung im remote machen !!
git fetch
git status
git pull
git status
```
