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
et j'ai ajouter --max-warnings 0
j'ai rajouter "prepare": "husky install" dans package.json

## 4) Configuration avancée d’ESLint :

2) 
✖ 3 problems (1 error, 2 warnings)
  1 error and 0 warnings potentially fixable with the `--fix` option.

  npx eslint . --fix -> pour regler le 1 error
  2:1  warning  Unexpected console statement  no-console
  4:3  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)

## 5) Mise en place de GitHub Actions

git add .
git commit -m "Ajout de GitHub Actions"
git push

  2:1  warning  Unexpected console statement  no-console
  4:3  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)

