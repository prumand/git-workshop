# Was ist ein branch?

Git speichert einen Snapshot der Daten. Wird ein commit gemacht, speichern wir die Info wer, wann etwas commited hat mit einer message und einem Pointer auf den jeweiligen Snapshot.
Wenn wir einen Branch erstellen, fügen wir ganz einfach einen neuen Pointer hinzu.

```bash
git log
git branch test-branch
git checkout test-branch
# bzw. weil man oft gleich in den branch wechset
git checkout -b test-branch # wenn es den noch nicht gibt
git log
```

Der neue branch ist jetzt genau auf dem selben Stand commit wie der master branch. Allerdings bleiben jetzt alle Änderungen in dem jeweiligen branch.

```bash
echo "Neue Infos für Branching" >> ./Branching.md
git commit -m "Neue Infos"
# zwischen den Branchen switchen
gco -
```
