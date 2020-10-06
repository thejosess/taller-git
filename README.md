# taller-git

## 1. Conceptos básicos
       man git 
para el manual completo    

        man git-orden     
       
Para iniciar repositorio con branch principal que se llama main
    
        git init -b main

El estado de tu respositorio

        git status

Pueden ser untracked que nos los reconoce y unstanged

* Untracked: Archivos que no están añadidos al repositorio. Para ello lo añades y lo commiteas

        git add
        git commit

    Cuando haces eso para a staged, para volver a unstanged. git restore -

* Unstanged:


Para subir los cambios a ese repositorio sería con git commit -m "mensaje corto" -m "mensaje largo". 


Cuando haces varios commit se quedan varios ahi y para gestionarlos

    git log
    git whatchanged

Al hacer el log coges una cadena que pone al lado de commit, y haces

    git log id_comit


Para ver cambios al ultimo commit

    git diff    

Entre commit 
    git diff HEAD id_comit


## Local y remoto

Todo lo que trabajos ahora mismo es de forma LOCAL.

Inicias un repositorio como git init
y luego quiere subir ese repositorio a uno de github, haces 

    git remote add origin git@github:thejosess/nombre_repo_creadoEnGIthub

    git remote add <remoto> <direccion>

Y para ver remote

    git remote
    //mas info con man git-remote

Despues de hacer un remote hay que subirlo, es empujar al remoto.
Luego hay que decirle que a partir de ahora la rama será main

    git push --set-upstream origin main


