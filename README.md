![an image with 5 steps of making own repository](./publiczne-repozytorium-ze-sforkowanego-5-krokow-v1.png)

&nbsp;

Oto prosty sposób, jak utworzyć repozytorium z własnym projektem na podstawie wcześniej sforkowanego repo (np. prywatnego repo z zadaniem).

&nbsp;

## 1. Utwórz nowe repozytorium na GitHubie.
Będzie to repozytorium dla Twojego projektu: [github.com/new](https://github.com/new). W dalszych instrukcjach znajdziesz je pod nazwą `<your-new-repo>`.

&nbsp;

## 2. Stwórz lokalną kopię swojego nowego repozytorium.
```
git clone https://github.com/<username>/<your-new-repo>.git
```
Po uruchomieniu komendy prawdopodobnie zobaczysz ostrzeżenie, że sklonowałeś puste repozytorium. Zgadza się, repo jest puste, więc nie ma się czym martwić.

&nbsp;

## 3. Przejdź do katalogu swojego lokalnego repozytorium i oznacz oryginalne repozytorium (sforkowane) jako źródłowe.
```
cd <your-new-repo>
git remote add upstream https://github.com/<username>/<your-fork-of-original-repo>.git
```
Po tej komendzie nie zobaczysz w konsoli żandej informacji zwrotnej. Możesz spokojnie przejść do kolejnego kroku.

&nbsp;

## 4. "Ściągnij" wszystkie pliki i historię zmian z oryginalnego (sforkowanego) repozytorim.
```
git pull upstream master
```
lub
```
git pull upstream main
```
Nazwę gałęzi (`main` lub `master`) znajdziesz w repozytorium ze sforkowanym projektem zaraz nad listą plików. Jest ona taka sama jak w oryginalnym repozytorium, które forkowałeś.

&nbsp;

## 5. Pushuj zawartość oryginalnego (sforkowanego) repozytorium do Twojego nowego repo na GitHubie.
```
git push origin master
```
lub
```
git push origin main
```

GitHub przy tworzeniu nowych repozytoriów nie stosuje już nazwy `master`, więc jeśli nie zmieniałeś gałęzi lub nie korzystasz z jakiegoś swojego starego repozytorium, to użyj drugiej komendu z nazwą `main`.
Jeśli chcesz upewnić się co do nazwy gałęzi, na której się znajdujesz, możesz użyć komendy `git branch --show-current`.

&nbsp;

✨ **Gotowe!** ✨
