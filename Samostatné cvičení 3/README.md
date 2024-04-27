# Samostatné cvičení 3

## 1 - Řetězce jako sekvence
Vytvořte nový program **jmeno.py**. Do proměnné jmeno uložte svoje celé jméno a nechte vypsat jeho třetí, pátý a sedmý znak. Vyzkoušejte, co se stane, když budete chtít znak na pozici, která překračuje délku řetězce.

<details>
<summary><b>Řešení</b></summary>

```Python
jmeno = "František Novák"

print(f"Třetí znak: {jmeno[2]}")  # 'a'
print(f"Pátý znak: {jmeno[4]}")  # 't'
print(f"Sedmý znak: {jmeno[6]}")  # 'š'

```

</details>

## 2 - Seznamy
Vytvořte nový program **seznam.py**. V tomto programu vytvořte následující:
- Vytvořte nějaký seznam celých čísel, například počty diváků na několika po sobě jdoucích představeních.
- Vytvořte nějaký seznam desetinných čísel, například zaplněnost divadla v několika po sobě jdoucích představeních.
- Vytvořte nějaký seznam řetězců, například seznam názvů několika divadelních představení, která divadlo hraje. Uložte tento   seznam do proměnné hry. Uložte do nějaké proměnné druhou položku tohoto seznamu.
- Do proměnné hodnoceni uložte seznam hodnocení, které obdržela divadelní hra "Plyšáci na útěku" v různých recenzních časopisech. Hodnocení je vždy dvouprvkový seznam obsahující název recenzního časopisu jako řetězec a samotné hodnocení jako číslo mezi 1 až 10

<details>
<summary><b>Řešení</b></summary>

```Python
divaci = [120, 150, 130, 145, 160]
zaplnenost = [0.9, 0.85, 0.95, 0.80, 0.75]
hry = ["Hamlet", "Romeo a Julie", "Válka s mloky", "Faust", "Othello"]
druha_hra = hry[1]  # "Romeo a Julie"

hodnoceni = [
    ["Divadelní noviny", 8],
    ["Scéna", 7],
    ["Kultura21", 9],
    ["Theatrolog", 6]
]

```

</details>

## 3 - Ověřování hesla
Založte si program **heslo.py**. Ověřování hesla se někdy dělá tak, že se vás systém ptá pouze na některé jeho znaky. Napište program, který má uloženo heslo, které musí uživatel zadat. Pak se jej postupně zeptejte například na druhý, pátý a sedmý znak hesla. Propusťte uživatele pouze tehdy, zadá-li všechny tyto znaky správně.

<details>
<summary><b>Řešení</b></summary>

```Python
heslo = "bezpecneHeslo123"

druhy_znak = input("Zadejte druhý znak vašeho hesla: ")
paty_znak = input("Zadejte pátý znak vašeho hesla: ")
sedmy_znak = input("Zadejte sedmý znak vašeho hesla: ")

if (druhy_znak == heslo[1] and paty_znak == heslo[4] and sedmy_znak == heslo[6]):
    print("Heslo ověřeno, vstup povolen.")
else:
    print("Nesprávné znaky, vstup nepovolen.")

```

</details>