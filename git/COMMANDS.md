INSTALLER GIT
=============
GitHub est un outil de travail en ligne permettant de mettre en commun des modifications effectuées par plusieurs personnes sur un projet donné.

GitHub pour Windows: https://windows.github.com
GitHub pour Mac : https://mac.github.com
Git pour Linux - Solaris : http://git-scm.com

CONFIGURATION DES OUTILS
========================
Configurer les informations de l'utilisateur pour tous les dépôts locaux

**git config --global user.name "[nom]"**  
...

**git config --global user.email "[adresse email]"**  
...

**git config --global http.proxy http://192.168.1.17:8080**    
...

**git config --global –unset http.proxy**  
...

CRÉER/CLONER DES DÉPÔTS
=======================
Démarrer un nouveau dépôt ou en obtenir un depuis une URL existante
 
**git init [nom-du-projet]**  
...

**git clone [url]**  
...

EFFECTUER DES CHANGEMENTS
=========================
Consulter les modifications et effectuer une opération de commit

**git status**  
...

**git add [fichier]**  
le fichier à ajouter doit être dans le répertoire
après on fait un commit (pour prendre en compte les modifications)
puis on le push (pour l'avoir sur internet)


**git reset [fichier]**  
...

**git diff**  
...

**git commit -m "[message descriptif]"**  
pour prendre en compte les modifications
...

**git commit -a -m "[message descriptif]"**  
...

GROUPER DES CHANGEMENTS
=======================
Nommer une série de commits et combiner les résultats de travaux terminés

**git branch**  
...

**git branch [nom-de-branche]**  
...

**git checkout [nom-de-branche]**  
...

**git merge [nom-de-branche]**  
...

**git branch -d [nom-de-branche]**  
...

VÉRIFIER L'HISTORIQUE DES VERSIONS
==================================
Suivre et inspecter l'évolution des fichiers du projet

**git log**  
...

**git log --follow [fichier]**  
...

**git diff [premiere-branche]...[deuxieme-branche]**  
...

**git show [commit]**  
...

DÉFAIRE DES COMMITS
===================
Corriger des erreurs et gérer l'historique des corrections

**git reset [commit]**  
...

**git reset --hard [commit]**  
...

SYNCHRONISER LES CHANGEMENTS
============================
Référencer un dépôt distant et synchroniser l'historique de versions

**git fetch [nom-de-depot]**  
...

**git merge [nom-de-depot]/[branche]**  
...

**git push [vers --> alias d'un remote] [branche locale]**  
"git push" -> envoie tout vers l'interface (dans son compte, et pas dans le projet lui-même)
ensuite ne pas oublier de faire un pull request (qui devra être accepté par un administrateur)
...

**git pull [alias d'un remote] [sur --> branche locale]**  
c'est l'inverse du push, ça envoie les fichiers mis à jour de l'interface vers l'ordi (souvent branche= master)
puis on push
...

**git remote add mon_alias https://github.com/mon_login/spid-git.git**  
c'est pour être plus à l'aise
on donne un surnom (alias) au projet
...
