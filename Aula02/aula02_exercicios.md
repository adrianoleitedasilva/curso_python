# Exercícios Listas

- Crie uma lista com cinco nomes de frutas e:
    - Imprima a segunda fruta da lista.
    - Substitua a terceira fruta por outra.
    - Adicione uma nova fruta no final.
    - Imprima todas as frutas, uma por linha.
- Peça ao usuário para digitar 5 números e armazene-os em uma lista.
    - Depois, imprima apenas os números pares.

# Exercícios Tuplas

- Crie uma tupla com os dias da semana e:
    - Imprima o primeiro e o último dia.
    - Verifique se "domingo" está na tupla.
    - Itere sobre a tupla e imprima cada dia com um índice (ex: "0 - segunda").
- Crie uma tupla com três números e calcule a média deles.

# Exercícios Dicionários

- Crie um dicionário chamado aluno com as chaves: nome, idade, nota.
    - Imprima cada item do dicionário no formato: "nome: João".
- Peça ao usuário para cadastrar três produtos com seus preços (dica: use um dicionário).
    - Depois, mostre todos os produtos e preços cadastrados.

# Exercícios Slide e Indexação

```python
letras = ['a', 'b', 'c', 'd', 'e', 'f', 'g']
```
- Dada a lista acima:
    - Imprima os três primeiros elementos.
    - Imprima os três últimos.
    - Inverta a lista usando slice.
    - Imprima apenas as letras nas posições pares.
- Peça ao usuário para digitar uma palavra e:
    - Mostre apenas os três primeiros caracteres.
    - Mostre a palavra ao contrário.

# Exercícios: Estruturas Condicionais

- Peça ao usuário uma idade:  
    - Diga se é menor de idade, maior de idade ou idoso (idade ≥ 60).
- Peça ao usuário uma nota de 0 a 10:
    - Diga se ele foi reprovado (nota < 5), em recuperação (5 ≤ nota < 7), ou aprovado (nota ≥ 7).
- Peça dois números e:
    - Diga qual é o maior, ou se são iguais.
- Crie um programa que peça ao usuário para digitar um número inteiro.
    - Diga se é par ou ímpar.
    - Se for múltiplo de 5, diga isso também.
-----------------------------------------------------
**Lista de frutas**
```python
frutas = ['maçã', 'banana', 'laranja', 'uva', 'melancia']
print(frutas[1])  # banana

frutas[2] = 'kiwi'
frutas.append('abacaxi')

for fruta in frutas:
    print(fruta)
```

**Números pares em uma lista**
```python
numeros = []

for i in range(5):
    n = int(input("Digite um número: "))
    numeros.append(n)

print("Números pares:")
for n in numeros:
    if n % 2 == 0:
        print(n)
```

**Tupla com dias da semana**
```python
dias = ('segunda', 'terça', 'quarta', 'quinta', 'sexta', 'sábado', 'domingo')

print(dias[0])        # segunda
print(dias[-1])       # domingo

print("domingo" in dias)  # True

for i, dia in enumerate(dias):
    print(f"{i} - {dia}")
```

**Média de três números**
```python
numeros = (7, 8, 9)
media = sum(numeros) / len(numeros)
print("Média:", media)
```

**Dicionário de aluno**
```python
aluno = {
    'nome': 'João',
    'idade': 20,
    'nota': 8.7
}

for chave, valor in aluno.items():
    print(f"{chave}: {valor}")
```

**Cadastro de produtos**
```python
produtos = {}

for i in range(3):
    nome = input("Digite o nome do produto: ")
    preco = float(input("Digite o preço: "))
    produtos[nome] = preco

print("Produtos cadastrados:")
for produto, preco in produtos.items():
    print(f"{produto}: R$ {preco:.2f}")
```


**Lista de letras**
```python
letras = ['a', 'b', 'c', 'd', 'e', 'f', 'g']

print(letras[:3])     # ['a', 'b', 'c']
print(letras[-3:])    # ['e', 'f', 'g']
print(letras[::-1])   # ['g', 'f', 'e', 'd', 'c', 'b', 'a']
print(letras[::2])    # ['a', 'c', 'e', 'g']
```

**Palavra do usuário**
```python
palavra = input("Digite uma palavra: ")
print("3 primeiros caracteres:", palavra[:3])
print("Ao contrário:", palavra[::-1])
```

**Faixa etária**
```python
idade = int(input("Digite sua idade: "))

if idade < 18:
    print("Menor de idade")
elif idade >= 60:
    print("Idoso")
else:
    print("Maior de idade")
```

**Classificação de nota**
```python
nota = float(input("Digite a nota (0 a 10): "))

if nota < 5:
    print("Reprovado")
elif nota < 7:
    print("Recuperação")
else:
    print("Aprovado")
```

**Maior número**
```python
a = int(input("Digite o primeiro número: "))
b = int(input("Digite o segundo número: "))

if a > b:
    print("O primeiro número é maior.")
elif b > a:
    print("O segundo número é maior.")
else:
    print("Os números são iguais.")
```

**Par/ímpar e múltiplo de 5**
```python
numero = int(input("Digite um número inteiro: "))

if numero % 2 == 0:
    print("Par")
else:
    print("Ímpar")

if numero % 5 == 0:
    print("Múltiplo de 5")
```