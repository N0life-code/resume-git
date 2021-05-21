# Index collaboratif des commandes `git`



## Revenir à la liste des commandes

Pour revenir à la liste complète des commandes, [cliquez ici](index.html)



## Commande `git clone`


### Description

La commande `git clone` clone un référentiel dans un répertoire nouvellement créé, crée des branches de suivi à distance pour chaque branche du référentiel cloné (visible à l'aide de `git branch --remotes`), et crée et extrait une branche initiale qui est dérivée de la branche actuellement active du référentiel cloné.


### Exemples

-Cloner depuis l'amont :

```
$ git clone git: //git.kernel.org/pub/scm/.../linux.git mon-linux
$ cd mon-linux
$ faire
```

-Créer un clone local qui emprunte au répertoire courant, sans vérifier les choses :

```
$ git clone -l -s -n. ../copie
$ cd ../copy
$ git show-branch
```

-Cloner depuis l'amont en empruntant à un annuaire local existant :

```
$ git clone --reference /git/linux.git \
	git: //git.kernel.org/pub/scm/.../linux.git \
	mon-linux
$ cd mon-linux
```

-Créer un référentiel nu pour publier vos modifications auprès du public :

```
$ git clone --bare -l /home/proj/.git /pub/scm/proj.git
```

# je ne fais que passer