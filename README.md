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
### V programu je zapotřebí knihovna random aby jsme mohly generovat čísla z našich nastavených hranic (v programu je hranice 0 až 999 pro obě proměné).
### Program je rozdělenej na tři části.
### - Nekonečná smička (while True)
### - Vypracování výsledku (def plus/minus/naso/delit)
### - Podávání příkladu (def priklad)

## Nekonečná smička (while True)
#### 1. V nekonečné smičce se nachází generace dvou náhodných proměních |rannum1| a |rannum2| z stanoveními hranicemi 0 až 999.
#### 2.Pak program vypíše zpravy aby uživately oznamil možnosti mezi kterými si vybere číslem vypsaní ve zprávách.
#### 3.Po uživately je žádáno aby zadal čísla od 1 do 4 pokud zadá jiné čísla než je poněm žádáno program se ho požádá znovu dokud nenapíše zprávný (dály však písmeno program ohlásí chybu protože float příjmá poze čísla neboli jejich hodnoty a musí se program restartovat).
#### 4.Pak nás program zavede do série podmínek, podle čísla které jsme z těch tří vybrali se  posuneme do vnitřku splněné podmínky a spouštíme Podávání příkladu.
![while projek](https://github.com/user-attachments/assets/0e1de3ae-d76a-4c20-9dcc-972b487f0d07)

## Vypracování výsledku (def plus/minus/naso/delit)
#### 1. Funkce !plus! co vyžaduje proměné |rannum1| a |rannum2| pro její funkčnost. V tomhle případě sčítá dvě čísla mezi sebou do proměné rovnoP (P jako Plus): rovnoP je potom hned vypsáno do terminálu.
#### 2. Funkce !minus! co vyžaduje proměné |rannum1| a |rannum2| pro její funkčnost. V tomhle případě odečíta dvě čisla mezi sebou do proměné rovnoP (P jako Plus): rovnoP je potom hned vypsáno do terminálu.
#### 3. Funkce !naso! co vyžaduje proměné |rannum1| a |rannum2| pro její funkčnost. V tomhle případě nasobí dvě proměné mezi sebou do proměné rovnoP (P jako Plus): rovnoP je potom hned vypsáno do terminálu.
#### 4. Funkce !delit! co vyžaduje proměné |rannum1| a |rannum2| pro její funkčnost. V tomhle případě dělí dvě čísla mezi sebou do proměné rovnoP (P jako Plus): rovnoP je potom hned vypsáno do terminálu.
![projekvzpracovani](https://github.com/user-attachments/assets/e88cb66e-bb27-4bfa-89ca-0a3aa578c260)

##Podávání příkladu (def priklad)
#### 1. Podle našeho zvoleného čísla se dostaneme do vnitřku podmínky s danou operací 1.Sčítání, 2.Odečítaní, 3. Nasobení, 4. Dělení.
#### 2. Když bylo naše zvolené číslo 1 tak se nám v terminálu oběví zprava ("Vypocítej příklad:",rannum1 ,"+", rannum2) kde |rannum1| a |rannum2| jsou vygenerovaní čísla už od smičky. Pak jsme vyžadani napsat číslo které vypočítame. Po zadání čísla nám hned vyskočí výsledek z příslušné funkce zde je to !plus!
#### 3. Když bylo naše zvolené číslo 2 tak se nám v terminálu oběví zprava ("Vypocítej příklad:",rannum1 ,"-", rannum2) kde |rannum1| a |rannum2| jsou vygenerovaní čísla už od smičky. Pak jsme vyžadani napsat číslo které vypočítame. Po zadání čísla nám hned vyskočí výsledek z příslušné funkce zde je to !minus!
#### 4. Když bylo naše zvolené číslo 3 tak se nám v terminálu oběví zprava ("Vypocítej příklad:",rannum1 ,"*", rannum2) kde |rannum1| a |rannum2| jsou vygenerovaní čísla už od smičky. Pak jsme vyžadani napsat číslo které vypočítame. Po zadání čísla nám hned vyskočí výsledek z příslušné funkce zde je to !naso!
#### 5. Když bylo naše zvolené číslo 4 tak se nám v terminálu oběví zprava ("Vypocítej příklad:",rannum1 ,"/", rannum2) kde |rannum1| a |rannum2| jsou vygenerovaní čísla už od smičky. Pak jsme vyžadani napsat číslo které vypočítame. Po zadání čísla nám hned vyskočí výsledek z příslušné funkce zde je to !delit!
![projekaqqpriklad](https://github.com/user-attachments/assets/3d9d5150-f9fe-4b78-8c4a-754e9472ebc5)
c
cc
c
