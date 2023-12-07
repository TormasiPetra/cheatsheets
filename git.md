Verziókövetés: 

git init // létrehozza a verziókövetést 
git status // megnézi hogy verziókövetve van-e már a mappa
ls -Force // megjeleníti a rejtett mappákat is 
cd .git

    a változások ebbe a git mappába kerülnek bele nagyon hatékonyan 

git log // kiírja  commitokat és hogy hány eddigi verzió van 
git add . // ez csinál egy verziót (snapshotot)
git commit -m "initial commit" 

    egy régebbi verzióra is vissza lehet állni 

git checkout `commit hash` (a git log-al lehet előhozni ,verziószám) // visszaállítja a verziót, vagy branchek között váltunk 

git switch - // visszaállítja a verziót, amiről visszamentünk 

git branch -M main // átállítja a master branch nevét main-re (Black lifes matter miatt)
     így lehet átírni: git config --global init.defaultBranch main


git remote -v // kiloggolja hogy van e remote repository

git remote add origin https://github.com/TormasiPetra/cheatsheets.git // azt az URL-t a githubról lehet kinyerni, repo létrehozás után 

git push // felpussolja a verziót 
git push --set-upstream origin master // a legelső pushnál kell, megmondja hogy a neve ugyanaz legyen 

Sorban: 
    git add . 
    git commit -m "commit"
    git push

Clone repository: 
    git clone https://github.com/pavaberna/cheatsheets.git BerniCheatSheets

git pull // leszedi a módosításokat 


git ignore // megadjuk, hogy milyem file.okat nem akarunk verziókövetni
    pl.: node modules belemehet
    
rm -rf .git // minden eddigi git log-ot töröl