# Samostatné cvičení 2

## 1 - Jednoduché podmínky
Založte si program **prihlaseni.py**. V tomto nechte uživatele zadat svoje uživatelské jméno a poté heslo. Pokud se heslo neshoduje s heslem simsalabim, vypište na výstup **Vstup nepovolen** a zavolejte funkci exit(), aby uživatel neznalý hesla nemohl s programem dál pracovat.

Na konec programu vlož příkaz, který se uživatele zeptá na věk. Pokud je uživatel starší 18 let, vypište na výstup **Smíš vstoupit** Pokud je mladší, vypiš **Vstup povolen od 18 let**

<details>
<summary><b>Řešení</b></summary>

```Python
uzivatelske_jmeno = input("Zadejte uživatelské jméno: ")
heslo = input("Zadejte heslo: ")

if heslo != "simsalabim":
    print("Vstup nepovolen")
    exit()
```

</details>

## 2 - Cena vstupenky

Vytvořte program **vstupenky01.py**, vytvořte si proměnnou plnaCena, do které uložte hodnotu 12.
Vytvořte podmínku, která do proměnné cena uloží cenu spočítanou podle věku uživatele dle následujících pravidel
- 0 euro pro návštěvníky mladší 6 let,
- 65% ze základní ceny pro návštěvníky 6 až 26 let (žák, student),
- 100% ze základní ceny pro návštěvníky 27 až 64 let (dospělý),
- 50% ze základní ceny pro ostatní (senior).
Nezapomeňte na zaokrouhlování, ať nám cena vyjde v celých centech. (využijte funkci round())

Nakonec spočtenou cenu vypište s nějakou hezkou zprávou na výstup.

<details>
<summary><b>Řešení</b></summary>

```Python
plnaCena = 12

vek = int(input("Zadejte svůj věk: "))

if vek < 6:
    cena = 0
elif vek <= 26:
    cena = round(0.65 * plnaCena, 2)
elif ek <= 64:
    cena = plnaCena
else:
    cena = round(0.5 * plnaCena, 2)

print(f"Cena vaší vstupenky je {cena} euro. Děkujeme za nákup!")
```

</details>

## 3 - Registrace

Založte si program **registrace.py**. Program nechá uživatele, aby si zvolil uživatelské jméno a heslo. Heslo jej nechejte zadat dvakrát a ověřte, že jej uživatel zadal dvakrát stejně. V opačném případě vypište varování, že hesla nejsou stejná. Při prvním zadávání ověřte, že heslo je bezpečné, což v tomto případě znamená, že je delší než 8 znaků (využijte funkci len()).

<details>
<summary><b>Řešení</b></summary>

```Python
uzivatelske_jmeno = input("Zadejte uživatelské jméno: ")
heslo1 = input("Zadejte heslo: ")

if len(heslo1) > 8:
    heslo2 = input("Zadejte heslo znovu pro potvrzení: ")
    if heslo1 == heslo2:
        print("Registrace úspěšná. Vítejte, " + uzivatelske_jmeno + "!")
    else:
        print("Hesla nejsou stejná. Zkuste to znovu.")
else:
    print("Heslo musí být delší než 8 znaků.")
```

</details>