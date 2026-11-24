# Katalog Silników Szachowych — Zbiór Danych Strukturalnych

![Format JSON](https://img.shields.io/badge/Format-JSON-green)
![Format CSV](https://img.shields.io/badge/Format-CSV-orange)
![Kodowanie](https://img.shields.io/badge/Kodowanie-UTF--8-blue)
![Liczba rekordów](https://img.shields.io/badge/Silniki-10-lightgrey)

> **Note:** This repository was created as a university project.

Repozytorium zawiera zestaw danych opisujący **10 nowoczesnych silników szachowych** (*Stockfish*, *Obsidian*, *PlentyChess*, *Integral*, *Reckless*, *Pawnocchio*, *Tarnished*, *Halogen*, *Quanticade*, *Patricia*), zapisany w dwóch formatach wymiany danych: **`JSON`** (`silniki.json`) oraz **`CSV`** (`silniki.csv`).

---

## Spis treści

1. [Temat i struktura zbioru danych](#temat-i-struktura-zbioru-danych)
2. [Status realizacji zadań](#status-realizacji-zadań)

---

## Temat i struktura zbioru danych

Zbiór gromadzi parametry techniczne oraz metadane czołowych silników szachowych open-source. Oba pliki (`silniki.json` i `silniki.csv`) przechowują dokładnie ten sam zestaw 10 rekordów, z których każdy opisany jest przez następujące pola:

* **Identyfikator (`id`)** — unikalny kod silnika w formacie `ENG-XXX` (od `ENG-001` do `ENG-010`).
* **Nazwa (`nazwa`)** — oficjalna nazwa silnika szachowego.
* **Architektura (`architektura`)** — podejście algorytmiczne (*Hybrydowa* — przeszukiwanie drzewa gry alfa-beta wspomagane siecią neuronową NNUE).
* **Status licencyjny (`openSource` / `open_source`)** — wartość logiczna (`true` / `false`) określająca otwartość kodu źródłowego.
* **Rok powstania (`rokPowstania` / `rok_powstania`)**
* **język programowania (`jezykProgramowania` / `jezyk_programowania`)**.
* **Ranking CCRL (`rankingCCRL` / `ranking_ccrl`)** — przybliżona siła gry w punktach Elo według listy rankingowej *Computer Chess Rating Lists*.
* **Parametry techniczne**:
  * minimalna i maksymalna obsługiwana liczba wątków CPU (`minWatkow`, `maxWatkow`),
  * wsparcie dla akceleracji obliczeń na karcie graficznej (`obslugaGPU`).
* **Relacje 1-do-wielu (listy wartości)**:
  * lista głównych autorów i współtwórców projektu (`autorzy`),
  * lista obsługiwanych protokołów komunikacji z interfejsem graficznym (`protokoly`, np. `UCI`).

> **Uwaga:** Wszystkie pliki zostały zapisane w kodowaniu **UTF-8**, co gwarantuje poprawne wyświetlanie polskich znaków oraz znaków diakrytycznych w imionach i nazwiskach autorów (np. *Jonathan Hallström*).

---

## Status realizacji zadań

- [x] Utworzenie publicznego repozytorium na platformie GitHub
- [x] Przygotowanie zbioru danych o 10 silnikach szachowych w formacie `JSON` (`silniki.json`)
- [x] Przygotowanie równoważnego zbioru w formacie tabelarycznym `CSV` (`silniki.csv`)
- [x] Sprawdzenie poprawności składniowej i spójności danych w obu plikach
- [x] Przygotowanie opisu projektu w `README.md` z wykorzystaniem formatowania Markdown
