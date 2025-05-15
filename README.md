# Projekt Program_Jednoduchá_Matika | Ondřej Karásek


## Základní informace


Jedná se o druhý školní ročníkový projekt.

Tento projekt byl vypracovaní: Ondřejem Karáskem

Třída: T3A

Školním roce: 2024/25

Skupina: P1


#### Úkolem bylo udělat jednoduchej a pochopitelnej program s využitím funkcí.
#### Protože fukce nejsou na naši škole moc probrané.
#### Byl tento program zaměřenej hlavně na ně.


## Co jsem udělal?
#### Jednoduchý časově nenároční program na procvičení základních matematickích operaci (+, -, *, /) kde obsah programu je primárně z funkcí.
#### Program je napsaní tak že se do něj dají jednoduše přidávat další matematické operace pro vlastní účely.


## Cíl
#### Protože jsem člověk který ve svém životě nic nepotřebuje a hodně věcí mi připadá zbitečních, tak jsem udělal něco co bi mohl aspoň muj bratr jednou použít až vyroste.


## Aplikace / Programovací jazyk
#### Aplikace ve které je program napsán: [PyCharmCommunity](https://pycharm-community-edition.en.softonic.com/)
#### Programovací jazyk: [Python](https://www.python.org/)


## Využité zdroje
#### Stránka ze který jsem čerpal informace o fungování funkcí [W3Schools](https://www.w3schools.com/python/python_functions.asp)
#### Část z fukcemi zde:[Funkce](https://www.w3schools.com/python/python_functions.asp)

## Program
> Matika

    import random

    def priklad():

        if vyber_prikladu == 1:
            print("Vypocítej příklad:",rannum1 ,"+", rannum2)
            uzi_vyz1 = float(input("Zadej vysledek: "))
            plus(rannum1,rannum2)

        elif vyber_prikladu == 2:
            print("Vypocítej příklad:", rannum1 ,"-", rannum2)
            uzi_vyz1 = float(input("Zadej vysledek: "))
            minus(rannum1, rannum2)

        elif vyber_prikladu == 3:
            print("Vypocítej příklad:", rannum1 ,"*", rannum2)
            uzi_vyz1 = float(input("Zadej vysledek: "))
            naso(rannum1, rannum2)

        elif vyber_prikladu == 4:
            print("Vypocítej příklad:", rannum1 ,"/", rannum2)
            uzi_vyz1 = float(input("Zadej vysledek: "))
            delit(rannum1, rannum2)

    def plus(rannum1, rannum2):
        rovnoP = rannum1 + rannum2
        print("Zprávný výsledek je",rovnoP)
        
    def minus(rannum1, rannum2):
        rovnoM = rannum1 - rannum2
        print("Zprávný výsledek je",rovnoM)
        
    def naso(rannum1, rannum2):
        rovnoN = rannum1 * rannum2
        print("Zprávný výsledek je",rovnoN)
        
    def delit(rannum1, rannum2):
        rovnoD = rannum1 / rannum2
        print("Zprávný výsledek je",rovnoD)

    while True:
        rannum1 = random.randrange(0, 999)
        rannum2 = random.randrange(0, 999)
        print("1. Sčítání")
        print("2. Odečítání")
        print("3. Nasobení")
        print("4. Dělení")
        vyber_prikladu = float(input("Napiš číslo podle toho co chceš počítat."))
        if vyber_prikladu == 1:
            priklad()
        elif vyber_prikladu == 2:
            priklad()
        elif vyber_prikladu == 3:
            priklad()
        elif vyber_prikladu == 4:
            priklad()
## Jak to funguje?
### Program je rozdělenej na tři části
### - Podávání příkladu (def priklad)
### - Vypracování výsledku (def plus/minus/naso/delit)
### - Nekonečná smička (while True)
