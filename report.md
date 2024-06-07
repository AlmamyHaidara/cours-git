# 1. Clone du depot
    git clone https://github.com/AlmamyHaidara/cours-git.git
### Permet de clone une version du repo distant

# 2. Configuration des identifiant git avec votre nom et email
    git config --global user.email almamyh27@gmail.com
    git config --global user.name almamyhaidara

### Permet de configure les identifants git comme le nom l'email et d' autre info si necessaire qui permettra a tes collegue de t'identifier sur git

# 3. Creation d'une nouvelle branch
    git checkout -b feature

### Permet de creer la branch feature et de ce deplacer sur la branch feature en garden les modification de la branch precedente

# 4. L'ajout du fichier <README.md>
    git add README.md

### Permet d'ajouter le fichier README.md sur git

# 5. Commitez vos changement
    git commit -m "commit message"
    git stash

### Permet d'envoie mes modification sur git en ajoutent un message et stash pour stocker les modification de facons temporel

# 6. Retour sur la branch main et en envoiant les modification sur le repot distant
    git stash apply
    git push origin main

### Permet d'applique les modifiation  stocker temporelement et de les pouche sur le repot distant

# 7. Mettre les modification temporel
    git stash
    git checkout feature
    git stash apply
    git commit -m "<< README >> : << Bon retour sur la branch feature >>"
    git push origin feature

### Ces commande permet de sauvegarde temporelement les modification , bascule sur une branch et commite et des push sur des une branch

# 8.La gestion de confli
    git checkout main
    git add .
    git commit -m "commit message"
    git rebase feature
    git rebase --continue
    git add .
    git commit -m "last commit"
    git push origin main
