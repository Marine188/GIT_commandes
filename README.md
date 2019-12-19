# GIT_commandes

rails new -d postgresql test_git => créer une app
git init 
git add 
git commit 
puis suivre les intructions dans GITHUB :
=> git remote add origin https://github.com/projetfinalthp/test_git.git et PUSH
git log => connaitre les différents commits effectués 


git remote -v => voir à quoi on est connecté



CREER UNE BRANCHE EN LOCAL :
git branch -a
Se mettre sur la branch mère pour créer de nouvelles branch => cela crée une copie :
git checkout -b development => création d'une branch development
git push origin development

Pour pusher la branch local en remote => git push et on copie la commande : git push --set-upstream origin devise_css


Merge toujours en local, pull et push en remote













# RECAPITULATIF DES COMMANDES GITHUB
​
## BRANCHE : CREATION, FUSION & PUSH SUR GITHUB
​
1. Créer et se positionner directement sur la branche, après création 
​
`git checkout -b nom-de-la-branche`
​
​
​
2. Commiter les changements effectués dans la branche
`git add *`
`git commit -m "les changements"`
​
Tous les changements sont enregistrés sur la branche locale de l'ordinateur et l'on peut y revenir à tout moment.
​
​
​
3. Envoyer la branche crée sur Github
​
`git push origin nom-de-la-branche`
​
​
​
4. Fusionner la branche locale souhaitée à la branche locale master et push sur github
​
`git checkout master` : on se positionne sur la branche local de master 
​
`git pull origin master` : on récupère tout le travail qui a été effectué sur GitHub pour mettre la branche master à jour 
​
`git checkout  nom-de-la-branche` : tu te remets sur ta branche en vue de la fusionner 
​
`git merge master` 
--> cette commande demande à Git de fusionner master dans ta branche. L'ordre est important : c'est master qui va DANS ta branche et pas l'inverse. La branche master n'est pas modifiée pour le moment.
​
    optionnel : gestion de conflits (voir plus loin)
​
`git checkout master` : tu te remets sur master
​
​
`git merge nom-de-la-branche`: on fusionne le contenu de notre branche locale ''nom de la branche'' dans notre branche locale master``
​
`git push origin master` : maintenant que la fusion est faite, il faut mettre GitHub à jour pour que tous tes collègues aient l'info. Donc on envoie la branche à jour sur Github.
​
​
​
### BRANCHE : SE POSITIONNER, VOIR LES BRANCHES & LES DETRUIRE
​
1. Se positionner sur une branche
​
`git checkout nom-de-la-branche`
​
​
​
2. Voir la liste des branches 
​
`git branch`
​
​
3. Supprimer une branche inutile qui a été fusionné sur master
​
`git branch -d nom-de-la-branche`
