# node-server-ts

comment creer un server node avec ts ?

# d'abord gerer git 
-aller dans le repertoire dans lequel in veux creer le projet 
-aller sur github 
-cliquer sur "NEW"
-suivre les instruction de création de repertoire jusqu'a la fin (je veux dire jusqua la creation du repertoire git )

# quelque commandes à faire 
-npm init
-npm install typescript
-npx tsc --init


# le package json
"build": "tsc" 
    = construit le file.js correspondant
"start": "ts-node-dev --respawn src/index.ts"
    =ts-node compile une fois mais ts-node-dev le fait à chaque changement 
"dev": "nodemon --exec ts-node src/index.ts"
    = fait pareil que npm run start . Utile quand npm run start ne fonctionne pas sur ton pc


les dépendances suivante : @types/express et @types/node  permettent d'avoir accès aux modules node et express typé .
*** il peut arrivé que certain modules ne le sois pas ! Dans ce cas il faut déclarer leur type . conf :https://www.youtube.com/watch?v=1UcLoOD1lRM


# warning

le compilateur javascript peut parfois être lent . solution : ctrl+shift+p 