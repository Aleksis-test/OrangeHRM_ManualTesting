# OrangeHRM QA Project

Projekt testerski aplikacji OrangeHRM obejmujący:

- testy manualne,
- zgłoszenia błędów,
- testy wydajnościowe,
- analizę odpowiedzi HTTP,
- walidację działania aplikacji.

---

# Zakres projektu

## Testy manualne
Przygotowano scenariusze testowe dla modułów:

- Logowanie
- Dashboard
- PIM
- Leave
- Buzz

Wykonano:
- testy funkcjonalne,
- testy negatywne,
- walidację formularzy,
- testy UI,
- testy użyteczności.
- testy dostępności WCAG

---

# Bug Reports

Przygotowano zgłoszenia błędów w Jira.

Przykładowe zgłoszenia:
- możliwość użycia znaków specjalnych w polach First Name i Last Name,
- brak przycisku Cancel podczas składania wniosku urlopowego,
- brak komunikatu walidacyjnego podczas próby dodania pustego posta.

Każde zgłoszenie zawiera:
- opis błędu,
- kroki reprodukcji,
- oczekiwany rezultat,
- rzeczywisty rezultat,
- priorytet,
- załączniki.

---

# Testy wydajnościowe

Testy wydajnościowe zostały wykonane przy użyciu Apache JMeter 5.6.3.

Przetestowane scenariusze:
- strona logowania,
- proces logowania użytkownika,
- Dashboard,
- moduł PIM.

---

# Wykorzystane elementy JMeter

- Thread Group
- HTTP Request
- HTTP Cookie Manager
- HTTP Header Manager
- Response Assertions
- Regular Expression Extractor
- Summary Report
- Aggregate Report
- View Results Tree

---

# Mechanizmy zastosowane w testach

## Token Extraction
Dynamiczne pobieranie tokenu logowania za pomocą Regular Expression Extractor.

## Session Handling
Obsługa sesji użytkownika za pomocą HTTP Cookie Manager.

## Assertions
Walidacja:
- statusów odpowiedzi,
- czasu odpowiedzi,
- tekstu odpowiedzi,
- rozmiaru odpowiedzi.

---

# Narzędzia

- Apache JMeter
- Jira
- TestRail
- Chrome DevTools
- OrangeHRM Demo
- Windows 11
- Microsoft Word

---
# Wyniki testów manualnych

Wykonano 62 przypadki testowe
- Około 97% przypadków testowych zakończyło się statusem Passed
- Wykryto pojedyncze błędy wymagające poprawy
- Nie wystąpiły krytyczne błędy blokujące możliwość dalszego testowania

# Wyniki testów wydajnościowych 

Wykonano 290 requestów.

Przetestowano:
- GET Login Page
- POST Login Request
- GET Dashboard
- GET PIM Employee List

Wyniki zawierają:
- średni czas odpowiedzi,
- throughput,
- error rate,
- aggregate metrics.

---

# Screenshots

Repozytorium zawiera:
- strukturę projektu JMeter,
- Summary Report,
- Aggregate Report,
- View Results Tree,
- przykłady bug reportów,
- przykłady scenariuszy testowych.

---

# Cel projektu

Celem projektu było rozwijanie praktycznych umiejętności w zakresie:
- testów manualnych,
- analizy błędów,
- testów wydajnościowych,
- pracy z narzędziami QA,
- analizy odpowiedzi HTTP,
- obsługi sesji i autoryzacji użytkownika.

## Autor
Aleksandra Janas
