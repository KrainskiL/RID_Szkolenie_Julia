# Szkolenie Julia - RID
Repozytorium zawiera materiały do szkolenia **Wprowadzenie do Data Science i uczenia maszynowego z językiem Julia** przeprowadzonego w ramach Regionalnej Inicjatywy Doskonałości SGH.

## Program ramowy
1. Wprowadzenie do języka Julia
2. Wirtualne środowisko i zarządzanie pakietami
3. Podstawowe typy danych
4. Przegląd operacji macierzowych i wektorowych
5. Wektoryzacja kodu (dot operator)
6. Praca z ramkami danych (DataFrames.jl, CSV.jl)
7. Wizualizacja danych z biblioteką Plots.jl
8. Generacja wykresów na potrzeby artykułów naukowych z PGFPlotsX.jl
9. Wprowadzenie do uczenia maszynowego z Julia – MLJ.jl
10. Uwagi o integracji z innymi językami programowania – Python oraz R

## Terminy spotkań:
* 14.03.2025 14:00-16:30 MS Teams
* 21.03.2025 14:00-16:30 MS Teams

## Instrukcja przygotowania środowiska

1. Zainstaluj [Julię](https://julialang.org/downloads/). Polecana jest instalacja bez uprawnień administratora (instalacja dla aktywnego użytkownika). W trakcie szkolenia będziemy korzystać z wersji **v1.11.4**.
2. Pobierz materiały:
    * Pobierz archiwum poprzez zielony przycisk `Code` -> `Download zip` i rozpakuj je w łatwo dostępnej lokalizacji LUB
    * Sklonuj repozytorium korzystając w terminalu z komendy `git clone https://github.com/KrainskiL/RID_Szkolenie_Julia`
3. Otwórz terminal i upewnij się że ścieżka robocza jest w folderze głównym pobranego repozytorium.
4. Uruchom Julię komendą `julia`. Jeśli pojawia się błąd dotyczący braku zainstalowanej aplikacji, sprawdź czy Julia znajduje się w [zmiennej środowiskowej PATH](https://julialang.org/downloads/platform/).
5. Po uruchomieniu REPL Julii wpisz następujące komendy:
```julia
using Pkg
pkg"activate ." # uruchomienie wirtualnego środowiska
pkg"instantiate"   # instalacja wymaganych pakietów.
```
6. Zainstaluj środowisko notatnika korzystając z IJulii (komendy w REPL Julii):
```julia
using IJulia
notebook(dir=".")
# Zaakceptuj instalację wpisując Y
```
Jeżeli Jupyter był już zainstalowany na maszynie, krok 6. można pominąć - po kroku 5. kernel Julii powinien być dostępny w interfejsie Jupyter.

## Visual Studio Code

Alternatywnym sposobem pracy z materiałami szkoleniowymi jest IDE [Visual Studio Code](https://code.visualstudio.com/). Do pracy z Julią zalecane jest zainstalowanie [oficjalnej wtyczki](https://github.com/julia-vscode/julia-vscode). VS Code zapewnia dedykowany edytor notatników i wiele funkcji przydatnych w tworzeniu oraz testowaniu kodu źródłowego. ⚠️UWAGA! Niewielka część komend w notatnikach może nie działać poprawnie w środowisku VS Code.

## Materiały dodatkowe

[Julia Academy](https://juliaacademy.com/)

[Julia Language Manual](https://docs.julialang.org/en/v1/)

[Julia for Data Analysis](https://www.manning.com/books/julia-for-data-analysis)
