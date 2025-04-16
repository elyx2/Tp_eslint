## 3) Intégration avec Git Hooks (Husky) :
2. Ajoutez un hook pre-commit pour lancer ESLint :
En exécutant la commande suivante :

bash
Copier
npx husky add .husky/pre-commit "npx eslint ."
Cela génère l'erreur suivante : husky - add command is DEPRECATED.

Pour résoudre ce problème, nous avons modifié la commande comme suit :

bash
Copier
echo "npx eslint ." > .husky/pre-commit
Grâce à cette modification, nous avons pu effectuer des commits avec ESLint lancé avant chaque commit.