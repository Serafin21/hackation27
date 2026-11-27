# EnergoPatrol · Łowcy Strat

Klikalny prototyp na **Innovation Hack Cementowni Warta** (#BudujemyBezpieczneJutro), Wyzwanie 4: *Jak zwiększyć świadomość i zaangażowanie pracowników w realizację celów ESG poprzez ich codzienne działania?*

Zespół **eFn**: Mikołaj Woźny, Jakub Dworczyk, Szymon Serafin.

## Idea w jednym zdaniu
Pracownik robi zdjęcie straty, a po naprawie dowiaduje się, ile zaoszczędził zakładowi i środowisku. Cały zakład widzi to na telebimie, a zmiana dostaje 20% zweryfikowanej oszczędności do wspólnej skarbonki.

## Co jest w prototypie
Jeden plik `index.html`, bez instalacji, zaprojektowany pod telefon.

| Adres | Ekran |
| --- | --- |
| `index.html` | **demo 1:1 z animacją**: ekran telefonu → aparat → zgłoszenie z mapą i kategorią → utrzymanie ruchu potwierdza naprawę → Twój wpływ i głosowanie → ranking (osoby, zmiany, cała firma) → wyłączanie urządzeń na postój |
| `animacja.html` | animacja pokazowa (ok. 50 s) do prezentacji |
| `panel.html` | wcześniejszy prototyp (aplikacja z mapą zakładu) |
| `panel.html#telebim` | telebim zakładu: cel miesiąca, strata tygodnia, ranking wydziałów, skarbonka |
| `panel.html#symulator` | symulator KPI pilotażu z suwakami |

Na telefonie demo wypełnia cały ekran; na komputerze pokazuje się w ramce telefonu (przycisk „Od nowa” w rogu). Naprawę przez utrzymanie ruchu demo symuluje samo po kilku sekundach.

## Uruchomienie
- Lokalnie: otwórz `index.html` w przeglądarce.
- Na telefonie (zalecane): włącz GitHub Pages (Settings → Pages → Branch `main`, folder `/`). Strona będzie pod adresem `https://serafin21.github.io/hackation27/`. Z tego adresu zrób kod QR do slajdu.
- Aparat i lokalizacja działają tylko przez HTTPS (GitHub Pages to zapewnia).

## Liczby
Wszystkie wartości to **szacunki na danych przykładowych** (zgodnie z regulaminem oznaczone w interfejsie). Parametry w `CFG` na początku skryptu:

- cena prądu 0,8 zł/kWh (parametr, do potwierdzenia z Wartą),
- 0,6 t CO₂/MWh,
- wycieki sprężonego powietrza: 1,1 / 4,3 / 17,2 kW (mały / ok. 3 mm / duży), 8000 h/rok,
- 20% zweryfikowanej oszczędności do skarbonki zmiany (propozycja).

## Zasady wbudowane w prototyp
- Wartość pojawia się dopiero po potwierdzeniu naprawy przez utrzymanie ruchu, nie po samym zdjęciu.
- Skarbonka jest wspólna dla zmiany; brak nagród indywidualnych i rankingu osób.
- Ranking na telebimie dotyczy wydziałów i liczy spadek zużycia energii z liczników.
- Lokalizacja pobierana tylko w chwili zgłoszenia, bez śledzenia.
- Zero kar.

## Użycie AI
Zgodnie z regulaminem: kod prototypu powstał z istotnym udziałem asystenta AI (Claude, Anthropic) na podstawie koncepcji, animacji i decyzji zespołu eFn.
