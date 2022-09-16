# 100 façons de faire Array.reduce

`reduce(arr: Array<any>, callback: Function, initialValue: any): any`

Créer une fonction `reduce` avec 3 paramètres :

- `arr` qui contiendra un tableau
- `callback` qui contiendra une fonction callback
  - `callback(item: any, index: number, array: Array<any>): any`
  - Cette fonction callback aura 3 paramètres. Vous n'êtes pas obligé de tous les utiliser
    - `item` qui contiendra l'élément courant
    - `index` qui contiendra l'index de l'élément courant
    - `array` qui contient le tableau de départ
- `initialValue` qui contiendra la valeur initiale utilisée dans la fonction `reduce`

Cette fonction va renvoyer une valeur qui contient le résultat de chaque valeur retournée par le callback.

Exemples :

| Input                                                                                                | Output                 |
| ---------------------------------------------------------------------------------------------------- | ---------------------- |
| `reduce([1, 2, 3, 4], (prev, curr) => prev + curr, 0)`                                               | `10`                   |
| `reduce([{ x: 1 }, { x: 2 }, { x: 3 }], (prev, curr) => prev + curr.x, 0)`                           | `6`                    |
| `reduce([["a", 1], ["b", 2], ["c", 3]], (acc, curr) => { acc[curr[0]] = curr[1]; return acc; }, {})` | `{ a: 1, b: 2, c: 3 }` |
