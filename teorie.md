# Část otázek

## Jaké jsou datové typy v Javascriptu?
string ("Dnes je prekrasny den !!",'Hello world !'), number (1;25,5257245;..), boolean (true,false), undefined (prázdno, není ji nic přiřazeno), object, null, Bigint, Symbol

## Jaký je rozdíl v porovnání pomocí `==` a `===`?
"==" porovnává hodnotu rozdílným datatypům (1 == "1"). Zatímco "===" porovnává hodnotu stejným datatypům (1 === 1).

## Kde se používá klíčové slovo `case`?
Můžeme string předělat na buď na to aby byl celý string v lowercasu(ahoj světe), či upper casu (AHOJ SVĚTE). Můžeme jej zapsat takto toDoList.toLowerCase() když chceme lower case a takto 
toDoList.toUpperCase() když chceme upper case. Case se tedy používá k úpravě a zahlazení stringů do jednoho typu  písma, buď lower nebo upper.

## Jak se používá a k čemu slouží funkce `filter()` nad polem?
Je schopen filtrovat v array pomocí předem definovaného zadání. Můžeme tak v kódu udělat funkci do které zapíšeme co chceme aby dělala, v tomto případě třeba nevypisovala všechny slova kde je písmeno X. Potom si jen do nějaké proměné dosadíme aby se rovnola vyfiltrované proměné kde byl mezi kulaté závorky dosazen filtr podle kterého jsme chtěli filtrovat. Dole ukázka protože nevím zda je moje slovní odpověď dostatečná.

function hasShortName(string) {
        return string.length <= 6;
    }

    const euCountriesArray = [
        "Germany",
        "France",
        "Italy",
        "Spain",
        "Poland",
        "Netherlands",
        "Belgium",
        "Greece",
    ];
    console.log(euCountriesArray);

    const euCountriesWithShortNames = euCountriesArray.filter(hasShortName);
    console.log(euCountriesWithShortNames);
Zdroj: https://github.com/Dice-Sensei/spselit-javascript/blob/main/08-Loops.md
## Jaké jsou rozdíly mezi polem a Set kolekcí?
Pole umožňuje hodnotám být obsaženy X krát v jednom poli což set neumožňuje.
Oba mají jinou syntaxi commandů - Set: .clear , .size ,...
Map: .unshift, .push,... 
V Setu nemůžeme přistupovat k prvkum pomocí indexu (čísla pořadí).
