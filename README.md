# GymTracker PRO v4 — Studio Edition

Responsywna prywatna aplikacja treningowa PWA, inspirowana przesłaną przez użytkownika wizualizacją: grafitowo-bordowe tło, różowe gradienty, lekki interfejs i abstrakcyjne formy 3D.

## Zawartość
- Pulpit z interaktywną, animowaną **proceduralną rzeźbą WebGL** (bez zewnętrznych bibliotek, bez pobieranych modeli) oraz efektem ruchu tła przy przewijaniu.
- Druga abstrakcyjna forma 3D na ekranie osiągnięć.
- Treningi Góra / Dół A/B, konfiguracja aktualnych obciążeń przed pierwszą sesją, zapisywanie serii, powtórzeń, RIR i oceny techniki.
- Sugerowanie progresji według reguły dwóch kolejnych sesji z pełną liczbą powtórzeń. Zmiana obciążenia zawsze po potwierdzeniu.
- Wykresy ciężaru na podstawie prawdziwych zapisów, historia i 27 osiągnięć.
- Dane w localStorage, import/eksport JSON; instalacja jako PWA po publikacji pod HTTPS.
- Usunięto nawigację i wizualizacje anatomii/musculatury.

## Uruchomienie
1. Rozpakuj ZIP.
2. Lokalnie otwórz `GymTracker-PRO-v4-preview.html` (jednoplikowy podgląd) albo uruchom serwer HTTP w katalogu projektu: `python -m http.server 8000` i przejdź pod `http://localhost:8000/`.
3. Aby korzystać na iPhonie, opublikuj **zawartość** katalogu na GitHub Pages (Settings → Pages → Deploy from branch → main / root); otwórz HTTPS w Safari i wybierz „Dodaj do ekranu początkowego”.

## Dane / prywatność
Zachowano klucz przechowywania `gymtracker-pro-v2`, żeby nie utracić wcześniej zapisanych danych na tej samej domenie. Historia zapisana na iPhonie nie będzie automatycznie dostępna na komputerze. Wykonaj kopię JSON przed zmianą przeglądarki lub domeny. Repozytorium GitHub Pages może być publicznie dostępne, ale wyniki pozostają lokalne w przeglądarce.

## WebGL i animacje
Rzeźby są generowane w kodzie JavaScript jako siatki przestrzenne i animowane przez WebGL. Nie są zewnętrznymi plikami GLB; nie wymagają sieci. Gdy WebGL jest niedostępny, widać statyczną/animowaną formę CSS. Na urządzeniach z ograniczeniem ruchu animacje są redukowane. Rzeczywistą wydajność należy sprawdzić na docelowym iPhonie.
