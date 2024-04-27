# Samostatné cvičení 4

## 1 - Seznam hodnocení

Mějme seznam hodnocení divadelní hry Plyšáci na útěku , který vypadá takto: 

```python
hodnoceni = [7, 9, 6, 7, 9, 8]
```

- Vytvořte program, který projde tento seznam a vypíše každé hodnocení na nový řádek.
- Upravte program tak, aby vypisoval výstup v tomto formátu

```python
7/10
9/10
6/10
7/10
9/10
8/10
```

<details>
<summary><b>Řešení</b></summary>

```Python
hodnoceni = [7, 9, 6, 7, 9, 8]
for rating in hodnoceni:
    print(f"{rating}/10")

```

</details>

## 2 - Procházení seznamu
Založte si program **hesla.py** a na jeho začátek vložte následující kód obsahující seznam hesel pro přihlášení do nějakého systému

```python
hesla = [
    "xyz101",
    "punťa",
    "razor-blade",
    "1234",
    "12011986",
    "martin111",
    "trhnisi",
    "hokuspokus",
    "jeník15",
    "kristus-te-spasi",
    "beruška",
    "strčprstskrzkrk",
]
```

- Pomocí cyklu vypište všechny hesla na obrazovku, každé na jeden řádek.
- Upravte váš program tak, aby vypisoval jen bezpečná hesla, tedy taková, jež jsou delší než 8 znaků.

<details>
<summary><b>Řešení</b></summary>

```Python
hesla = [
    "xyz101",
    "punťa",
    "razor-blade",
    "1234",
    "12011986",
    "martin111",
    "trhnisi",
    "hokuspokus",
    "jeník15",
    "kristus-te-spasi",
    "beruška",
    "strčprstskrzkrk",
]

print("Všechna hesla:")
for heslo in hesla:
    print(heslo)

print("\nBezpečná hesla (delší než 8 znaků):")
for heslo in hesla:
    if len(heslo) > 8:
        print(heslo)

```

</details>

## 3 - Složitější seznam
Založte si program **cykly02.py** a použijte v něm následující seznam měsíců v roce, Všimněte si, že je to seznam seznamů.

```python
mesice = [
    ["leden", 31],
    ["únor", 28],
    ["březen", 31],
    ["duben", 30],
    ["květen", 31],
    ["červen", 30],
    ["červenec", 31],
    ["srpen", 31],
    ["září", 30],
    ["říjen", 31],
    ["listopad", 30],
    ["prosinec", 31],
]
```

- Pomocí cyklu projděte tento seznam a vypište na výstup názvy jednotlivých měsíců.
- Pomocí dalšího cyklu vypište na výstup počty dní v jednotlivých měsících.

<details>
<summary><b>Řešení</b></summary>

```Python
mesice = [
    ["leden", 31],
    ["únor", 28],
    ["březen", 31],
    ["duben", 30],
    ["květen", 31],
    ["červen", 30],
    ["červenec", 31],
    ["srpen", 31],
    ["září", 30],
    ["říjen", 31],
    ["listopad", 30],
    ["prosinec", 31],
]

print("Názvy měsíců:")
for mesic in mesice:
    print(mesic[0])

print("\nPočty dnů v jednotlivých měsících:")
for mesic in mesice:
    print(f"{mesic[0]}: {mesic[1]} dnů")

```

</details>