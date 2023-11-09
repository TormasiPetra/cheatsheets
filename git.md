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





