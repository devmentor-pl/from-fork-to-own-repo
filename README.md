![an image with 5 steps of making own repository](./publiczne-repozytorium-ze-sforkowanego-5-krokow.png)

&nbsp;

Oto prosty sposób, jak utworzyć repozytorium z własnym projektem na podstawie wcześniej sforkowanego repo (np. prywatnego repo z zadaniem).

&nbsp;

## 1. Utwórz nowe repozytorium na GitHubie.
Będzie to repozytorium dla Twojego projektu: [github.com/new](https://github.com/new).

&nbsp;

## 2. Stwórz jego lokalną kopię.
```
git clone https://github.com/<username>/<forked-repo>.git
```
&nbsp;

## 3. Oznacz oryginalne repozytorium jako źródłowe.
```
cd <forked-repo>
git remote add upstream https://github.com/<username>/<original-repo>.git
```
&nbsp;

## 4. "Ściągnij" wszystkie pliki i historię zmian z oryginalnego (sforkowanego) repozytorim.
```
git pull upstream master
```
&nbsp;

## 5. Pushuj zawartość oryginalnego (sforkowanego) repozytorium do Twojego nowego repo na GitHubie.
```
git push origin master
```

&nbsp;

✨ **Gotowe!** ✨
