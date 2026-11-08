# GymTracker Focus — gotowe plany 4-dniowe

Zachowany minimalistyczny interfejs z trzema zakładkami: **Trening / Kalendarz / Progres**.

## Wbudowany plan
- Poniedziałek — Upper A: 7 ćwiczeń, 18 serii
- Wtorek — Lower A: 6 ćwiczeń, 16 serii
- Czwartek — Upper B: 8 ćwiczeń, 22 serie
- Piątek — Lower B: 6 ćwiczeń, 18 serii

Każde ćwiczenie ma dokładną liczbę serii i zakres powtórzeń zgodny z podaną rozpiską. Góra/Dół A/B pozostają edytowalne. W edycji dostępny jest przycisk „Przywróć gotowy plan”.

## Instalacja
Rozpakuj ZIP i prześlij pliki **z folderu** `GymTracker-Focus-Plany` do katalogu publikowanego przez GitHub Pages (np. root repozytorium). Otwórz `index.html` przez serwer HTTP albo GitHub Pages.

## Dane
Przechowywane w localStorage pod kluczem `gymtracker-iphone14plus` jak w poprzedniej wersji Focus. Aktualizacja nie czyści historii. Wcześniejsze własne zmiany ćwiczeń pozostają zachowane — jeśli chcesz mieć komplet nowego planu, kliknij „Edytuj plan” → „Przywróć gotowy plan”.

Zdjęcia ćwiczeń ładowane są z publicznej bazy `yuhonas/free-exercise-db` i wymagają internetu. Niektóre zdjęcia dla wariantów ćwiczeń mogą być niedostępne — aplikacja pokazuje wtedy komunikat zastępczy.


## Aktualizacja: zmiana trwającego treningu
- Strzałka „Wróć” prowadzi na ekran główny, nie kończąc aktywnej sesji.
- „Zmień trening” umożliwia wybór innego planu. Zmiana z zapisanymi seriami wymaga potwierdzenia, ponieważ usuwa tylko serie z bieżącej, niedokończonej sesji.
- Poprzednie ukończone treningi i ustawione ciężary są zachowywane.
- Na iPhonie zablokowano przypadkowy zoom i ruch poziomy; pionowy scroll pozostaje aktywny.


## Nowość: poprzedni trening ćwiczenia
Na ekranie wykonywanego ćwiczenia pojawia się ostatnia ukończona sesja z tym ćwiczeniem: data, liczba zapisanych serii, wykorzystany ciężar oraz waga i powtórzenia dla każdej serii. Historia wyszukiwana jest we wszystkich czterech planach i nie obejmuje niezakończonego bieżącego treningu.

## Dodatki tej wersji
- Wybór planu bez przypisywania go do dnia tygodnia.
- Poprzednia sesja tego samego ćwiczenia: liczba serii, ciężary i powtórzenia.
- 150 osiągnięć (6 kategorii po 25 poziomów) liczonych z ukończonych treningów: sesje, serie, powtórzenia, tonaż, maksymalny ciężar, poprawione rekordy.
- Filtry według kategorii/statusu i stronicowanie po 25 elementów.
- Nie naliczamy wyników z rozpoczętej, niezakończonej sesji.
