# 100 façons de faire Array.map

`map(arr: Array<any>, callback: Function): Array<any>`

Créer une fonction `map` avec 2 paramètres :

- `arr` qui contiendra un tableau
- `callback` qui contiendra une fonction callback
  - `callback(item: any, index: number, array: Array<any>): any`
  - Cette fonction callback aura 3 paramètres. Vous n'êtes pas obligé de tous les utiliser
    - `item` qui contiendra l'élément courant
    - `index` qui contiendra l'index de l'élément courant
    - `array` qui contient le tableau de départ

Cette fonction va renvoyer un nouveau tableau qui contient chaque élément renvoyé par le callback.

Exemples :

| Input                                                                                                        | Output                          |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------- |
| `map([{a: 1}, {a: 2}, {a: 3}], (c) => c.a)`                                                                  | `[1, 2, 3]`                     |
| `map([{ name: "Cody", age: 18 }, { name: "Colette", age: 32 }, { name: "Connor", age: 44 }], (c) => c.name)` | `["Cody", "Colette", "Connor"]` |
