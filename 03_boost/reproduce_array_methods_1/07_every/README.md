# 100 façons de faire Array.every

`every(arr: Array<any>, callback: Function): boolean`

Créer une fonction `every` avec 2 paramètres :

- `arr` qui contiendra un tableau
- `callback` qui contiendra une fonction callback
  - `callback(item: any, index: number, array: Array<any>): boolean`
  - Cette fonction callback aura 3 paramètres. Vous n'êtes pas obligé de tous les utiliser
    - `item` qui contiendra l'élément courant
    - `index` qui contiendra l'index de l'élément courant
    - `array` qui contient le tableau de départ

Cette fonction va renvoyer :

- `true` si chaque élément du tableau valide le callback
- `false` si au moins un élément du tableau ne valide pas le callback

Exemples :

| Input                                    | Output  |
| ---------------------------------------- | ------- |
| `every([1, 2, 100, 3], (c) => c < 10)`   | `false` |
| `every([1, 2, 100, 3], (c) => c > 0)`    | `true`  |
| `every([1, 2, 100, 3], (c) => c < 1000)` | `true`  |
