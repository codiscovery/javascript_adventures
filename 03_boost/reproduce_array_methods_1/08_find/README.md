# 100 façons de faire Array.find

`find(arr: Array<any>, callback: Function): any`

Créer une fonction `map` avec 2 paramètres :

- `arr` qui contiendra un tableau
- `callback` qui contiendra une fonction callback
  - `callback(item: any, index: number, array: Array<any>): boolean`
  - Cette fonction callback aura 3 paramètres. Vous n'êtes pas obligé de tous les utiliser
    - `item` qui contiendra l'élément courant
    - `index` qui contiendra l'index de l'élément courant
    - `array` qui contient le tableau de départ

Cette fonction va renvoyer le premier élément qui valide la condition retournée par le callback.
Si l'élément n'est pas trouvée, la fonction renverra `undefined`

Exemples :

| Input                                         | Output      |
| --------------------------------------------- | ----------- |
| `find([14, 38, 2, 100, 1, 3], (c) => c < 10)` | `2`         |
| `find([2, 100, 1, 3], (c) => c < 0)`          | `undefined` |
