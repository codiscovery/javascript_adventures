# 100 façons de faire Array.filter

`filter(arr: Array<any>, callback: Function): Array<any>`

Créer une fonction `filter` avec 2 paramètres :

- `arr` qui contiendra un tableau
- `callback` qui contiendra une fonction callback.
  - `callback(item: any, index: number, array: Array<any>): boolean`
  - Cette fonction callback aura 3 paramètres
    - `item` qui contiendra l'élément courant
    - `index` qui contiendra l'index de l'élément courant
    - `array` qui contient le tableau de départ

Cette fonction va filtrer tous les éléments qui ne valide pas la condition du callback.
La fonction `filter` devra créer un nouveau tableau

Exemples :

| Input                                                                                                               | Output                                                        |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| `filter([1, 14, 38, 2, 100, 44, 3, 12], (c) => c < 10)`                                                             | `[1, 2, 3]`                                                   |
| `filter([{ name: "Cody", age: 18 }, { name: "Colette", age: 32 }, { name: "Connor", age: 44 }], (c) => c.age > 30)` | `[{ name: "Colette", age: 32 }, { name: "Connor", age: 44 }]` |
