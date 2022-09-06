# Soluções para o [exercício 1064](../../problemas/beecrowd/1064.md) em python

## Código 1

---

- Leitura dos 6 valores e gravação em uma lista

```python
l = []
for i in range(6):
    l.append(float(input()))
```

- Criação de uma nova lista com os valores positivos

```python
p = [i for i in l if i>0]
```

- Impressão da quantidade de positivos e sua média

```python
print("{} valores positivos".format(len(p)))
print("{0:.1f}".format(sum(p)/len(p)))
```

- Código completo

```python
l = []
for i in range(6):
    l.append(float(input()))

p = [i for i in l if i>0]

print("{} valores positivos".format(len(p)))
print("{0:.1f}".format(sum(p)/len(p)))
```

---

## Código 2

---

- Declaração de varíaveis para armazenar a quantidade de valores positivos e a soma desses valores

```python
c = 0
s = 0
```

- Leitura e processamento dos valores

```python
for i in range(6):
    aux = float(input())
    if aux>0:
        c += 1
        s += aux
```

- Impressão da quantidade de positivos e sua média

```python
print("{} valores positivos".format(c))
print("{0:.1f}".format(s/c))
```

- Código completo

```python
c = 0
s = 0

for i in range(6):
    aux = float(input())
    if aux>0:
        c += 1
        s += aux

print("{} valores positivos".format(c))
print("{0:.1f}".format(s/c))
```

---
