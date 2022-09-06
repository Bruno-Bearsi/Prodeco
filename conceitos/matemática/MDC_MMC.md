# MDC e MMC

## MDC

Produto dos divisores comuns entre dois ou mais números

### Exemplo

> 24 = 2 * 2 * 2 * 3

> 18 = 2 * 3 * 3

24 e 18 compartilham 2 * 3, logo seu mdc é 6

### Implementação

Implementação em pseudo-código

```
function gcd(a, b)
    while b ≠ 0
        t := b
        b := a mod b
        a := t
    return a
```

---

## MMC

Menor inteiro positivo que pode ser dividido por dois ou mais inteiros.

### Exemplo

| A | B | Div |
| - | - | - |
| 6 | 8 | 2 |
| 3 | 4 | 2 |
| 3 | 2 | 2 |
| 3 | 1 | 3 |
| 1 | 1 | 24 |

O MMC de 6 e 8 é 24

### Implementação

Implementação em pseudo-código utilizand o MDC entre os valores

```
function lcm(a, b)
    return a * b / gcd(a,b)
```


