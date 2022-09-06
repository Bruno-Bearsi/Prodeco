# Soluções para o [exercício 1028](../../problemas/beecrowd/1028.md) em python

## Código 1

---

- Definição da função para cálculo do MDC

```python
def gcd(a,b):
    while b != 0:
        t = b
        b = a%b
        a = t
    return a
```

- Laço de repetição para os casos de teste

```python
for i in range(int(input())):
```

- Processamento das entradas e impressão da chamada da função

```python
a,b = map(int,input().split())
print(gcd(a,b))
```

- Código Completo

```python
def gcd(a,b):
    while b != 0:
        t = b
        b = a%b
        a = t
    return a

for i in range(int(input())):
    a,b = map(int,input().split())
    print(gcd(a,b))
```

---