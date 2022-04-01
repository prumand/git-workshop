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
