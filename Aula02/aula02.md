# Aula 02

## Listas

Uma lista é uma coleção mutável e ordenada de elementos, que pode conter diferentes tipos de dados (inteiros, strings, listas, etc.).

**Criação de Lista**
```python
frutas = ['maçã', 'banana', 'laranja']
```

**Acesso por índice**
```python
print(frutas[0])  # maçã
print(frutas[1])  # banana
```

**Modificação**
```python
frutas[1] = 'abacaxi'
print(frutas)  # ['maçã', 'abacaxi', 'laranja']
```

**Iteração**
```python
for fruta in frutas:
    print(fruta)
```

## Tuplas em Python

Uma tupla é uma coleção imutável e ordenada de elementos. Útil para garantir que os dados não sejam alterados acidentalmente.

**Criação de Tupla**
```python
coordenadas = (10, 20)
```

**Acesso por índice**
```python
print(coordenadas[0])  # 10
print(coordenadas[1])  # 20
```

**Iteração**
```python
for valor in coordenadas:
    print(valor)
```

## Dicionários em Python

Um dicionário armazena pares chave:valor.

**Criação de Dicionário**
```python
aluno = {'nome': 'Ana', 'idade': 22, 'curso': 'Python'}
```

**Acesso por chave**
```python
print(aluno['nome'])  # Ana
```

**Modificação e Adição**
```python
aluno['idade'] = 23
aluno['nota'] = 9.5
print(aluno)
```

**Iteração**
```python
for chave, valor in aluno.items():
    print(f'{chave}: {valor}')
```

# Indexação e Slice (Fatiamento)

Tanto listas quanto tuplas e strings suportam indexação e fatiamento.

**Indexação**
```python
lista = ['a', 'b', 'c', 'd']
print(lista[0])   # a
print(lista[-1])  # d (último elemento)
```

**Fatiamento (slice)**
```python
print(lista[1:3])     # ['b', 'c']
print(lista[:2])      # ['a', 'b']
print(lista[::2])     # ['a', 'c'] (de 2 em 2)
print(lista[::-1])    # ['d', 'c', 'b', 'a'] (reverso)
```

**Slice com Strings**
```python
mensagem = "Python é divertido"
print(mensagem[0:6])  # Python
print(mensagem[-9:])  # divertido
```

**Impressão de Itens**

**Lista**
```python
numeros = [1, 2, 3, 4]
for n in numeros:
    print(n)
```

**Tupla**
```python
cores = ('vermelho', 'verde', 'azul')
for cor in cores:
    print(cor)
```

**Dicionário**
```python
pessoa = {'nome': 'Carlos', 'idade': 30}
for chave in pessoa:
    print(f'{chave}: {pessoa[chave]}')
```

# Estruturas Condicionais

As estruturas condicionais permitem executar diferentes blocos de código dependendo de condições lógicas. Em Python, usamos as palavras-chave:

- if – se a condição for verdadeira
- elif – senão se... (opcional e pode haver vários)
- else – senão (opcional e só pode haver um)

```python
if condição:
    # bloco se a condição for verdadeira
elif outra_condição:
    # bloco se a segunda condição for verdadeira
else:
    # bloco se nenhuma condição anterior for verdadeira
```

## Exemplos de Uso

**Exemplo 1: Verificar idade para votar**
```python
idade = 16

if idade >= 18:
    print("Pode votar.")
else:
    print("Não pode votar.")
```

**Exemplo 2: Classificação de notas**
```python
nota = 8.5

if nota >= 9:
    print("Excelente!")
elif nota >= 7:
    print("Bom!")
elif nota >= 5:
    print("Regular.")
else:
    print("Reprovado.")
```

**Exemplo 3: Número par ou ímpar**
```python
numero = 7

if numero % 2 == 0:
    print("Par")
else:
    print("Ímpar")
```

## Condição com Operadores Lógicos

Podemos usar operadores como and, or, not nas condições:
```python
idade = 20
tem_carteira = True

if idade >= 18 and tem_carteira:
    print("Pode dirigir.")
else:
    print("Não pode dirigir.")
```

## Condicional com Operador Ternário (forma compacta)
```python
idade = 17
mensagem = "Maior de idade" if idade >= 18 else "Menor de idade"
print(mensagem)
```

