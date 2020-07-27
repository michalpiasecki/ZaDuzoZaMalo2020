# Projekt aplikacji "Zgadywanka" (gra w "Za dużo, za mało")

Ekstremalnie prosta (w logice) gra w "Za dużo, za mało" realizowana etapowo z "przyrostowym zdobywaniem wiedzy".

---

## Etapy

### Krok 1 - wariant monolityczny

Wszystko w `Main()` - logika i interfejs uzytkownika, wariant aplikacji konsolowej

Zagadnienia:

* `Console.Write()`, `Console.WriteLine()`
* Generowanie liczb losowych (`Random`)
* `Console.ReadLine()`, konwersja napisu na liczbę, obsługa wyjątków zgłaszanych przy konwersji
* Warunkowy wybór: `if-elseif-else`
* pętla

### Krok 2 - wariant modularny (proceduralny)

Refaktoryzacja poprzedniego kodu, klasa traktowana jako moduł, uproszczenie kodu, określenie procedur i funkcji wielokrotnego użycia.

### Krok 3 - wariant obiektowy

* Projekt typu _Class library_, `.Net Standard`
* Klasa `Gra` opisująca model gry (dostarczająca API dla gry)
* Pola klasy, właściwości, metody
* Hermetyzacja
* Testy jednostkowe

### Krok 4 - aplikacja konsolowa oparta na modelu gry

Projekt aplikacji konsolowej, wykorzystującej opracowany model gry.

Podział na część odpowiedzialną za widok (obsługa konsoli) oraz kontroler (komunikację widoku z modelem).

### Krok 5 - aplikacja okienkowa (WinForm) oparta na modelu gry

* model programowania oparty na zdarzeniach
* logika interfejsu

---

## Propozycje rozszerzenia projektu

1. Zaimplementuj wariant gry, w którym to komputer odgaduje liczbę wylosowaną (wymyśloną) przez człowieka, zaś człowiek odpowiada na pytania komputera.

2. Zaimplementuj wariant gry *komputer-człowiek* uwzględniający co najwyżej jedno "oszustwo"
   1. komputer losuje liczbę
   2. człowiek próbuje ja odgadnąć
   3. komputer może (nie musi) raz się "pomylić" podając fałszywą odpowiedź
   4. człowiek wie, że komputer może (nie musi) raz oszukać, ale nie wie kiedy.

3. Zaimplementuj wariant gry z poprzedniego punktu w układzie *człowiek-komputer*.

---

## Wyzwania

### Wyzwanie 1: aplikacja WPF oparta na modelu gry

### Wyzwanie 2: aplikacja ASP .Net oparta na modelu gry

### Wyzwanie 3: aplikacja typu _web service_ oparta na modelu gry

### Wyzwanie 4: aplikacja Xamarin oparta na modelu gry
