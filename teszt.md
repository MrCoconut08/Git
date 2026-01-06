# Mi az a git és github?

## Git
A git egy elosztott verziókezelő rendszer, amelyet Linus Torvald fejlesztett 2005-ben. Lehetővé teszi:
- Kódváltozások nyomonkövetését
- Korábbi kódverziókhoz való visszatérést
- Párhuzamos fejlesztés branch-eken
- Offline munka a teljes project történelmével

## GitHub 
A GitHub egy felhőalapú platform Git repositoty-dk tárolására és kezelésére. Funkciói:
- Repositoty hosting
- Együtműködési eszközök (Issue, Pull Request)
- CI/CD Integráció (GitHub Actions)
- Projectmenedzsment (Projects, Milestones)
- Kód review és biztonság

> Összeefoglalva
**Git** - verjiókezelő eeszköz a gépeden **GitHub** - online paltform a repository-k tárolására

Miért érdemes megtanulni?
- Csapatmunka (Több fejlesztő dolgozhat ugyanazon a projekten)
- Biztonság (kód biztonságos tárolása, pl nem vész el)
- Történet (Minden változás visszakövethető)
- Visszaállítás (Bármikor visszatérhetünk a korábbi verzióhoz)
- Iparági standard (a legtöbb cég elvárja a Git ismeratét)

## Telepítés


 ### Ellenörzés

 >git --version
 >git version

 ## Git alapvető parancsok

 ### Lokális repository létrehozása

 git init

 git add .

 git commit -m ""

 git log

 git reset HEAD~1

 git status

git remote add origin https://github.com/papprichard/git.git
git branch -M main
git push -u origin main

CTRL + SHIFT + P code parancsok megnyitása
CTR + SHIFT + V markdown file előnéz

# néhány hasznolss parancs

```
    git diff
    git log --oneline
    # Utolsó commit visszavonása (lokálisan)
    git reset --soft HEAD-1
    # Utolsó commit visszaállitása változás is törlődik 
    git reset HEAD-1
    git checkout <fájlnév>
    #Változások ideiglenes félretétele
    git stash
    git stash pap
    nemtom
```

# git commit üzenetek konvenciók

```
<tipus>: <rövid leírás>
# Tipusok
feat: új funkció
fix: Hibajavítás
docs: Dokumentáció
style: Formázás (nem változik a kód)
refaktor: Refaktorálás
test: Tesztek
# példa
git commit -n "feat: adduser Autenticarion"
```

# gitingore
Ez a ***.gitignore*** fájl meghatározza a hogy  mely fájlokat ne kövesse a git?