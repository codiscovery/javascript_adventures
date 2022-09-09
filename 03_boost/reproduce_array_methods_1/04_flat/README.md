# 100 façons de faire Array.flat

`flat(arr: Array<any>): Array<any>`

Créer une fonction `flat` avec 1 paramètre :

- `arr` qui contiendra un tableau

Cette fonction va aplatir le tableau en enlevant les tableaux dans le tableau

Exceptions :

1. La vraie méthode contient 1 paramètre, celui-ci ne sera pas pris en compte

Exemples :

| Input                     | Output            |
| ------------------------- | ----------------- |
| `flat(["a", "b", ["c"]])` | `["a", "b", "c"]` |
| `flat([1, 2, [3, 4]])`    | `[1, 2, 3, 4]`    |
