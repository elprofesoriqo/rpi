# Organizacja i infrastruktura projektu

> **RankIt | RPI 2026/2027**<br>
> Dokument: RPI-RANKIT-ORG-001 | Wersja: 1.0 | Data: 2026-10-24<br>
> Autorzy: Igor Jankowski, Piotr Ratkowski, Zachariasz Słupski<br>
> Status: opracowanie organizacyjne

## Cel dokumentu

Dokument opisuje organizację projektu RankIt, sposób współpracy oraz miejsce przechowywania kodu i dokumentacji. Repozytorium GitHub jest wspólnym punktem dostępu do materiałów projektu. Podział obowiązków i rytm komunikacji są propozycją organizacyjną. Nie przypisują członkom zespołu niepotwierdzonych umiejętności ani nie stwierdzają, że opisane spotkania już się odbyły.

## 1. Opis projektu i produktu

**RankIt** to aplikacja webowa do tworzenia rankingów i oceniania różnych rzeczy. Jej celem jest zebranie propozycji i ocen w jednym miejscu oraz ułatwienie porównania wyników.

### Proponowany zakres pierwszej wersji

Użytkownik powinien móc utworzyć ranking, dodać do niego oceniane pozycje, przyznać im oceny i zobaczyć uporządkowane wyniki. To podstawowy zakres wynikający z krótkiego opisu aplikacji. Szczegóły, takie jak skala ocen, logowanie, współdzielenie rankingu i zasady edycji, wymagają decyzji zespołu przed implementacją.

Poza pierwszym zakresem proponuje się pozostawić płatności, rekomendacje, powiadomienia i integracje z zewnętrznymi serwisami. Dzięki temu projekt pozostaje mały i możliwy do zademonstrowania w ramach przedmiotu.

### Użytkownicy i potrzeby

- **Twórca rankingu** chce szybko dodać temat i pozycje.
- **Oceniający** chce ocenić pozycje według jasnej skali.
- **Odbiorca wyników** chce łatwo porównać oceny.

Są to robocze persony wynikające z funkcji aplikacji, a nie wyniki badań użytkowników. Głównym ograniczeniem jest czas projektu w roku akademickim 2026/2027. Dokładny termin oddania nie został podany w załączonym opisie zadania. Na obecnym etapie nie wskazano też systemów, z którymi aplikacja ma się integrować.

Obszarem zastosowania jest grupowe porównywanie propozycji, np. pomysłów, miejsc lub produktów. Planowanymi odbiorcami są pojedynczy użytkownicy i małe grupy. Nie przyjęto modelu płatności ani wyników badań rynku.

### Główne etapy

1. Uzgodnienie wymagań i podziału obowiązków.
2. Szkic widoków i decyzja o najprostszym modelu oceniania.
3. Implementacja podstawowego scenariusza tworzenia rankingu i oceniania.
4. Sprawdzenie scenariusza na kilku przykładowych rankingach.
5. Przygotowanie demonstracji i końcowych materiałów.

Daty etapów należy dopasować do harmonogramu przedmiotu.

## 2. Interesariusze i użytkownicy

| Interesariusz | Rola i potrzeba |
| --- | --- |
| Zespół projektowy | Uzgadnia wymagania, buduje aplikację i przygotowuje dokumentację. Skład: Igor Jankowski, Piotr Ratkowski i Zachariasz Słupski. |
| Opiekun przedmiotu | Ocenia zgodność projektu z wymaganiami RPI i udziela wskazówek. Nazwisko opiekuna nie zostało podane. |
| Twórcy rankingów | Przygotowują tematy i pozycje do oceny. |
| Oceniający i odbiorcy | Wystawiają oceny lub korzystają z wyników rankingu. |

## 3. Zespół

Skład zespołu podany przez autorów projektu: **Igor Jankowski, Piotr Ratkowski i Zachariasz Słupski**. Repozytorium należy do konta `elprofesoriqo`, którego publiczna nazwa profilu to Igor Jankowski. Loginy pozostałych członków zostały potwierdzone przez zespół: [Piotr Ratkowski](https://github.com/PitereQ767) (`@PitereQ767`) i [Zachariasz Słupski](https://github.com/Zacharay) (`@Zacharay`). Na dzień 2026-10-24 zaproszenia z dostępem do zapisu oczekują na akceptację; do tego czasu listę współpracowników repozytorium tworzy samo konto właściciela.

Poniższy podział jest propozycją odpowiedzialności na potrzeby małego projektu. Nie opisuje wcześniejszego poziomu umiejętności poszczególnych osób.

| Osoba | Proponowany obszar odpowiedzialności |
| --- | --- |
| Igor Jankowski | Koordynacja, utrzymanie repozytorium, dokumentacja i integracja zmian. |
| Piotr Ratkowski | Projekt widoków i prace nad interfejsem użytkownika. |
| Zachariasz Słupski | Logika rankingów, model danych i sprawdzanie scenariuszy. |

Zespół może pracować zdalnie, korzystając ze wspólnego repozytorium. Ponieważ nie wskazano miejsca pracy ani używanego komunikatora, spotkania online są propozycją, a nie potwierdzonym stanem.

## 4. Komunikacja

Proponowany prosty rytm pracy:

- raz w tygodniu krótkie spotkanie zespołu online, około 15 minut;
- bieżące zadania i decyzje techniczne zapisujemy w GitHub Issues, aby pozostały przy kodzie;
- większe zmiany przechodzą przez Pull Request, a przed połączeniem autor sprawdza podgląd różnic;
- pytania do opiekuna projektu kierujemy kanałem wskazanym przez prowadzącego przedmiot.

Zespół powinien użyć już dostępnego komunikatora, np. Teams albo Discord. Nie przekazano nazwy kanału ani zrzutu ekranu, dlatego raport nie przedstawia zrzutu ani nie sugeruje, że spotkania już się odbyły.

## 5. Repozytorium kodu

- **Adres:** [github.com/elprofesoriqo/rpi](https://github.com/elprofesoriqo/rpi)
- **Właściciel i osoba utrzymująca repozytorium:** Igor Jankowski (`elprofesoriqo`)
- **Przeznaczenie:** kod aplikacji, materiały projektowe oraz historia zmian w Git.
- **Widoczność:** publiczna.

Adres repozytorium jest podany w raporcie i README. Zrzut ekranu strony repozytorium z widocznym zespołem nie został dołączony.

Pracujemy na gałęzi `main`. Zadania wykonujemy na krótkich gałęziach `feature/...`, `fix/...` albo `docs/...`, a ukończone zmiany łączymy z `main` po sprawdzeniu. Zaproszenia do repozytorium dla potwierdzonych kont `@PitereQ767` i `@Zacharay` zostały wysłane i oczekują na akceptację.

Repozytorium nie zawiera jeszcze kodu aplikacji ani konfiguracji jej budowania. Dlatego nie deklaruje się działającego CI ani zautomatyzowanych testów.

## 6. Dokumentacja i szablon

Dokumenty projektu przechowujemy w katalogu `docs/` w tym samym repozytorium co kod. Dzięki temu są dostępne zespołowi razem z historią zmian.

Używamy krótkich nazw z małych liter i łączników, np. `organizacja-i-infrastruktura.md`. Wersję zapisujemy w metryce dokumentu, a historię zmian przechowuje Git. Osoba utrzymująca repozytorium pilnuje nazw, aktualności odnośników i tego, aby dokumenty nie dublowały się. Każdy raport powinien zaczynać się od metryki projektu i dokumentu zgodnej z [szablonem projektu](szablon-dokumentu-projektu.md).

## 7. Narzędzia

| Obszar | Narzędzie i użycie |
| --- | --- |
| Kontrola wersji i współdzielenie kodu | Git oraz GitHub. |
| Zadania i decyzje | GitHub Issues; Pull Requests do przeglądu zmian. |
| Dokumentacja | Markdown w `docs/`, podgląd bezpośrednio na GitHubie. |
| Komunikacja synchroniczna | Teams lub Discord; wybór istniejącego kanału przez zespół. |
| Tworzenie i sprawdzenie aplikacji | Zależne od stosu technologicznego, który nie został jeszcze wskazany. |

Na obecnym etapie nie dokładamy tablicy, CI ani dodatkowych usług, dopóki zespół nie ustali technologii i rzeczywistej potrzeby.

## 8. Wykorzystanie AI i wnioski

AI wykorzystano do odczytania wymagań zadania, przygotowania układu raportu, propozycji prostych zasad repozytorium i redakcji pierwszej wersji dokumentów. Przykładowy prompt (skrót polecenia użytkownika): „Przygotuj prostą dokumentację części o organizacji i infrastrukturze projektu. Aplikacja to RankIt do tworzenia rankingów i oceniania”. Wynikiem była propozycja dokumentacji w repozytorium obejmująca opis projektu, organizację, szablon i prezentację.

AI przyspiesza przygotowanie struktury i tekstu, ale nie potwierdza faktów o umiejętnościach, odbytych spotkaniach, opiekunie ani terminie. Te informacje należy sprawdzić z zespołem. Nie wygenerowano fikcyjnego zrzutu komunikatora ani fikcyjnych wypowiedzi członków zespołu.

### Do potwierdzenia przed prezentacją

- umiejętności członków i ewentualna korekta roboczego podziału zadań;
- nazwisko opiekuna oraz termin oddania projektu;
- używany komunikator i rzeczywisty zrzut ekranu kanału zespołu;
- decyzje o skali ocen, logowaniu i udostępnianiu rankingów.

## Podstawa

Opis zadania „Organizacja i infrastruktura projektu”, Realizacja projektu informatycznego 2026/2027, przekazany plik PDF.

---

RankIt | RPI-RANKIT-ORG-001 | v1.0 | 2026-10-24
