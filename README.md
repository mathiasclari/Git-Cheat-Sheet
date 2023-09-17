# Git Kratka Navodila 📜

Dobrodošli v svetu Gita, zmogljivega sistema za nadzor različic, ki ohranja vaš projekt urejen in sodelovanje nemoteno. Spodaj je profesionalen Git vodič za hitro navigacijo po Gitu, vključno z možnostjo `git commit --amend` in nekaterimi primeri dobrih sporočil za commit.

## Začetek 🚀

1. **Namestite Git** 📦
   - Prenesite in namestite Git s [git-scm.com](https://git-scm.com/downloads).

2. **Nastavite svojo identiteto** 👤
   - Nastavite svoje ime: `git config --global user.name "Vaše ime"`
   - Nastavite svoj e-poštni naslov: `git config --global user.email "vašepošta@primer.com"`

## Osnove Gita 📚

3. **Inicializirajte repozitorij** 🚀
   - Ustvarite nov Git repozitorij: `git init`

4. **Klonirajte repozitorij** 🧬
   - Klonirajte obstoječi repozitorij: `git clone <URL-repozitorija>`

5. **Preverite stanje** 🧐
   - Preglejte stanje vašega delovnega imenika: `git status`

6. **Dodajte datoteke** ➕
   - Dodajte spremembe za commit: `git add <ime-datoteke>` ali `git add .` (za vse spremembe)

7. **Commit spremembe** 💬
   - Izvedite commit z deskriptivnim sporočilom: `git commit -m "Vaše sporočilo za commit"`

   Primeri sporočil za commit:
   - `novo: Dodaj funkcionalnost registracije uporabnika`
   - `popravek: Odpravite težavo z vpisno stranjo`
   - `vzdrževanje: Posodobite odvisnosti`
   - `dokumentacija: Izboljšajte dokumentacijo API-ja`
   - `slog: Oblikujte kodo v skladu s slogovnim vodnikom`
   - `preureditev: Preorganizirajte strukturo projekta`
   - `test: Dodajte enote za preverjanje pristnosti`

8. **Popravite commite z Vim ✍️**
   - Uredi zadnje sporočilo za commit in spremembe interaktivno:

     ```bash
     git commit --amend
     ```

     Ta ukaz odpre besedilni urejevalnik Vim in vam omogoča, da uredite sporočilo za commit. Tukaj je, kako uporabiti Vim:

     - Pritisnite `i`, da vstopite v način vstavljanja. Zdaj lahko urejate besedilo.
     - Uporabite puščice, da se premikate na del sporočila za commit, ki ga želite urediti.
     - Ko končate urejanje, pritisnite `Esc`, da izstopite iz načina vstavljanja.

     Da shranite spremembe:
     - Vtipkajte `:w` in pritisnite `Enter`. S tem poveste Vimu, naj shrani (zapise) spremembe.
     - Za izhod iz Vima:
       - Vtipkajte `:q` in pritisnite `Enter`, če niste naredili nobenih sprememb, ki bi jih želeli shraniti.
       - Vtipkajte `:wq` in pritisnite `Enter`, da shranite in izstopite iz Vima, če ste naredili spremembe.

     Upoštevajte, da ima Vim krivuljo učenja, vendar je močno besedilno orodje, ko se ga enkrat naučite.

## Veje in združevanje 🌿

9. **Ustvarite novo vejo 🌱**
   - Začnite novo vejo: `git branch <ime-veje>`
   - Preklopite na vejo: `git checkout <ime-veje>`

10. **Združite veje 🤝**
    - Združite vejo v trenutno vejo: `git merge <ime-veje>`

11. **Izbrišite vejo ❌**
    - Izbrišite vejo (lokalno): `git branch -d <ime-veje>`
    - Izbrišite vejo (oddaljeno): `git push origin --delete <ime-veje>`

## Zgodovina in popravki 🕰️

12. **Preglejte zgodovino commitov 📜**
    - Preglejte zgodovino commitov: `git log`

13. **Potovanje v preteklost ⏳**
    - Preglejte določen commit: `git checkout <SHA-commita>`

## Sodelovanje 🤝

14. **Oddaljeni repozitoriji 🌐**
    - Dodajte oddaljeni repozitorij: `git remote add origin <URL-repozitorija>`

15. **Potegnite zahteve 🙏**
    - Ustvarite in pregledujte zahteve za poteg na platformah, kot so GitHub ali GitLab.

16. **Reševanje konfliktov 🔥**
    - Naslovite konflikte združevanja sodelovalno.

## Popravljanje napak 🙈

17. **Ponastavite commit 🔄**
    - Razveljavite lokalne spremembe: `git reset HEAD~1`

18. **Povrnite spremembe ↩️**
    - Ustvarite nov commit za razveljavitev prejšnjih sprememb: `git revert <SHA-commita>`

19. **Shranite spremembe 📦**
    - Začasno shranite spremembe za kasnejšo uporabo: `git stash`

## Nasveti in triki 🎩

20. **Psevdonimi 🐇**
    - Nastavite bližnjice za ukaze: `git config --global alias.<ime-psevdonima> "<git-ukaz>"`

21. **Interaktivno ponovno osnovanje 🧩**
    - Interaktivno prerazporedite, združite in uredite commitse: `git rebase -i <osnovna-veja>`

22. **.gitignore 🙅**
    - Ustvarite datoteko .gitignore, da določite datoteke in mape, ki jih Git ignorira.

Ostanite organizirani, učinkovito sodelujte in izkoristite vse zmožnosti Gita v vaših projektih. Git je močno orodje, ko ga obvladate. Veselo kodiranje! 🚀👩‍💻👨‍💻
