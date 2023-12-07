npm init
npm i -D typescript
npx tsc --init
tsconfig: 59. soraban kikommentel és beir :     "outDir": "./out",
tsconfig . 29.sor kikommentel és beir :         "rootDir": "./src",
package json 6. soraban a scripts alatt:        "build": "tsc" -re atir ami ott volt

git ignore fajli csinalas --> terminalba ni .gitignore  vagy vs codeban csak uj fajl .gitignore

gitignore fajlba belerak a node_modules illetve most az out mappa, mer a js fajlt se kell kovetni, mert eleg ha megvan a ts file amibol keosbb latszodik a js