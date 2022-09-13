# 100 façons de reproduire les méthodes d'Array

Pour réussir cette aventure, vous aurez besoin de boucles et des callbacks.

Seul la méthode `Array.push()` est autorisée.

Si vous avez des soucis pour utiliser les boucles ou callbacks, vous pouvez lire la suite, sinon vous pouvez démarrer.

## Episode 0 à 9 : Boucles

Que ce soit des boucles :

- `for...of`
- `while`
- ou `for`

Vous pourrez réussir.

Toutefois, je vous invite à utiliser la boucle for. Celle-ci est versatile et existe dans tous les autres langages.

Cette boucle est souvent utilisé lorsque l’on sait où on démarre et où on finit.
Pour cela vous allez définir 3 expressions pour démarrer la boucle.

1. la condition de départ, c’est là où démarre la boucle
2. la condition de sortie, c’est là où se termine
3. l’opération à chaque fin d’itération

```js
for (let index = 0 /* 1 */; index < 5 /* 2 */; index++ /* 3 */) {
  console.log(index);
}
```

Ensuite, pour chaque itération de la boucle, le corps de la fonction sera exécuté.

Dans ce cas, la boucle affichera 10 fois la variable index qui aura les valeurs de zéro a 4 a l’intérieur de la boucle.

```bash
0
1
2
3
4
```

Dans le corps de la boucle, il y a 2 mots clés autorisés dans la boucle for qui sont très pratique.

- continue
- et break

Lorsque vous utilisez continue, vous allez ordonner à la de passer à la prochaine itération sans passer par le reste des instructions de l’iteration courante.

Si index est égale à 2, alors je passe à l’itération suivante et le console.log qui aurait dû afficher 3 ne s’effectue jamais.

```js
for (let index = 0; index < 5; index++) {
  console.log("BEFORE", index);
  if (index === 2) {
    continue;
  }
  console.log("AFTER", index);
}
```

Ce code affichera dans la console :

```bash
BEFORE 0
AFTER  0
BEFORE 1
AFTER  1
BEFORE 2
          // Missing: continue have been used
BEFORE 3
AFTER  3
BEFORE 4
AFTER  4
```

Le break, en plus de stopper le reste des instructions de l’itération courante, il va aussi terminer la boucle et en sortir.

```js
for (let index = 0; index < 5; index++) {
  console.log("BEFORE", index);
  if (index === 2) {
    break;
  }
  console.log("AFTER", index);
}
console.log("END OF LOOP");
```

Ce code affichera dans la console :

```bash
BEFORE 0
AFTER  0
BEFORE 1
AFTER  1
BEFORE 2
          // Missing: break have been used
END OF LOOP
```

A savoir que si votre boucle est dans une fonction, return aura le même effet que break, mais en plus :

- il retournera une valeur à la fonction
- il arrêtera l'exécution de la boucle ET du reste de la fonction

## Episode 5 - 9 : Callbacks

Coming soon
