# Samostatné cvičení 5

## 1 - Násobení
Napiš funkci mult, která bude mít dva číselné parametry. Funkce oba parametry vynásobí a vrátí výsledek.

<details>
<summary><b>Řešení</b></summary>

```Python
def mult(a, b):
    return a * b

```

</details>

## 2 - Hotel
Napiš funkci total_price, která vypočte cenu noci v hotelu. Funkce bude mít dva parametry - persons a breakfast. Cena za noc za osobu je 850 Kč a cena za snídani za osobu je 125 Kč. Funkce vrátí výslednou cenu. Parametr breakfast je nepovinný a výchozí hodnota je False.

Funkci vyzkoušej se zadáním dvou i jedné hodnoty, např. total_price(3), total_price(2, True).

<details>
<summary><b>Řešení</b></summary>

```Python
def total_price(persons, breakfast=False):
    base_price = 850 
    breakfast_price = 125 if breakfast else 0
    return (base_price + breakfast_price) * persons

```

</details>

## 3 - Faktoriál
Vytvořte program, který obsahuje funkci pro výpočet libovolného faktoriál. (https://cs.wikipedia.org/wiki/Faktori%C3%A1l)

<details>
<summary><b>Řešení</b></summary>

```Python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

```

</details>
