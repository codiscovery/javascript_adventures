# 100 façons de faire Array.join

`join(arr: Array<any>, delimiter?: string): string`

Créer une fonction `join` avec 2 paramètres :

- `arr` qui contiendra un tableau
- `delimiter` qui contiendra une chaîne de caractère

Exception(s) :

1. Comme la vraie méthode, si le `delimiter` n'est pas défini, alors le `delimiter` sera la virgule

Exemples :

| Input                        | Output    |
| ---------------------------- | --------- |
| `join(["a", "b", "c"], "-")` | `"a-b-c"` |
| `join(["a", "b", "c"], "")`  | `"abc"`   |
| `join(["a", "b", "c"], " ")` | `"a b c"` |
| `join(["a", "b", "c"])`      | `"a,b,c"` |
