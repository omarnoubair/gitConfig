Installer Git

Nous vous recommandons d'installer Git sur votre ordinateur en téléchargeant GitHub Desktop . 
Nous n'utiliserons pas l'application de bureau dans Git-it (uniquement le terminal!). 
Ce paquet logiciel comprend aussi Git et est la manière la plus simple d'installer Git sur les plates-formes non Linux.

Windows : Utilisez Git Shell pour votre terminal.
Mac : ouvrez GitHub Desktop et, à partir des Préférences, sélectionnez l'installation des outils de ligne de commande. 
Pour vous en servir utiliser l'application terminal .
Vous avez déjà Git ou pas sûr? 
Tapez git --version dans votre terminal et s'il renvoie un numéro de version Supérieur à 1.7.10, 
Tout est déjà installé! Pour plus d'informations, visitez le site web officiel de Git.

Configurer Git

Une fois que GitHub Desktop (et donc Git) est installé, ouvrez votre terminal . Vous pouvez vérifier que Git existe vraiment en tapant:
git --version
Cela renverra la version de Git sur votre ordinateur et ressemblera à ceci:
git version 1.9.1
Ensuite, configurez Git afin qu'il puisse vous associer votre travail :
Définissez votre nom:
git config --global user.name "Your Name"
Maintenant configurez votre courrier électronique:
git config --global user.email "youremail@example.com"
Vous avez fini avec le premier défi! Cliquez sur le bouton "Vérifier" pour vérifier le défi.


Repository

Créer un Dépôt

Vous allez créer un nouveau dossier de projet puis l'initialiser en tant que dépôt Git. 
Nommer le dossier 'hello-world' dans ce défi, vous pouvez choisir un nom différent si vous avez déjà un dossier nommé ainsi 
(c'est un nom commun en informatique).
Ouvrez votre terminal!
Dans la fenêtre de votre terminal, tapez ces commandes, une à la fois, en appuyant sur la touche "Entrée" pour valider votre saisie
Tout d'abord, créez un nouveau dossier:
Astuce: mkdir signifie make directory
mkdir hello-world
Ensuite, entrez dans ce dossier:
Astuce: cd signifie change directory
cd hello-world
Enfin, dites à Git d'initialiser(démarrer le suivi) du dossier dans lequel vous êtes:
git init
La dernière commande devrait renvoyer quelque chose commençant par "Initialized empty Git repository". 
Les autres commandes ne renvoie rien.
Vous l'avez fait! Si vous voulez être sûr que c'est un dépôt Git, 
tapez git status et s'il ne vous retourne pas 'fatal: Not a git repository...' c'est que tout est parfait !

Commit To it 

Créer un nouveau fichier
Maintenant que vous avez un référentiel commencé, ajoutez-y un fichier.
Ouvrez votre éditeur de texte et créez un nouveau fichier vide. 
Maintenant, écrivez un peu de texte, tapez peut-être "Bonjour!", 
et enregistrez le fichier sous «readme.txt» dans le dossier «hello-world» que vous avez créé lors du précédent défi.

Vérifier l'état + ajouter et soumettre les modifications

Ensuite, vérifiez le statut de votre dépôt pour savoir s'il y a eu des changements. 
Vous savez que vous avez changé quelque chose , mais Git le sait-il aussi ?
Assurez-vous que vous êtes toujours dans votre répertoire «hello-world» lorsque vous exécutez ces commandes. 
Utilisez maintenant Git pour voir ce qui a changé dans votre dépôt:
Tout d'abord, vérifiez le statut:
git status
Git devrait vous dire qu'un fichier a été ajouté.
Puis ajouter le fichier que vous venez de créer afin qu'il devienne une partie des modifications que vous soumettez avec Git:
git add readme.txt
Enfin, soumettez (commit) ces modifications à l'historique du dépôt avec un court (m) message décrivant les mises à jour.
git commit -m "Création du fichier readme"

Étape: Effectuez plus de modifications

Ajoutez une autre ligne au fichier "readme.txt" et enregistrez le fichier à nouveau.
Dans le terminal, vous pouvez afficher les différences entre le fichier actuel et la dernière version soumise.
Dites à Git de vous afficher le diff:
git diff
Maintenant, avec ce que vous venez d'apprendre ci-dessus, soumettez ces derniers changements.