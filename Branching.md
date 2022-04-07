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

## Mergen von Branchen

Wenn wir nun weiter arbeiten können wir natürlich auch die Änderungen auch wieder in den main branch holen.

```bash
git checkout test-branch
# um abzubrechen einfach die commit message löschen
git merge main
git log
```

## Lokale branches vs. Remote branches

Aktuell sind all unsere Änderung noch lokal. Aber wir wollen ja auch unsere Änderungen vom branch mit anderen teilen. Das können wir mit ein `push` bewerkstelligen.

```bash
git push
# Pro-Tip: Git gibt immer sehr gut Fehlermeldungen
git push --set-upstream origin test-branch
```

Jetzt können wir uns den branch auch im Repo-Manager ansehen.
